---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

My research focuses on automatic optimization for ML and HPC systems, with current work in autotuning, compiler/runtime systems, hardware-aware optimization, and efficient LLM inference.

Automatic System Optimization / Autotuning
======

**HYPERF**  
End-to-end autotuning for high-performance computing. I evaluated HYPERF against an OpenTuner baseline across PolyBench kernels; HYPERF achieved a 6.0x average execution speedup and 1.2x faster tuning convergence. Published at HPDC 2025.

**UniTune**  
UniTune is an autotuning framework for exploring large, hierarchical search spaces. For the SC 2026 submission, I profiled row-binning strategies for the SpMV workload across matrices from the SuiteSparse Matrix Collection, developed a hierarchical ML selector to identify promising configurations, and integrated its predictions into UniTune's sampler. For the next submission, I am adapting a bandit-based Rising-Successive Rejects (R-SR) budget allocation strategy to UniTune's hierarchical search space.

Efficient LLM Systems / Sparse Computing
======

**Towards Batched Activation Sparsity in LLM Decoding** *(Master's thesis)*
Motivated by TEAL (ICLR 2025), I investigated whether batch-shared activation sparsity remains effective during autoregressive LLM decoding while preserving model quality. I developed an oracle analysis and Triton block-sparse GEMM kernels. The project found 64% per-decoding-step sparsity potential at batch size 16, while revealing a gap between the oracle upper bound and practical online sparsification due to quality degradation and autoregressive error accumulation.
