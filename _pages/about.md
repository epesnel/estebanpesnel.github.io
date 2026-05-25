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

A major challenge in neural video optimization is that standard codecs are fundamentally non-differentiable:

$$
y = C(x)
$$

where \(C(\cdot)\) denotes a video codec.

Because quantization, mode decision, and entropy coding break gradient propagation:

$$
\frac{\partial C(x)}{\partial x} \approx 0
$$

standard backpropagation cannot directly optimize codec-aware pipelines.

My work investigates surrogate-gradient approaches enabling neural networks to learn from the *real codec distortion* while maintaining stable optimization.

In our work **SCALED** (*Surrogate-gradient for Codec-Aware Learning of Downsampling in ABR Streaming*), we optimize a neural downsampling module \(f_\theta\) jointly with video compression:

$$
x_d = f_\theta(x)
$$

$$
\hat{x} = C(x_d)
$$

while using differentiable surrogate gradients during backpropagation:

$$
\frac{\partial \mathcal{L}}{\partial x_d}
\approx
\frac{\partial \tilde{C}(x_d)}{\partial x_d}
$$

This allows the optimization process to incorporate the *actual codec realization* instead of relying solely on disconnected differentiable approximations.

The resulting framework improves rate-distortion efficiency for ABR streaming pipelines while remaining fully compatible with standard video codecs.

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
