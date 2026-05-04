---
title: "CMI-RewardBench: Evaluating Music Reward Models with Compositional Multimodal Instruction"
collection: publications
permalink: /publication/cmi-rewardbench
date: 2026-03-01
venue: 'ICML 2026'
paperurl: 'https://arxiv.org/abs/2603.00610'
excerpt: 'Accepted by ICML 2026. We evaluate music reward models with compositional multimodal instruction and introduce CMI-Pref and CMI-RewardBench.'
---
The paper **CMI-RewardBench: Evaluating Music Reward Models with Compositional Multimodal Instruction** has been accepted by **ICML 2026**.

![1777908995485](/image/publications/CMI-Rewardbench.png)

**Authors**: Yinghao Ma, Haiwen Xia, Hewei Gao, Weixiong Chen, Yuxin Ye, Yuchen Yang, Sungkyun Chang, Mingshuo Ding, Yizhi Li, Ruibin Yuan, Simon Dixon, Emmanouil Benetos

[Paper link (arXiv)](https://arxiv.org/abs/2603.00610)

- Introduced a new task for evaluating generated audio from compositional music instructions.
- Created CMI-Pref using 23 music generation models, with an LLM-labeled dataset of 110k preferences and 797 hours of generated audio, plus a human-labeled subset with 4027 preference labels.
- Built CMI-RewardBench by integrating prior works to further evaluate preference learning.
- Trained a parameter-efficient reward model that achieves near-SOTA correlation with human labels across multiple evaluation protocols, demonstrating the effectiveness of CMI-Pref and enabling inference-time scaling for music generation models.
