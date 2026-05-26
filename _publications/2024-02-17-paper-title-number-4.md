---
layout: single
collection: publications
category: conferences
permalink: /publication/scaled
title: "SCALED: Surrogate-gradient for Codec-Aware Learning of Downsampling in ABR Streaming"
excerpt: 'End-to-end training with real non-differentiable video codecs via surrogate gradients.'
date: 2025-12-08
venue: 'Picture Coding Symposium (PCS) 2025'
paperurl: 'https://arxiv.org/pdf/2602.00198'
author_profile: false
---

<script>
MathJax = {
  tex: {
    inlineMath: [['$', '$'], ['\\(', '\\)']],
    displayMath: [['$$', '$$'], ['\\[', '\\]']],
    processEscapes: true
  }
};
</script>

<style>
/* Hide template auto-generated header */
.page__title, .page__meta, .page__share, .page__footer-follow { display: none !important; }

/* ── Base ── */
.sp { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', sans-serif; color: var(--text); }

/* ── Hero banner ── */
.sp-hero {
  background: linear-gradient(135deg, var(--card-bg) 0%, rgba(41,151,255,0.12) 50%, rgba(255,140,66,0.08) 100%);
  border: 1px solid var(--card-border);
  -webkit-backdrop-filter: saturate(180%) blur(20px);
  backdrop-filter: saturate(180%) blur(20px);
  border-radius: 12px; padding: 2em 2.2em 1.8em;
  margin-bottom: 2em; color: var(--text); position: relative; overflow: hidden;
}
.sp-hero-logos {
  position: absolute; top: 1.2em; right: 1.5em;
  display: flex; align-items: center; gap: 1em;
  opacity: 0.5; z-index: 1;
}
.sp-hero-logos img {
  height: 20px; width: auto; object-fit: contain;
  opacity: 0.5;
}
.sp-hero-logos img[alt="MediaKind"] {
  filter: brightness(0) invert(1);
}
.sp-hero::before {
  content: ''; position: absolute; top: -40px; right: -40px;
  width: 200px; height: 200px; border-radius: 50%;
  background: rgba(41,151,255,0.06);
}
.sp-hero::after {
  content: ''; position: absolute; bottom: -60px; left: 30%;
  width: 300px; height: 300px; border-radius: 50%;
  background: rgba(255,140,66,0.04);
}
.sp-hero-venue {
  display: inline-flex; align-items: center; gap: 0.4em;
  background: var(--accent-subtle); border: 1px solid var(--pill-border);
  border-radius: 20px; padding: 0.25em 0.9em;
  font-size: 0.8em; font-weight: 500; margin-bottom: 1em; color: var(--accent);
}
.sp-hero-title {
  font-size: 1.5em; font-weight: 800; line-height: 1.3;
  margin: 0 0 0.8em 0; max-width: 700px; color: var(--heading);
}
.sp-hero-title em { color: var(--accent); font-style: normal; }
.sp-authors {
  font-size: 0.88em; margin-bottom: 0.5em; opacity: 0.9; line-height: 1.8; color: var(--text);
}
.sp-authors .me { font-weight: 700; color: var(--accent); }
.sp-affiliations {
  font-size: 0.75em; opacity: 0.65; margin-bottom: 1.4em; line-height: 1.7; color: var(--text-secondary);
}
.sp-buttons { display: flex; flex-wrap: wrap; gap: 0.5em; }
.sp-btn {
  display: inline-flex; align-items: center; gap: 0.35em;
  padding: 0.45em 1.1em; border-radius: 6px;
  font-size: 0.82em; font-weight: 600;
  text-decoration: none !important; cursor: pointer; border: none;
  transition: transform 0.15s, box-shadow 0.15s;
}
.sp-btn:hover { transform: translateY(-1px); box-shadow: 0 4px 12px rgba(0,0,0,0.25); }
.sp-btn-primary { background: rgba(41,151,255,0.2); color: var(--accent); border: 1px solid var(--pill-border); }
.sp-btn-secondary { background: var(--accent-subtle); color: var(--accent); border: 1px solid var(--pill-border); }
.sp-btn-secondary:hover { background: var(--accent); color: white; }

/* ── Tags ── */
.sp-tags { margin: 0 0 0.8em 0; }
.sp-tag {
  display: inline-block; padding: 0.2em 0.7em; border-radius: 20px;
  font-size: 0.76em; font-weight: 500; margin: 2px;
  background: var(--accent-warm-subtle); color: var(--accent-warm);
  border: 1px solid rgba(255,140,66,0.15);
}

/* ── Sections ── */
.sp-section { margin: 2em 0 0.6em; }
.sp-section-title {
  font-size: 1.05em; font-weight: 700; color: var(--heading);
  border-left: 4px solid var(--blue); padding-left: 0.65em;
  margin: 0 0 0.8em 0;
}
.sp-abstract {
  background: var(--card-bg); border: 1px solid var(--card-border);
  border-radius: 8px; padding: 1.1em 1.3em;
  font-size: 0.92em; line-height: 1.8; color: var(--text);
}

/* ── Contribution grid ── */
.sp-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(200px,1fr)); gap: 0.8em; }
.sp-card {
  background: var(--card-bg); border: 1px solid var(--card-border);
  border-radius: 8px; padding: 0.9em 1em;
  font-size: 0.87em; line-height: 1.55; color: var(--text);
  border-top: 3px solid var(--blue);
}
.sp-card strong { display: block; color: var(--heading); margin-bottom: 0.3em; font-size: 0.95em; }

/* ── Equation blocks ── */
.sp-eq {
  background: var(--eq-bg); border-left: 3px solid var(--separator);
  border-radius: 0 6px 6px 0; padding: 0.8em 1.2em;
  margin: 0.8em 0; overflow-x: auto;
}
.sp-eq-label { font-size: 0.75em; color: var(--text-muted); text-align: right; margin-top: 0.3em; }

/* ── Result cards ── */
.sp-results { display: flex; flex-wrap: wrap; gap: 0.8em; margin: 0.8em 0 1.4em; }
.sp-result {
  border-radius: 10px; padding: 1em 1.4em; text-align: center;
  min-width: 120px; flex: 1;
}
.sp-result-a { background: linear-gradient(135deg,#1a365d,#2b6cb0); color:white; }
.sp-result-b { background: linear-gradient(135deg,#1c4532,#276749); color:white; }
.sp-result-c { background: linear-gradient(135deg,#44337a,#6b46c1); color:white; }
.sp-result-d { background: linear-gradient(135deg,#7b341e,#c05621); color:white; }
.sp-result .val { font-size: 1.5em; font-weight: 800; }
.sp-result .lbl { font-size: 0.7em; opacity: 0.88; margin-top: 0.3em; line-height: 1.4; }

/* ── Table ── */
.sp-table-wrap { overflow-x: auto; margin: 1em 0; }
.sp-table { width: 100%; border-collapse: collapse; font-size: 0.84em; color: var(--text); }
.sp-table thead tr { background: #1b3a5c; color: white; }
.sp-table th { padding: 0.6em 0.8em; text-align: center; font-weight: 600; white-space: nowrap; }
.sp-table td { padding: 0.45em 0.8em; text-align: center; border-bottom: 1px solid var(--card-border); }
.sp-table tbody tr:hover { background: var(--blue-pale); }
.sp-table .ours { background: var(--card-bg); font-weight: 600; }
.sp-table .ours td:first-child { border-left: 3px solid #27ae60; }
.sp-table .good { color: #48bb78; font-weight: 600; }
.sp-table .bad  { color: #fc8181; font-weight: 600; }
.sp-table .group-header td {
  background: var(--blue-pale); color: var(--text-muted); font-size: 0.8em;
  font-weight: 700; text-align: left; padding: 0.3em 0.8em;
  letter-spacing: 0.05em; text-transform: uppercase;
}

/* ── Citation ── */
.sp-citation {
  position: relative; background: #1a202c; color: #a0aec0;
  border-radius: 10px; padding: 1.3em 1.5em 1em;
  font-family: 'SFMono-Regular', Consolas, monospace;
  font-size: 0.81em; line-height: 1.75; overflow-x: auto; margin-top: 0.8em;
}
.sp-copy {
  position: absolute; top: 0.7em; right: 0.8em;
  background: #2d3748; color: #a0aec0; border: none;
  border-radius: 5px; padding: 0.25em 0.8em;
  font-size: 0.78em; cursor: pointer;
}
.sp-copy:hover { background: #4a5568; color: #fff; }
pre.sp-bib { margin: 0; white-space: pre-wrap; color: #a0aec0; }
.bib-key  { color: #fc8181; }
.bib-val  { color: #68d391; }
.bib-type { color: #b794f4; font-weight: 700; }
.bib-field { color: #63b3ed; }
</style>

<div class="sp">

<!-- ════════════ HERO ════════════ -->
<div class="sp-hero">
  <div class="sp-hero-logos">
    <img src="/images/logos/inria_white.png" alt="INRIA" />
    <img src="/images/logos/mediakind.svg" alt="MediaKind" />
  </div>
  <div class="sp-hero-venue">📍 PCS 2025 &nbsp;·&nbsp; Aachen, Germany &nbsp;·&nbsp; December 2025</div>
  <div class="sp-hero-title">
    <em>SCALED</em>: Surrogate-gradient for Codec-Aware<br/>Learning of Downsampling in ABR Streaming
  </div>
  <div class="sp-authors">
    <span class="me">Esteban Pesnel</span><sup>*†</sup>,
    Julien Le Tanou<sup>*</sup>,
    Michael Ropert<sup>*</sup>,
    Thomas Maugey<sup>†</sup>,
    Aline Roumy<sup>†</sup>
  </div>
  <div class="sp-affiliations">
    <sup>*</sup>MediaKind, Rennes, France &nbsp;&nbsp;
    <sup>†</sup>INRIA, Rennes, France — team COMPACT
  </div>
  <div class="sp-tags">
    <span class="sp-tag">Video Compression</span>
    <span class="sp-tag">Surrogate Gradients</span>
    <span class="sp-tag">ABR Streaming</span>
    <span class="sp-tag">Deep Learning</span>
    <span class="sp-tag">H.264 / x264</span>
    <span class="sp-tag">Rate-Distortion</span>
  </div>
  <div class="sp-buttons">
    <a class="sp-btn sp-btn-primary" href="https://arxiv.org/pdf/2602.00198" target="_blank">📄 PDF (arXiv)</a>
    <a class="sp-btn sp-btn-secondary" href="https://arxiv.org/abs/2602.00198" target="_blank">🔗 arXiv:2602.00198</a>
    <a class="sp-btn sp-btn-secondary" href="https://doi.org/10.1109/PCS65673.2025.11417641" target="_blank">🏛 DOI</a>
  </div>
</div>

<!-- ════════════ ABSTRACT ════════════ -->
<div class="sp-section">
<div class="sp-section-title">Abstract</div>
<div class="sp-abstract">
The rapid growth in video consumption has introduced significant challenges to modern streaming architectures. OTT video delivery now predominantly relies on Adaptive Bitrate (ABR) streaming, which dynamically adjusts bitrate and resolution based on client-side constraints such as display capabilities and network bandwidth. This pipeline typically involves downsampling the original high-resolution content, encoding and transmitting it, followed by decoding and upsampling on the client side. Traditionally, these processing stages have been optimized in isolation, leading to suboptimal end-to-end rate-distortion (R-D) performance. The advent of deep learning has spurred interest in jointly optimizing the ABR pipeline using learned resampling methods. However, training such systems end-to-end remains challenging due to the non-differentiable nature of standard video codecs, which obstructs gradient-based optimization. Recent works have addressed this issue using differentiable proxy models, based either on deep neural networks or hybrid coding schemes with differentiable components such as soft quantization, to approximate the codec behavior. While differentiable proxy codecs have enabled progress in compression-aware learning, they remain approximations that may not fully capture the behavior of standard, non-differentiable codecs. In this work, we introduce a novel framework that enables end-to-end training with real, non-differentiable codecs by leveraging data-driven surrogate gradients derived from actual compression errors. It facilitates the alignment between training objectives and deployment performance. Experimental results show a <strong>5.19% improvement in BD-BR (PSNR)</strong> compared to codec-agnostic training approaches, consistently across the entire rate-distortion convex hull spanning multiple downsampling ratios.
</div>
</div>

<!-- ════════════ OVERVIEW ════════════ -->
<div class="sp-section">
<div class="sp-section-title">Overview</div>
<p>In ABR streaming, high-resolution video is downscaled server-side, encoded with a standard codec (e.g. H.264), transmitted, decoded, and upscaled client-side — typically with a fixed bicubic filter. SCALED optimizes the <strong>learned downscaler</strong> \(f\) so that the full chain — downscale → encode → decode → bicubic upscale — produces the best possible reconstruction at a given bitrate. The key difficulty is that the codec \(\phi\) is non-differentiable: gradients cannot flow through it during training. SCALED solves this by injecting <strong>surrogate gradients</strong> derived from the actual compression error statistics, enabling true end-to-end optimization without any proxy codec.</p>

<img src="/images/scaled_overview.png" alt="SCALED pipeline overview" style="width:100%; border-radius: 20px; margin: 1.2em 0; border: 1px solid var(--card-border);" />
</div>

<!-- ════════════ CONTRIBUTIONS ════════════ -->
<div class="sp-section">
<div class="sp-section-title">Contributions</div>
<div class="sp-grid">
  <div class="sp-card">
    <strong>🎯 True-codec training</strong>
    Real H.264/x264 in the forward pass. No learned or handcrafted proxy required.
  </div>
  <div class="sp-card">
    <strong>∂ Surrogate Jacobian</strong>
    Reparameterization of the codec gradient via the std. deviation of true compression noise.
  </div>
  <div class="sp-card">
    <strong>⚡ Two training variants</strong>
    SCALED<sub>D</sub> (distortion only) and SCALED<sub>RD</sub> (rate-distortion with differentiable rate proxy).
  </div>
</div>
</div>

<!-- ════════════ METHOD ════════════ -->
<div class="sp-section">
<div class="sp-section-title">Method</div>

<p>The core challenge: applying Straight-Through Estimation (STE) to codecs causes divergence - the compression error fully disconnects from gradient flow, leading to \(|\,f(x;\theta_f)\,|_1 \to \infty\). SCALED reparameterizes the codec output as:</p>

<div class="sp-eq">
$$\hat{y} = y + \mathrm{sg}(\epsilon)\,\frac{\sigma(\epsilon)}{\mathrm{sg}(\sigma(\epsilon))}, \qquad \epsilon = \phi(y) - y$$
<div class="sp-eq-label">Eq. (7) — SCALED forward pass</div>
</div>

<p>Gradient flows exclusively through \(\sigma(\epsilon)\), yielding a dynamically scaled surrogate Jacobian that encodes true codec statistics:</p>

<div class="sp-eq">
$$\frac{\partial \hat{y}}{\partial y}\bigg|_{\text{surrogate}} = \mathbf{I} - \frac{\boldsymbol{\epsilon}\,(\boldsymbol{\epsilon} - \bar{\boldsymbol{\epsilon}})^T}{N\,\sigma^2(\boldsymbol{\epsilon})}$$
<div class="sp-eq-label">Eq. (8) — Surrogate Jacobian</div>
</div>

<p>Unlike STE or proxy-based methods, the gradient adapts dynamically to the current compression error distribution.</p>
</div>

<!-- ════════════ RESULTS ════════════ -->
<div class="sp-section">
<div class="sp-section-title">Results</div>

<div class="sp-results">
  <div class="sp-result sp-result-a">
    <div class="val">−6.11%</div>
    <div class="lbl">BD-BR PSNR · XIPH<br/>SCALED<sub>RD</sub> vs Lanczos</div>
  </div>
  <div class="sp-result sp-result-b">
    <div class="val">−5.07%</div>
    <div class="lbl">BD-BR PSNR · UVG<br/>SCALED<sub>RD</sub> vs Lanczos</div>
  </div>
  <div class="sp-result sp-result-c">
    <div class="val">+5.19%</div>
    <div class="lbl">BD-BR gain<br/>vs codec-agnostic</div>
  </div>
  <div class="sp-result sp-result-d">
    <div class="val">×6</div>
    <div class="lbl">scale ratios<br/>2/3 → 1/5</div>
  </div>
</div>

<div class="sp-table-wrap">
<table class="sp-table">
<thead>
<tr>
  <th>Method</th><th>Strategy</th><th>Codec-aware</th>
  <th>PSNR</th><th>SSIM</th><th>VMAF</th><th>VMAF-NEG</th>
</tr>
</thead>
<tbody>
<tr class="group-header"><td colspan="7">XIPH dataset — BD-BR vs Lanczos (↓ is better)</td></tr>
<tr>
  <td>ProgDownLite<sub>YUV</sub></td><td>D-only, no codec</td><td>✗</td>
  <td>-0.85%</td><td>-1.19%</td><td>-4.71%</td><td>-3.60%</td>
</tr>
<tr>
  <td>ProgDownLite<sub>YUV</sub></td><td>STE</td><td>✓</td>
  <td class="bad">+68.57%</td><td class="bad">+48.34%</td><td class="bad">+11.22%</td><td class="bad">+20.69%</td>
</tr>
<tr>
  <td>ProgDownLite<sub>YUV</sub></td><td>Proxy [Guleryuz et al.]</td><td>✓</td>
  <td>-1.47%</td><td>-1.87%</td><td>-2.58%</td><td>-1.67%</td>
</tr>
<tr class="ours">
  <td><strong>SCALED<sub>D</sub></strong></td><td>D + true codec</td><td>✓</td>
  <td class="good">-4.67%</td><td class="good">-5.21%</td><td class="good">-9.80%</td><td class="good">-7.78%</td>
</tr>
<tr class="ours">
  <td><strong>SCALED<sub>RD</sub></strong></td><td>R-D + true codec</td><td>✓</td>
  <td class="good">-6.11%</td><td class="good">-4.29%</td><td class="good">-8.80%</td><td class="good">-7.59%</td>
</tr>
</tbody>
</table>
</div>
</div>

<!-- ════════════ CITATION ════════════ -->
<div class="sp-section">
<div class="sp-section-title">Citation</div>
<div class="sp-citation">
<button class="sp-copy" onclick="
  navigator.clipboard.writeText(document.getElementById('bibRaw').innerText);
  this.textContent='✓ Copied'; setTimeout(()=>this.textContent='Copy',1800);
">Copy</button>
<pre class="sp-bib" id="bibRaw"><span class="bib-type">@INPROCEEDINGS</span>{<span class="bib-key">11417641</span>,
  <span class="bib-field">author</span>    = {<span class="bib-val">Pesnel, Esteban and Le Tanou, Julien and Ropert, Michael
               and Maugey, Thomas and Roumy, Aline</span>},
  <span class="bib-field">booktitle</span> = {<span class="bib-val">2025 Picture Coding Symposium (PCS)</span>},
  <span class="bib-field">title</span>     = {<span class="bib-val">SCALED: Surrogate-gradient for Codec-Aware Learning
               of Downsampling in ABR Streaming</span>},
  <span class="bib-field">year</span>      = {<span class="bib-val">2025</span>},
  <span class="bib-field">pages</span>     = {<span class="bib-val">1--5</span>},
  <span class="bib-field">doi</span>       = {<span class="bib-val">10.1109/PCS65673.2025.11417641</span>}
}</pre>
</div>
</div>

</div><!-- end .sp -->
