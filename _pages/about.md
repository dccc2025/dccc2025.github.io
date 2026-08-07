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
    <span>LLM Quantization</span>
    <span>Multimodal LLMs</span>
    <span>Large Audio Models</span>
    <span>Embodied Simulation</span>
    <span>Quantum Machine Learning</span>
    <span>Physical AI</span>
    <span>Hyperspectral Image Processing</span>
    <span>Heat-assisted Detection and Ranging</span>
  </div>
  <p>
    My current research focuses on LLM quantization, multimodal LLMs, and physical AI.
  </p>
  <p>
    I also have experience with <strong><a href="https://www.nature.com/articles/s41586-023-06174-6">HADAR-based physical vision</a></strong>; <strong>audio signal processing</strong>, including text-to-speech, pattern recognition, and downstream task fine-tuning; and <strong>embodied simulation</strong>, including asset development, teleoperation, and plugin development.
  </p>
  <p class="home-alert">I am actively seeking 27 Fall PhD opportunities!</p>
  <p>
    I am always open to collaborations and discussions. Please feel free to contact me.
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
    <a class="home-work__figure" href="https://arxiv.org/pdf/2608.02192">
      <img src="{{ base_path }}/images/projects/t2exture_main_figure_web.jpg" alt="T squared exture thermal texture imaging framework">
    </a>
    <div class="home-work__body">
      <h3>T<sup>2</sup>exture: Sparsely Perturbed Thermal-to-Texture Imaging</h3>
      <p class="home-work__meta">arXiv 2026 · Thermal texture imaging under sparse active acquisition</p>
      <p>
        T<sup>2</sup>exture reconstructs temporally dense thermal texture sequences from densely sampled passive frames and a small number of actively perturbed keyframes, using source-off state estimation and structure- and semantic-guided propagation.
      </p>
      <p class="home-work__links">
        <a href="https://arxiv.org/pdf/2608.02192">Paper</a>
        <span>/</span>
        <a href="https://github.com/dccc2025/T2exture">Code</a>
        <span>/</span>
        <a href="https://huggingface.co/datasets/chenjiashuo/T2exture_datasets">Dataset</a>
        <span>/</span>
        <a href="https://huggingface.co/chenjiashuo/T2exture_model">Model Weights</a>
      </p>
    </div>
  </article>

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
