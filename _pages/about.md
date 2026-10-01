---
permalink: /
title: "Junseo Lee"
author_profile: false
one_page: true
redirect_from:
  - /about/
  - /about.html
---

<section id="about" class="home-section">
  <h2>About</h2>
  <p>I am interested in building systems that automatically find efficient ways to run complex ML workloads. My research focuses on reducing search costs and adapting execution to the underlying hardware.</p>
  <p>During my M.S. at Seoul National University, I worked on compiler autotuning and efficient LLM inference, including search over large optimization spaces, activation sparsity, and sparse GPU kernels.</p>
  <p>I am preparing for Fall 2027 Ph.D. applications in computer systems and ML systems. I hope to develop systems that optimize ML workloads across algorithms, compilers, runtimes, and hardware, making high-performance execution easier to achieve without extensive manual tuning.</p>
</section>

<section id="research-interests" class="home-section">
  <h2>Research Interests</h2>
  <ul class="research-interest-list">
    <li>Computer systems</li>
    <li>ML systems</li>
    <li>Compilers and runtime systems</li>
    <li>Autotuning</li>
    <li>Hardware-aware optimization</li>
  </ul>
</section>

<section id="publications" class="home-section">
  <h2>Publications</h2>
  <p><strong><a class="publication-title" href="https://doi.org/10.1145/3731545.3731588">HYPERF: End-to-End Autotuning Framework for High-Performance Computing</a></strong><br>
  Juseong Park<sup>*</sup>, Yongwon Shin<sup>*</sup>, Junghyun Lee, <strong>Junseo Lee</strong>, Juyeon Kim, Oh-Kyoung Kwon, and Hyojin Sung.<br>
  HPDC 2025. <small>* Co-first authors.</small></p>
</section>

<section id="research-projects" class="home-section">
  <h2>Research Projects</h2>

  <h3>Automatic System Optimization / Autotuning</h3>

  <p><strong>HYPERF</strong><br>
  End-to-end autotuning for high-performance computing. I evaluated HYPERF against an OpenTuner baseline across PolyBench kernels; HYPERF achieved a 6.0x average execution speedup and 1.2x faster tuning convergence. Published at HPDC 2025.</p>

  <p><strong>HYPERF v2</strong><br>
  HYPERF v2 is an autotuning framework for exploring large, hierarchical search spaces. For the SC 2026 submission, I profiled row-binning strategies for the SpMV workload across matrices from the SuiteSparse Matrix Collection, developed a hierarchical ML selector to identify promising configurations, and integrated its predictions into HYPERF v2's sampler. For the next submission, I am adapting a bandit-based Rising-Successive Rejects (R-SR) budget allocation strategy to efficiently explore HYPERF v2's hierarchical search space.</p>

  <h3>Efficient LLM Systems / Sparse Computing</h3>

  <p><strong>Towards Batched Activation Sparsity in LLM Decoding</strong> <em>(Master's thesis)</em><br>
  Motivated by the potential of activation sparsity to accelerate LLM inference, I investigated whether TEAL's approach could be extended to batch-shared sparsity during autoregressive decoding while preserving model quality. I developed an oracle analysis and Triton block-sparse GEMM kernels. The project found 64% per-decoding-step sparsity potential at batch size 16, while revealing a gap between the oracle upper bound and practical online sparsification due to quality degradation and autoregressive error accumulation.</p>
</section>

<section id="education" class="home-section">
  <h2>Education</h2>

  <div class="education-entry">
    <h3>Seoul National University</h3>
    <p>M.S. in Data Science, 2024-2026. Advisor: Hyojin Sung.</p>
  </div>

  <div class="education-entry">
    <h3>Yonsei University</h3>
    <p>B.A. in Applied Statistics, 2020-2024.</p>
  </div>

  <div class="education-entry">
    <h3>University of California, Berkeley</h3>
    <p>UCEAP Exchange Program, 2022-2023.</p>
  </div>
</section>
