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

A central challenge is that standard codecs are non-differentiable: $$y = \phi(x), \qquad \frac{\partial \phi(x)}{\partial x} \approx 0$$ which prevents direct end-to-end optimization through standard backpropagation.

In our work *SCALED* (*Surrogate-gradient for Codec-Aware Learning of Downsampling in ABR Streaming*), we investigate surrogate-gradient approaches enabling neural networks to optimize directly with real codecs such as H.264/x264. We jointly optimize a learned downsampling function \(f(x;\theta_f)\) with the compression pipeline: $$\hat{x} = g(\phi(f(x;\theta_f)))$$ while approximating the backward pass using codec-aware surrogate gradients derived from real compression errors: $$\hat{y} = y + \mathrm{sg}(\epsilon)\frac{\sigma(\epsilon)}{\mathrm{sg}(\sigma(\epsilon))}$$ where $$\epsilon = \phi(y)-y$$

This approach improves rate-distortion efficiency for ABR streaming pipelines while remaining fully compatible with standard video codecs.


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
