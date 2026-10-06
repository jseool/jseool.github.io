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
  <div class="about-layout">
    <div class="about-copy">
      <p>I am interested in building systems that automatically optimize complex ML workloads. My research focuses on making this optimization practical by reducing search costs and adapting execution to the underlying hardware.</p>
      <p>I received a Master of Data Science from Seoul National University, where I worked as a graduate researcher in the <a class="lab-link" href="https://codelab.snu.ac.kr/">CODE Lab</a>. I worked on compiler autotuning for high-performance computing, developing data-driven autotuning strategies. I also investigated activation sparsity for efficient LLM inference and developed sparse GPU kernels. I continue to collaborate with the lab on an autotuning framework.</p>
      <p><strong>Status:</strong> I am applying to <strong>Computer Science Ph.D. programs for Fall 2027</strong>, with a focus on computer systems and ML systems.</p>
    </div>
    <figure class="about-photo">
      <img src="/images/junseo-lee.jpg" alt="Portrait of Junseo Lee">
    </figure>
  </div>
</section>

<section id="research-interests" class="home-section">
  <h2>Research Interests</h2>
  <ul class="research-interest-list">
    <li><strong>ML Systems &amp; Compilers:</strong> Compiler and runtime optimization for ML workloads</li>
    <li><strong>Autotuning &amp; Search Algorithms:</strong> Efficient exploration of large optimization spaces</li>
    <li><strong>Hardware-aware Execution:</strong> Efficient GPU kernels and sparse computation</li>
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
  An end-to-end autotuning framework for high-performance computing. I evaluated HYPERF against OpenTuner on PolyBench kernels, demonstrating a 6.0x average execution speedup and 1.2x faster tuning convergence. <em>Published at HPDC 2025.</em></p>

  <p><strong>SpMV Workload Optimization</strong> <em>(HYPERF follow-up)</em><br>
  I built an ML-based selector for sparse matrix-vector multiplication (SpMV). It uses XGBoost to decide whether to group rows by their nonzero counts and a C5.0 decision tree to select grouping configurations (nonzero-count interval and number of groups) for evaluation. Integrating its predictions into the autotuning sampler reduced configuration evaluations from 570 to 230 to reach within 5% of the best observed execution time across matrices from the SuiteSparse Matrix Collection. <em>Included in the SC 2026 submission.</em></p>

  <p><strong>Autotuning Sampler and TVM Cost Model</strong><br>
  In ongoing follow-up work on HYPERF, I am adapting Rising-Successive Rejects to allocate more evaluation budget to promising combinations of algorithm parameters and polyhedral structures in the autotuning sampler. I am also applying bootstrap aggregation to TVM's execution-time prediction model to improve its reliability with limited training data. <em>In preparation for OSDI.</em></p>

  <h3>Efficient LLM Systems / Sparse Computing</h3>

  <p><strong>Towards Batched Activation Sparsity in LLM Decoding</strong> <em>(Master's thesis)</em><br>
  I developed an oracle analysis and Triton block-sparse GPU kernels to study sharing activation sparsity across sequences in batched LLM decoding. The oracle showed approximately 64% average block sparsity at batch size 16 when each decoding step was evaluated independently. With limited model-quality degradation, an online heuristic achieved only 11.5% average sparsity. Mask-selection overhead made end-to-end decoding slower than dense execution, with throughput at only 0.59&times; the dense baseline.</p>
</section>

<section id="education" class="home-section">
  <h2>Education</h2>

  <div class="education-entry">
    <h3>Seoul National University</h3>
    <p>Master of Data Science, 2024-2026. Advisor: Hyojin Sung.</p>
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
