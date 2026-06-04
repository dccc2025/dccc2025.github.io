---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<style>
  .cv-entry {
    margin-top: 1rem;
    max-width: 720px;
  }

  .cv-status {
    color: #9B1C31;
    font-weight: 700;
    font-size: 1.08em;
    margin-bottom: 1.05rem;
  }

  .cv-link-row {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
    gap: 0.65rem;
    margin-bottom: 0.85rem;
  }

  .cv-link-label {
    font-weight: 600;
  }

  .cv-link-button {
    display: inline-flex;
    align-items: center;
    gap: 0.45rem;
    margin: 0;
  }

  .cv-view-counter {
    margin-top: 0.35rem;
  }
</style>

<div class="cv-entry">
  <p class="cv-status">
    I am actively seeking Fall 2027 Ph.D. opportunities.
  </p>

  <div class="cv-link-row">
    <span class="cv-link-label">Click here to see my CV:</span>
    <a class="btn btn--primary cv-link-button" href="{{ base_path }}/files/ChengDai_cv.pdf" target="_blank" rel="noopener">
      <i class="fas fa-file-pdf" aria-hidden="true"></i>
      <span>CV Here</span>
    </a>
  </div>

  <p class="cv-view-counter">
    <img src="https://hits.sh/dccc2025.github.io/cv.svg?label=CV%20views&color=9B1C31&labelColor=343A40" alt="CV page view counter">
  </p>
</div>
