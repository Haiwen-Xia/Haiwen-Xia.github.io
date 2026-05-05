---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

<style>
  .paper-box {
    display: flex;
    align-items: flex-start;
    gap: 1.5rem;
    margin: 1.5rem 0 2rem;
    padding: 1.25rem;
    border: 1px solid #e6e6e6;
    border-radius: 18px;
    background: linear-gradient(180deg, #ffffff 0%, #fafafa 100%);
    box-shadow: 0 12px 28px rgba(15, 23, 42, 0.08);
  }

  .paper-box-image {
    flex: 0 0 280px;
  }

  .paper-box-image-inner {
    position: relative;
  }

  .paper-box-image img {
    display: block;
    width: 100%;
    border-radius: 14px;
    border: 1px solid #dddddd;
    background: #f5f5f5;
  }

  .paper-badge {
    position: absolute;
    top: 12px;
    left: 12px;
    display: inline-block;
    padding: 0.3rem 0.75rem;
    border-radius: 999px;
    background: rgba(148, 24, 24, 0.92);
    color: #ffffff;
    font-size: 0.82rem;
    font-weight: 700;
    letter-spacing: 0.02em;
  }

  .paper-box-text {
    flex: 1 1 auto;
    min-width: 0;
  }

  .paper-box-text h3 {
    margin-top: 0;
    margin-bottom: 0.75rem;
  }

  .paper-box-text p {
    margin-bottom: 0.75rem;
  }

  .paper-links {
    margin-bottom: 0.9rem;
    font-weight: 600;
  }

  .paper-links a {
    margin-right: 1rem;
  }

  .paper-box-text ul {
    margin-top: 0.5rem;
  }

  .paper-box-text li {
    margin-bottom: 0.45rem;
  }

  @media (max-width: 768px) {
    .paper-box {
      flex-direction: column;
    }

    .paper-box-image {
      flex-basis: auto;
      width: 100%;
    }
  }
</style>

## News

- *2026.05*: The Paper "CMI-RewardBench: Evaluating Music Reward Models with Compositional Multimodal Instruction" has been accepted by ICML 2026.

## Featured Publication

<div class='paper-box'>
  <div class='paper-box-image'>
    <div class='paper-box-image-inner'>
      <div class='paper-badge'>ICML 2026</div>
      <img src="{{ '/images/publications/CMI-RewardBench.png' | relative_url }}" alt="CMI-RewardBench">
    </div>
  </div>
  <div class='paper-box-text'>
    <h3><a href="https://arxiv.org/abs/2603.00610">CMI-RewardBench: Evaluating Music Reward Models with Compositional Multimodal Instruction</a></h3>
    <p>Yinghao Ma*, Haiwen Xia*, Hewei Gao, Weixiong Chen, Yuxin Ye, Yuchen Yang, Sungkyun Chang, Mingshuo Ding, Yizhi Li, Ruibin Yuan, Simon Dixon, Emmanouil Benetos</p>
    <p class="paper-links"><a href="https://arxiv.org/abs/2603.00610">Paper</a><a href="{{ '/publication/cmi-rewardbench' | relative_url }}">Details</a></p>
    <ul>
      <li>Introduced a new task for evaluating generated audio from compositional music instructions.</li>
      <li>Created the CMI-Pref dataset using 23 music generation models, with 110k LLM-labeled preferences, 797 hours of generated audio, and a human-labeled subset containing 4027 preference labels.</li>
      <li>Built CMI-RewardBench to evaluate preference learning methods on compositional multimodal music instructions.</li>
      <li>Trained a parameter-efficient reward model that reaches near-SOTA correlation with human labels across multiple evaluation protocols and supports inference-time scaling for music generation models.</li>
    </ul>
  </div>
</div>

You can also find my articles on [My Google Scholar profile](https://scholar.google.com/citations?user=3AdGPngAAAAJ).

{% include base_path %}

{% for post in site.publications reversed %}
  {% unless post.featured %}
  {% include archive-single.html %}
  {% endunless %}
{% endfor %}
