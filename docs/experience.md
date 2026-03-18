# Professional Experience

## NSF-National Center for Atmospheric Research (NSF-NCAR) &mdash; Boulder, CO

<div class="timeline">

<div class="timeline-item">

### HPC Consultant / Computational Scientist
<div class="meta"><span class="dates">Oct 2022 – Present</span> · CISL · <em>Supervisor: Dr. Ben Kirk</em></div>

- **Technical Lead, NSF-NCAR Community AI Ecosystem:** Leading an initiative across all NCAR labs to build an open, modular platform unifying data pipelines, scalable multi-GPU training, and inference for NCAR's converged HPC+AI infrastructure. Authored a comprehensive AI/ML cyberinfrastructure needs assessment — covering distributed training frameworks, data infrastructure, GPU-accelerated pipelines and preprocessing, and hybrid physics-ML integration — that defined the opportunity space, platform architecture, and adoption strategy for AI/ML in Earth-system science at NCAR.

- Primary architect of NCAR's **distributed scientific ML training infrastructure** — designed and scaled multi-node, multi-GPU training systems on NCAR's Derecho supercomputer, implementing data parallel (DDP), fully sharded training (FSDP), model and tensor parallelism, and hybrid strategies in PyTorch and JAX for large-scale geoscientific AI models across multiple NCAR research groups.

- Core technical contributor to the **MILES CREDIT global weather prediction platform** — implemented DDP, FSDP, and domain-parallel training strategies to scale graph neural network and transformer architectures for multi-node global weather forecasting.

- Architected **GPU-native data loading pipelines** for large, multidimensional Earth system datasets using NVIDIA DALI, KvikIO, and CuPy-based preprocessing, minimizing host-device transfers and enabling high-throughput end-to-end training in I/O-bound AI/ML workflows. Demonstrated **~17x training throughput improvement** through optimized Zarr v3 chunking, GPU Direct Storage, GPU-based decompression (nvCOMP), and DALI pipelining.

- Profiled and optimized scientific AI training and inference workflows using **NVIDIA Nsight Systems and Linaro MAP** — identifying communication, I/O, and memory bottlenecks. Achieved **~55x speed-up** by removing I/O bottlenecks and improving torch dataloaders.

- Developed **performance benchmarks** to diagnose and eliminate communication and parallel I/O bottlenecks in end-to-end AI/ML workflows in ESS; established best practices for NCCL configuration, CUDA-aware MPI tuning, Zarr chunking and sharding optimization for Lustre, GPU-native data loader design, and parallel read strategies.

- Designed and delivered **advanced technical curriculum** on training, scaling, and optimizing PyTorch-based AI/ML workflows for weather modeling. Delivered hands-on workshops (SciPy, ESDS, NCAR) on scalable geospatial data analysis using Dask, CuPy-Xarray, and Zarr.

- Active contributor to **open-source projects** including Xarray, CuPy-Xarray, Zarr, WRF, CESM, CTSM. Contributed multiple Pythia Cookbooks.

- Evaluated and benchmarked **domain-specific AI/ML frameworks** — NVIDIA PhysicsNeMo, ECMWF Anemoi, CREDIT — to inform NCAR's AI infrastructure roadmap.

- Led the **NCAR HPC User Group (NHUG, 300+ members)**, fostering best practices in computational geoscience and AI/ML workflows.

- Built **LLM-based RAG systems** (RAGNA) to automate scientific knowledge extraction and data discovery.

</div>

<div class="timeline-item">

### Associate Scientist III
<div class="meta"><span class="dates">Apr 2021 – Oct 2022</span> · CGD · <em>Supervisor: Dr. David Lawrence</em></div>

- Developed Python-based frameworks for automated domain subsetting, scalable regridding, and running single-point and regional CTSM simulations.

- Designed interactive visualization dashboards for evaluation of weather and climate simulations against tower observations (NCAR-NEON) and for the LENS-2 large ensemble dataset.

- Created a user-friendly framework and tutorials for Docker-based land simulations and analysis in Jupyter-Lab.

</div>

<div class="timeline-item">

### Scientific Software Engineer II
<div class="meta"><span class="dates">Jan 2019 – Apr 2021</span> · CGD · <em>Supervisor: Dr. David Lawrence</em></div>

- Designed and developed a lightweight infrastructure for coupling of various NWP models (WRF) to CTSM using ESMF.

- Developed a Python-based framework for visualization, statistical analysis, and performance evaluation of several WRF simulations against observations and satellite data.

</div>

<div class="timeline-item">

### ASP Postdoctoral Fellow
<div class="meta"><span class="dates">Sep 2017 – Jan 2019</span> · ASP · <em>Supervisor: Dr. Richard Loft</em></div>

- Implemented and evaluated various ML and DL algorithms for seasonal and sub-seasonal forecast of extreme heat events.

- Designed and trained deep neural networks for emulating complex cloud microphysical processes.

- Co-supervised four interns on neural network architectures for seasonal forecasts and WRF/WRF-Chem performance optimization.

</div>

<div class="timeline-item">

### Visiting Graduate Assistant
<div class="meta"><span class="dates">May 2015 – Aug 2017</span> · CISL · <em>Supervisor: Dr. Davide Del Vento</em></div>

- Analyzed performance and identified major bottlenecks in WRF and WRF-Chem using PAPI, TAU, Intel VTune XE, and Linaro MAP.

- Performed node-level optimization of WRF advection kernel for Intel, GNU, and PGI compilers.

- Accelerated WRF and WRF-Chem advection kernel on Intel Xeon and Xeon Phi (MIC).

- Ported performance-critical sections of WRF/MPAS to GPU using OpenACC directives.

</div>

</div>
