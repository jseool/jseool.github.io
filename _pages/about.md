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
      <p>I received a Master of Data Science from Seoul National University, advised by <a class="lab-link" href="https://hsung.snu.ac.kr/bio" title="Visit Prof. Hyojin Sung's website">Prof. Hyojin Sung&nbsp;<i class="fas fa-external-link-alt external-link-icon" aria-hidden="true"></i></a> in <a class="lab-link" href="https://codelab.snu.ac.kr/" title="Visit CODE Lab's website">CODE Lab&nbsp;<i class="fas fa-external-link-alt external-link-icon" aria-hidden="true"></i></a>, where I continue to collaborate on autotuning research.</p>
      <p>My research lies at the intersection of <strong>machine learning and computer systems</strong>, with a focus on automated system optimization. I have worked on compiler autotuning and ML-guided configuration selection for high-performance computing, as well as activation sparsity and GPU kernel optimization for efficient LLM inference. My goal is to develop methods that <strong>automatically discover hardware-efficient execution</strong> strategies while reducing search costs and manual tuning.</p>
      <p><strong>Status:</strong> I am applying to <strong>Computer Science Ph.D. programs for Fall 2027</strong>.</p>
    </div>
    <figure class="about-photo">
      <img src="/images/junseo-lee.jpg" alt="Portrait of Junseo Lee">
    </figure>
  </div>
</section>

<section id="research-interests" class="home-section">
  <h2>Research Interests</h2>
  <ul class="research-interest-list">
    <li><strong>ML for Systems &amp; Autotuning:</strong> ML-guided performance modeling and efficient optimization search.</li>
    <li><strong>Compilers &amp; Runtime Systems:</strong> Compiler optimization and hardware-aware execution.</li>
    <li><strong>Efficient ML Systems:</strong> GPU kernel optimization and efficient ML inference.</li>
  </ul>
</section>

<section id="publications" class="home-section">
  <h2>Publications</h2>
  <p><strong><a class="publication-title" href="https://doi.org/10.1145/3731545.3731588">HYPERF: End-to-End Autotuning Framework for High-Performance Computing</a></strong> <a class="publication-paper-link" href="https://doi.org/10.1145/3731545.3731588" aria-label="View HYPERF paper on ACM" title="View paper (ACM)"><i class="fas fa-file-pdf" aria-hidden="true"></i></a><br>
  Juseong Park<sup>*</sup>, Yongwon Shin<sup>*</sup>, Junghyun Lee, <strong>Junseo Lee</strong>, Juyeon Kim, Oh-Kyoung Kwon, and Hyojin Sung. <small>* Co-first authors.</small><br>
  In the 34th International Symposium on High-Performance Parallel and Distributed Computing (<strong>HPDC</strong>), 2025.</p>
</section>

<section id="research-projects" class="home-section">
  <h2>Research Projects</h2>

  <h3>Compiler Autotuning</h3>

  <p class="project-title"><strong>HYPERF</strong> <em>(HPDC 2025)</em> <a class="publication-paper-link" href="https://doi.org/10.1145/3731545.3731588" aria-label="View HYPERF paper on ACM" title="View paper (ACM)"><i class="fas fa-file-pdf" aria-hidden="true"></i></a></p>
  <ul class="project-details">
    <li>Evaluated HYPERF, an end-to-end autotuning framework, against OpenTuner on PolyBench kernels, demonstrating a <strong>6.0&times; average execution speedup</strong> and <strong>1.2&times; faster tuning convergence</strong>.</li>
  </ul>

  <p class="project-title"><strong>Sparse Matrix-Vector Multiplication (SpMV) Optimization</strong> <em>(HYPERF follow-up)</em></p>
  <ul class="project-details">
    <li>Profiled an SpMV optimization that groups matrix rows with similar numbers of nonzero elements to improve load balancing.</li>
    <li>Developed an ML-based selector using XGBoost to predict when the optimization is beneficial and C5.0 to recommend promising tuning configurations.</li>
    <li>Integrated the predictions into HYPERF v2's autotuning sampler, <strong>reducing tuning trials by 60% (570 &rarr; 230)</strong> while achieving <strong>performance within 5% of the best configuration</strong>.</li>
  </ul>

  <p class="project-title"><strong>Autotuning Search and Cost Model Analysis</strong> <em>(Ongoing)</em></p>
  <ul class="project-details">
    <li>Investigating why TVM's autotuner misses high-performing schedules. The analysis focuses on the cost model's predictions for candidate schedules and the role of random exploration.</li>
  </ul>

  <h3>Efficient LLM Inference</h3>

  <p class="project-title"><strong>Towards Batched Activation Sparsity in LLM Decoding</strong> <em>(Master's Thesis)</em></p>
  <ul class="project-details">
    <li>Investigated whether blocked activation sparsity could be shared across sequences to accelerate batched LLM decoding without compromising model quality.</li>
    <li>Developed an oracle analysis and <strong>Triton block-sparse GEMM kernels</strong> to evaluate sparsity potential and GPU performance under batching.</li>
    <li>Found <strong>64% average oracle sparsity</strong> at batch size 16 through independent per-step analysis, corresponding to an estimated <strong>1.6&times; kernel-only speedup</strong> over dense cuBLAS.</li>
    <li>Identified a substantial gap between oracle sparsity potential and practical online execution: an online heuristic achieved only 11.5% sparsity with limited quality degradation, and end-to-end decoding throughput reached only 0.59&times; the dense baseline.</li>
  </ul>
</section>

<section id="education" class="home-section">
  <h2>Education</h2>

  <div class="education-entry">
    <h3>Seoul National University</h3>
    <p>Master of Data Science | 2024 - 2026</p>
    <p>Advisor: <a class="lab-link" href="https://hsung.snu.ac.kr/bio" title="Visit Prof. Hyojin Sung's website">Hyojin Sung&nbsp;<i class="fas fa-external-link-alt external-link-icon" aria-hidden="true"></i></a> (<a class="lab-link" href="https://codelab.snu.ac.kr/" title="Visit CODE Lab's website"><strong>C</strong>omputing <strong>O</strong>ptimization and <strong>D</strong>ata-driven <strong>E</strong>xploration Lab&nbsp;<i class="fas fa-external-link-alt external-link-icon" aria-hidden="true"></i></a>)</p>
    <p><em>Thesis: Towards Batched Activation Sparsity in LLM Decoding</em></p>
  </div>

  <div class="education-entry">
    <h3>Yonsei University</h3>
    <p>B.A. in Applied Statistics | 2020 - 2024</p>
  </div>

  <div class="education-entry">
    <h3>University of California, Berkeley</h3>
    <p>UCEAP Exchange Program (Statistics) | 2022 - 2023</p>
  </div>
</section>
