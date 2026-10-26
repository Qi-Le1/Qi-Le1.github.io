---
permalink: /
title: "About Me"
author_profile: true
excerpt: "Qi Le is a Computer Science Ph.D. student at the University of Minnesota researching efficient and trustworthy language models."
redirect_from:
  - /about/
  - /about.html
---

{% include research-styles.html %}

I am a Ph.D. student in [Computer Science & Engineering](https://cse.umn.edu/cs) at the [University of Minnesota, Twin Cities](https://twin-cities.umn.edu/), advised by Prof. [Ali Anwar](https://chalianwar.github.io/), Prof. [Jie Ding](https://jding.org/), and Dr. [Enmao Diao](https://diaoenmao.com/).

My research focuses on making language models more efficient and trustworthy. I work on **structured pruning, model merging, and KV-cache compression**, with related projects in model adaptation, multi-value alignment, content safety, and federated learning.

I am interested in **AI/ML research internships** focused on efficient language models and their practical deployment.

<p class="research-links">
  <a class="btn btn--primary" href="{{ '/assets/Curriculum_Vitae.pdf' | relative_url }}">Download CV</a>
  <a class="btn" href="{{ '/publications/' | relative_url }}">Publications</a>
  <a class="btn" href="https://github.com/Qi-Le1">GitHub</a>
</p>

## Research Highlights

<div class="research-highlights" markdown="1">

### Probe Pruning: Dynamic LLM Inference

**First author · ICLR 2025**

[Probe Pruning](https://proceedings.iclr.cc/paper_files/paper/2025/hash/b44efaa3b7a389ea56c7ee9d6589e800-Abstract-Conference.html) adapts attention heads and MLP channels to each input batch using lightweight probes and historical activations, without fine-tuning. At 40% pruning on LLaMA-2-7B / WikiText2, it achieved **1.46× attention-block and 1.30× MLP-block inference speedups** on an NVIDIA A100. [Code](https://github.com/Qi-Le1/Probe_Pruning).

### Structured Pruning for Language and Reasoning Models

**Coauthor · ACL 2026 Outstanding Paper · DAC 2026**

I contributed to [GISP](https://aclanthology.org/2026.acl-long.1653/), an iterative, task-aligned global pruning framework. At 50% pruning on LLaMA-2-7B, it achieved **1.70× prefill throughput and 45% lower inference memory** on an NVIDIA A6000 at batch size 1. Our related [RESP](https://arxiv.org/abs/2512.02185) work uses self-generated reasoning traces and progressive calibration to prune reasoning models.

### Alignment and Content Safety

**Coauthor · ICLR 2025 Oral · NAACL 2025**

I contributed to [MAP](https://proceedings.iclr.cc/paper_files/paper/2025/hash/ca549a1547bc8e8ca2df968aeaf57715-Abstract-Conference.html), which aligns language models with user-defined human-value targets, and [AID](https://aclanthology.org/2025.naacl-long.229/), which combines eight safety detectors with input-dependent weights. AID achieved a **0.12 median absolute AUC gain** over the best individual detector across its benchmark detection tasks.

### Federated Learning and Model Adaptation

**First author · IEEE BigData 2024 Best Student Paper**

[DynamicFL](https://ieeexplore.ieee.org/abstract/document/10826074) allocates client communication frequencies under resource budgets. In a matched-schedule CIFAR-10 experiment with a CNN and one class per client, it improved accuracy from **44.4% to 49.8%** over random client selection. I also contributed to [ColA](https://arxiv.org/abs/2404.13844), which offloads adapter-gradient computation for model adaptation. [DynamicFL code](https://github.com/Qi-Le1/DynamicFL).

</div>

## Current Work

My two first-author submissions to **ICLR 2027** study model merging through iterative parameter replacement (**OBMerge**) and KV-cache eviction with output-projected, OBS-inspired compensation (**ProjCache**). Both are submitted manuscripts.

## Selected Recognition

- **Outstanding Paper Award**, ACL 2026 — *From Local to Global*.
- **Machine Learning Systems Fellowship**, Amazon, 2025–2026.
- **Best Student Paper Award**, IEEE BigData 2024 — *DynamicFL*.

See my [publications]({{ '/publications/' | relative_url }}) for the full paper list and [professional service]({{ '/service/' | relative_url }}) for reviewing activities.
