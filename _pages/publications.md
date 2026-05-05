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

{% for post in site.publications reversed %}
  {% if post.featured %}
    {% include featured-publication.html post=post %}
  {% endif %}
{% endfor %}

You can also find my articles on [My Google Scholar profile](https://scholar.google.com/citations?user=3AdGPngAAAAJ).

{% include base_path %}

{% for post in site.publications reversed %}
  {% unless post.featured %}
  {% include archive-single.html %}
  {% endunless %}
{% endfor %}
