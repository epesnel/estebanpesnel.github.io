---
title: "SCALED: Surrogate-gradient for Codec-Aware Learning of Downsampling in ABR Streaming"
collection: publications
category: conferences
permalink: /publication/scaled
excerpt: 'Surrogate-gradient framework enabling end-to-end optimization with real non-differentiable video codecs for ABR streaming.'
date: 2026-01-30
venue: 'Picture Coding Symposium (PCS) 2025 - Aachen, Germany'
paperurl: 'https://arxiv.org/pdf/2602.00198'
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

## Citation

```bibtex
@INPROCEEDINGS{11417641,
  author={Pesnel, Esteban and Tanou, Julien Le and Ropert, Michael and Maugey, Thomas and Roumy, Aline},
  booktitle={2025 Picture Coding Symposium (PCS)}, 
  title={SCALED: Surrogate-gradient for Codec-Aware Learning of Downsampling in ABR Streaming}, 
  year={2025},
  volume={},
  number={},
  pages={1-5},
  keywords={Training;Codecs;Quantization (signal);Pipelines;Bit rate;Rate-distortion;Encoding;Video codecs;Standards;Videos},
  doi={10.1109/PCS65673.2025.11417641}
}
```

![SCALED overview](/images/scaled_overview.png)
