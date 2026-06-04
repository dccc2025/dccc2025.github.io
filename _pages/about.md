---
permalink: /
title: "Cheng Dai"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

{% include base_path %}

<section class="home-intro">
  <div class="home-skills" aria-label="Research skills">
    <span>Thermal Inversion</span>
    <span>Computational Imaging</span>
    <span>Generative AI</span>
    <span>Multimodal LLMs</span>
    <span>Audio Intelligence</span>
    <span>Embodied AI Systems</span>
    <span>Lightweight Deployment</span>
  </div>
  <p>
    I work on thermal infrared hyperspectral imaging, HADAR-based physical vision, and efficient AI systems that move visual perception beyond appearance-only sensing. My current research focuses on temperature-emissivity-texture decomposition, physically interpretable thermal perception, and lightweight deployment for practical sensing systems.
  </p>
  <p class="home-alert">I am actively seeking 27 Fall PhD opportunities!</p>
  <p>
    I am deeply grateful for the guidance and support I have received from my mentors, senior students, and friends.
  </p>
  <p>
    I am always open to collaborations and discussions. Please feel free to contact me at <a href="mailto:daicheng@westlake.edu.cn">daicheng@westlake.edu.cn</a>.
  </p>
  <p class="home-actions">
    <a class="home-button" href="{{ base_path }}/files/ChengDai_cv.pdf">CV</a>
    <a class="home-button" href="{{ base_path }}/publications/">Publications</a>
    <a class="home-button" href="https://github.com/dccc2025">GitHub</a>
  </p>
</section>

<section class="home-section">
  <h2>Selected Works</h2>

  <article class="home-work">
    <a class="home-work__figure" href="https://arxiv.org/abs/2606.03806">
      <img src="{{ base_path }}/images/projects/tex1500_architecture_web.jpg" alt="TeX-UNet architecture for TeX-1500">
    </a>
    <div class="home-work__body">
      <h3>TeX-1500: A Paired Real-World LWIR Hyperspectral Dataset and Benchmark</h3>
      <p class="home-work__meta">arXiv 2026 · Dataset and baseline for temperature-emissivity-texture decomposition</p>
      <p>
        TeX-1500 introduces a paired real-world long-wave infrared hyperspectral dataset for supervised HSI-to-TeX learning, together with TeX-UNet as a wavelength-aware baseline for physical-property-centered thermal perception.
      </p>
      <p class="home-work__links">
        <a href="https://arxiv.org/abs/2606.03806">Paper</a>
        <span>/</span>
        <a href="https://github.com/dccc2025/TeX-1500">Code</a>
        <span>/</span>
        <a href="https://huggingface.co/datasets/jialelin2007/TeX-1500">Dataset</a>
        <span>/</span>
        <a href="https://huggingface.co/dccc2025/TeX-UNet">Model Weights</a>
      </p>
    </div>
  </article>

  <article class="home-work">
    <a class="home-work__figure" href="https://arxiv.org/abs/2605.13664">
      <img src="{{ base_path }}/images/projects/hair_main_figure_web.jpg" alt="HAIR restoration framework">
    </a>
    <div class="home-work__body">
      <h3>HADAR-Based Thermal Infrared Hyperspectral Image Restoration</h3>
      <p class="home-work__meta">arXiv 2026 · Physics-driven restoration for thermal infrared hyperspectral imaging</p>
      <p>
        HAIR restores degraded TIR-HSI through a physics-driven pipeline that combines degradation clean-up, spectral calibration, and TeX decomposition-synthesis under the HADAR radiative-transfer view.
      </p>
      <p class="home-work__links">
        <a href="https://arxiv.org/abs/2605.13664">Paper</a>
        <span>/</span>
        <a href="https://github.com/jialelin2007/HAIR">Code</a>
      </p>
    </div>
  </article>
</section>

<section class="home-section">
  <h2>Timeline</h2>
  <div class="home-timeline">
    <div class="home-timeline__item">
      <span>2026.06</span>
      <p><strong>TeX-1500</strong> released as a paired real-world LWIR HSI-TeX dataset and benchmark.</p>
    </div>
    <div class="home-timeline__item">
      <span>2026.05</span>
      <p><strong>HAIR</strong> released as a HADAR-based restoration framework for thermal infrared hyperspectral images.</p>
    </div>
    <div class="home-timeline__item">
      <span>2025.09 - Current</span>
      <p><strong>Research Assistant, AI for Physics Lab, Westlake University.</strong> Worked on HADAR algorithms, TeX decomposition, and lightweight thermal perception under the guidance of Xin Yuan and Fanglin Bao.</p>
    </div>
    <div class="home-timeline__item">
      <span>2025.04 - 2025.09</span>
      <p><strong>Audio AI Intern, Amoon AI.</strong> Worked on low-resource infant-cry activity detection and state classification, audio foundation-model fine-tuning, and edge deployment.</p>
    </div>
    <div class="home-timeline__item">
      <span>2024.12 - 2025.02</span>
      <p><strong>AI Engineering Intern, Lightwheel AI.</strong> Built engineering tools for embodied AI workflows, including RoboCasa plugin development and teleoperation tooling.</p>
    </div>
    <div class="home-timeline__item">
      <span>2025.09 - 2026.03</span>
      <p><strong>Graduate Study, Wuhan University.</strong> Studied Communication Engineering at the State Key Laboratory of Surveying, Mapping and Remote Sensing Information Engineering.</p>
    </div>
    <div class="home-timeline__item">
      <span>2021.08 - 2025.06</span>
      <p><strong>B.Eng. in Communication Engineering, Jilin University.</strong> Built foundations in signal processing, communication systems, mathematical modeling, and engineering practice.</p>
    </div>
  </div>
</section>
