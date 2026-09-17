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
Autotuning framework work around data-driven search-space exploration. For the SC 2026 submission, I worked on SuiteSparse SpMV autotuning by profiling row-binning strategies, developing a hierarchical ML selector, and integrating predicted top configurations into UniTune's sampler. For the resubmission preparation, I am exploring how a bandit-based R-SR budget allocation strategy can be adapted to UniTune's hierarchical search space.

Efficient LLM Systems / Sparse Computing
======

**Towards Batched Activation Sparsity in LLM Decoding**  
Master's thesis on whether activation sparsity remains effective under batched autoregressive LLM decoding while preserving model quality. I developed oracle analyses and Triton block-sparse GEMM kernels for Llama 2 7B on an NVIDIA A100X. The project found substantial oracle per-step sparsity potential, 64% at batch size 16, while revealing a gap between oracle upper bounds and practical online sparsification due to quality degradation and autoregressive error accumulation.
