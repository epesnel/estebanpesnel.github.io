---
title: "SCALED: Surrogate-gradient for Codec-Aware Learning of Downsampling in ABR Streaming"
collection: publications
category: conferences
permalink: /publication/scaled
excerpt: 'Surrogate-gradient framework enabling end-to-end optimization with real non-differentiable video codecs for ABR streaming.'
date: 2025-12-08
venue: 'Picture Coding Symposium (PCS) 2025 — Aachen, Germany'
paperurl: 'https://arxiv.org/pdf/2602.00198'
header:
  teaser: /images/scaled_overview.png
---

<style>
.pub-badges { margin: 0.5em 0 1.5em 0; display: flex; flex-wrap: wrap; gap: 0.5em; }
.pub-badge {
  display: inline-flex; align-items: center; gap: 0.3em;
  padding: 0.3em 0.8em; border-radius: 20px;
  font-size: 0.82em; font-weight: 500; text-decoration: none !important;
}
.badge-arxiv   { background: #b31b1b; color: white; }
.badge-arxiv:hover { background: #8b1414; }
.badge-doi     { background: #2c6fad; color: white; }
.badge-doi:hover { background: #1a4f7a; }
.badge-venue   { background: #f0f4f8; color: #333; border: 1px solid #ccc; }
.badge-tag     { background: #e8f4f8; color: #1a5276; border: 1px solid #aed6f1; }

.pub-section {
  margin: 1.8em 0 0.5em 0;
  font-size: 1.05em;
  font-weight: 700;
  color: #2c3e50;
  border-left: 4px solid #4a90d9;
  padding-left: 0.6em;
}
.pub-abstract {
  background: #f8fbff;
  border: 1px solid #d6eaf8;
  border-radius: 6px;
  padding: 1em 1.2em;
  font-size: 0.93em;
  line-height: 1.75;
  color: #333;
}
.contrib-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
  gap: 0.8em;
  margin: 0.8em 0;
}
.contrib-item {
  background: #f9f9f9;
  border-left: 3px solid #4a90d9;
  border-radius: 0 4px 4px 0;
  padding: 0.6em 0.8em;
  font-size: 0.88em;
  line-height: 1.5;
}
.contrib-item strong { display: block; color: #1a3a5c; margin-bottom: 0.2em; }
.result-box {
  display: inline-block;
  background: linear-gradient(135deg, #1a5276, #2c6fad);
  color: white;
  border-radius: 8px;
  padding: 0.8em 1.4em;
  font-size: 1.1em;
  font-weight: 700;
  margin: 0.5em 0.5em 0.5em 0;
  text-align: center;
  min-width: 140px;
}
.result-box span { display: block; font-size: 0.68em; font-weight: 400; opacity: 0.9; margin-top: 0.2em; }
.eq-block {
  background: #f5f5f5;
  border-radius: 6px;
  padding: 0.8em 1.2em;
  margin: 0.8em 0;
  overflow-x: auto;
}
.citation-box {
  position: relative;
  background: #1e2a38;
  color: #abb2bf;
  border-radius: 8px;
  padding: 1.2em 1.4em;
  font-family: 'SFMono-Regular', Consolas, monospace;
  font-size: 0.82em;
  line-height: 1.7;
  overflow-x: auto;
  margin-top: 0.8em;
}
.citation-box .kw  { color: #c678dd; }
.citation-box .val { color: #98c379; }
.citation-box .key { color: #e06c75; }
.citation-box .num { color: #d19a66; }
.copy-btn {
  position: absolute; top: 0.6em; right: 0.8em;
  background: #3a4a5a; color: #abb2bf; border: none;
  border-radius: 4px; padding: 0.25em 0.7em;
  font-size: 0.78em; cursor: pointer;
}
.copy-btn:hover { background: #4a6a8a; color: white; }
</style>

<div class="pub-badges">
  <a class="pub-badge badge-arxiv" href="https://arxiv.org/pdf/2602.00198" target="_blank">📄 arXiv</a>
  <a class="pub-badge badge-doi" href="https://doi.org/10.1109/PCS65673.2025.11417641" target="_blank">🔗 DOI</a>
  <span class="pub-badge badge-venue">📍 PCS 2025 · Aachen · Dec 2025</span>
  <span class="pub-badge badge-tag">Video Compression</span>
  <span class="pub-badge badge-tag">Surrogate Gradients</span>
  <span class="pub-badge badge-tag">ABR Streaming</span>
  <span class="pub-badge badge-tag">Deep Learning</span>
</div>

<div class="pub-section">Abstract</div>

<div class="pub-abstract">
ABR streaming pipelines traditionally optimize downsampling, compression, and reconstruction independently, leading to suboptimal end-to-end rate-distortion performance. Recent deep learning approaches attempted to jointly optimize these stages using differentiable codec proxies, but such approximations often fail to accurately reproduce the behavior of real video codecs. We introduce <strong>SCALED</strong>, a surrogate-gradient framework enabling end-to-end optimization directly with real, non-differentiable codecs (H.264/x264). The method leverages data-driven surrogate gradients derived from actual compression errors while keeping the true codec in the forward pass.
</div>

<div class="pub-section">Key Contributions</div>

<div class="contrib-grid">
  <div class="contrib-item">
    <strong>True-codec training</strong>
    End-to-end optimization with real H.264/VVC codecs — no learned proxy required.
  </div>
  <div class="contrib-item">
    <strong>Surrogate gradient</strong>
    Data-driven Jacobian derived from actual compression noise for stable backpropagation.
  </div>
  <div class="contrib-item">
    <strong>Codec-agnostic</strong>
    Works across different codecs and quality parameters without retraining.
  </div>
  <div class="contrib-item">
    <strong>ABR pipeline</strong>
    Jointly optimizes downscaling, compression, and reconstruction end-to-end.
  </div>
</div>

<div class="pub-section">Method</div>

Standard codecs are non-differentiable — the gradient is zero almost everywhere:

<div class="eq-block">
$$y = \phi(x), \qquad \dfrac{\partial \phi(x)}{\partial x} \approx 0$$
</div>

SCALED replaces the codec in the backward pass with a surrogate forward:

<div class="eq-block">
$$\hat{y} = y + \mathrm{sg}(\epsilon)\,\dfrac{\sigma(\epsilon)}{\mathrm{sg}(\sigma(\epsilon))}, \qquad \epsilon = \phi(y) - y$$
</div>

where $\mathrm{sg}(\cdot)$ denotes the stop-gradient operator. Gradient flow goes exclusively through $\sigma(\epsilon)$, yielding a Jacobian that encodes true compression statistics.

<div class="pub-section">Results</div>

<div>
  <div class="result-box">−6.1% BD-BR<span>vs. codec-agnostic training</span></div>
  <div class="result-box">x264 · VVenC<span>codec-agnostic</span></div>
  <div class="result-box">× 1 / ½ / ¼<span>all scale ratios</span></div>
</div>

<div class="pub-section">Citation</div>

<div class="citation-box" id="citationBox">
<button class="copy-btn" onclick="
  navigator.clipboard.writeText(document.getElementById('citationRaw').innerText);
  this.textContent='Copied!';
  setTimeout(()=>this.textContent='Copy',1500);
">Copy</button>
<pre id="citationRaw" style="margin:0; white-space:pre-wrap;">@INPROCEEDINGS{11417641,
  author    = {Pesnel, Esteban and Le Tanou, Julien and Ropert, Michael
               and Maugey, Thomas and Roumy, Aline},
  booktitle = {2025 Picture Coding Symposium (PCS)},
  title     = {SCALED: Surrogate-gradient for Codec-Aware Learning
               of Downsampling in ABR Streaming},
  year      = {2025},
  pages     = {1--5},
  doi       = {10.1109/PCS65673.2025.11417641}
}</pre>
</div>
