---
title: "SCALED: Surrogate-gradient for Codec-Aware Learning of Downsampling in ABR Streaming"
collection: publications
category: conference
permalink: /publication/scaled
excerpt: 'Surrogate-gradient framework enabling end-to-end optimization with real non-differentiable video codecs for ABR streaming.'
date: 2026-01-30
venue: 'Picture Coding Symposium (PCS) 2025 - Aachen, Germany'
paperurl: 'https://arxiv.org/pdf/2602.00198'
citation: 'Esteban Pesnel, Julien Le Tanou, Michael Ropert, Thomas Maugey, and Aline Roumy. (2026). "SCALED: Surrogate-gradient for Codec-Aware Learning of Downsampling in ABR Streaming." <i>arXiv preprint arXiv:2602.00198</i>.'
---
Adaptive Bitrate (ABR) streaming pipelines traditionally optimize downsampling, compression, and reconstruction independently, leading to suboptimal end-to-end rate-distortion performance. Recent deep learning approaches attempted to jointly optimize these stages using differentiable codec proxies, but such approximations often fail to accurately reproduce the behavior of real video codecs.

In this work, we introduce **SCALED**, a surrogate-gradient framework enabling end-to-end optimization directly with real non-differentiable codecs such as H.264/x264. The proposed method leverages data-driven surrogate gradients derived from actual compression errors while keeping the true codec in the forward pass.

A central challenge is that standard codecs are fundamentally non-differentiable:

$$
y = \phi(x), \qquad \frac{\partial \phi(x)}{\partial x} \approx 0
$$

To address this issue, SCALED introduces a modified surrogate-gradient formulation:

$$
\hat{y} = y + \mathrm{sg}(\epsilon)\frac{\sigma(\epsilon)}{\mathrm{sg}(\sigma(\epsilon))}
$$

where:

$$
\epsilon = \phi(y)-y
$$

This formulation enables stable gradient propagation while preserving the true codec behavior during optimization.

Experimental results on ABR streaming pipelines demonstrate significant rate-distortion improvements over codec-agnostic and proxy-based training approaches, achieving up to **6.1% BD-BR reduction** while remaining fully compatible with standard deployment pipelines.
