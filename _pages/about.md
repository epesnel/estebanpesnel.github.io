---
permalink: /
title: "Esteban Pesnel"
author_profile: true
mathjax: true
redirect_from: 
  - /about/
  - /about.html
---

I am a CIFRE PhD candidate at INRIA and MediaKind within the CompACT team in Rennes, working on AI-driven video compression and neural video processing.

My research focuses on differentiable optimization for modern video pipelines, including:
- learned image/video compression,
- codec-aware neural optimization,
- perceptual quality optimization,
- adaptive bitrate (ABR) streaming,
- neural wrappers around standard codecs.

I hold an engineering degree from INSA Rennes and also studied aerospace engineering at ÉTS Montréal (École de technologie supérieure, Canada).

## Research Overview

A major challenge in neural video optimization is that standard codecs are non-differentiable: $$ y = C(x) $$ where \(C(\cdot)\) denotes a video codec. Quantization, mode decision, and entropy coding severely disrupt gradient propagation: $$ \frac{\partial C(x)}{\partial x} \approx 0 $$ making standard backpropagation ineffective for codec-aware optimization.

My research investigates surrogate-gradient approaches enabling neural networks to optimize against the *real codec distortion* while maintaining stable training dynamics.

In **SCALED** (*Surrogate-gradient for Codec-Aware Learning of Downsampling in ABR Streaming*), we jointly optimize a neural downsampling module \(f_\theta\) with video compression: $$ x_d = f_\theta(x), \qquad \hat{x} = C(x_d) $$ while approximating codec gradients during backpropagation using differentiable surrogate models: $$ \frac{\partial \mathcal{L}}{\partial x_d} \approx \frac{\partial \tilde{C}(x_d)}{\partial x_d} $$ This framework enables codec-aware optimization using the actual codec realization rather than disconnected differentiable proxies, improving rate-distortion performance for ABR streaming pipelines while remaining compatible with standard codecs.

## Research Interests

- Video compression
- Learned compression
- Differentiable codec modeling
- Neural video processing
- Perceptual optimization
- Adaptive bitrate streaming
- Deep learning for media systems

## Recent Activities

- Presentation at PCS 2025 (Aachen, Germany 🇩🇪) on codec-aware learning for ABR streaming ! -> [PDF](https://arxiv.org/pdf/2602.00198)

## Links

- [Google Scholar](https://scholar.google.com/citations?view_op=list_works&hl=fr&user=Jy7NZNwAAAAJ)
- [ORCID](https://orcid.org/0009-0004-5906-0152)
- [LinkedIn](https://www.linkedin.com/in/estebanpesnel)
- [ResearchGate](https://www.researchgate.net/profile/Esteban-Pesnel)
- [GitHub](https://github.com/epesnel)
