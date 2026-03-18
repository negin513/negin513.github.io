---
date: 2025-07-09
categories:
  - AI/ML
  - HPC
tags:
  - GPU
  - Zarr
  - Xarray
  - DALI
  - CuPy
  - Performance
authors:
  - negin
---

# It is all about I/O!

**Read the full blog post about GPU-native data loading here: [https://xarray.dev/blog/gpu-pipeline](https://xarray.dev/blog/gpu-pipeline)**

Data loading is a major bottleneck in AI/ML workflows, especially when working with large geoscientific datasets. At a hackathon, we explored how GPU-native data loaders using Zarr v3, CuPy, and DALI can help overcome this bottleneck and accelerate end-to-end workflows.

<!-- more -->

In typical ML pipelines for Earth system science, the GPU sits idle waiting for the CPU to load and preprocess data. With datasets like ERA5 that can be hundreds of terabytes, this I/O bottleneck severely limits training throughput.

During a few days at the hackathon, we built a GPU-native pipeline that moves data loading and preprocessing onto the GPU:

- **Optimized chunking** — Rechunked ERA5 data to align with model access patterns using Zarr v3
- **Direct-to-GPU reads** — Used KvikIO and Zarr Python 3's `zarr.config.enable_gpu()` to read data directly into GPU memory
- **GPU-based decompression** — Leveraged NVIDIA nvCOMP for Zstandard decompression on GPU, eliminating CPU-side decompression
- **NVIDIA DALI pipelining** — Overlapped CPU and GPU compute to minimize idle time on both

The combined optimizations achieved **~17x improvement** in training throughput on a single GPU by eliminating I/O bottlenecks and maximizing GPU utilization.

For detailed benchmarks, implementation details, and code, read the full blog post at [xarray.dev/blog/gpu-pipeline](https://xarray.dev/blog/gpu-pipeline).
