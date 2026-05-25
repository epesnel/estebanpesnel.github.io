---
permalink: /
title: "Esteban Pesnel"
author_profile: true
mathjax: true
redirect_from:
  - /about/
  - /about.html
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
.intro-card {
  background: #f0f6ff;
  border: 1px solid #c3daf7;
  border-left: 4px solid #2c6fad;
  border-radius: 0 10px 10px 0;
  padding: 1.1em 1.4em;
  margin-bottom: 1.8em;
  font-size: 0.93em;
  line-height: 1.75;
  color: #2d3748;
}
.intro-card p { margin: 0.5em 0 0; }
.intro-thesis {
  font-size: 0.9em; color: #1b3a5c; margin-bottom: 0.3em;
}

/* Research topics */
.topic-grid {
  display: grid; grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
  gap: 0.6em; margin: 0.8em 0 1.6em;
}
.topic-item {
  background: #f0f6ff; border: 1px solid #bee3f8;
  border-radius: 8px; padding: 0.6em 0.8em;
  font-size: 0.84em; color: #1b3a5c; line-height: 1.4;
  display: flex; align-items: center; gap: 0.4em;
}

/* Section headers */
.hs { font-size: 1.05em; font-weight: 700; color: #1b3a5c;
  border-left: 4px solid #2c6fad; padding-left: 0.65em;
  margin: 1.8em 0 0.8em; }

/* Research overview card */
.research-card {
  background: #f8fbff; border: 1px solid #c3daf7;
  border-radius: 10px; padding: 1.3em 1.5em; margin-bottom: 1.5em;
}
.research-card p { font-size: 0.93em; line-height: 1.8; color: #2d3748; margin: 0 0 0.8em; }
.research-card p:last-child { margin-bottom: 0; }
.eq-block {
  background: #f0f4f8; border-left: 3px solid #90cdf4;
  border-radius: 0 6px 6px 0; padding: 0.7em 1.1em;
  margin: 0.8em 0; overflow-x: auto; text-align: center;
}

/* News / activity card */
.news-card {
  border: 1px solid #e2e8f0; border-radius: 10px;
  overflow: hidden; margin-bottom: 1em;
}
.news-card-header {
  background: #1b3a5c; color: white;
  padding: 0.5em 1.1em; font-size: 0.82em; font-weight: 600;
  display: flex; align-items: center; gap: 0.5em;
}
.news-card-body {
  padding: 0.9em 1.1em; font-size: 0.9em; line-height: 1.65; color: #2d3748;
}
.news-card-body a { color: #2c6fad; font-weight: 600; }
.news-pill {
  display: inline-block; background: #ebf4ff; color: #2b6cb0;
  border-radius: 20px; padding: 0.1em 0.6em; font-size: 0.78em;
  border: 1px solid #bee3f8; margin-left: 0.3em; vertical-align: middle;
}
</style>

<!-- ══════════════ INTRO ══════════════ -->
<div class="intro-card">
  <div class="intro-thesis">
    🎯 <strong>PhD thesis</strong> — <em>"Learned video downscaling for end-to-end Rate-Distortion optimization of video streaming systems"</em>
  </div>
  <p>CIFRE PhD candidate at <strong>INRIA</strong> &amp; <strong>MediaKind</strong> (team CompACT, Rennes),
  working on AI-driven video compression and neural video processing.
  Engineering degree from <strong>INSA Rennes</strong> · exchange semester in aerospace engineering at <strong>ÉTS Montréal</strong>.</p>
</div>

<!-- ══════════════ RESEARCH TOPICS ══════════════ -->
<div class="hs">Research Focus</div>

<div class="topic-grid">
  <div class="topic-item">🎬 Learned video compression</div>
  <div class="topic-item">🔁 Codec-aware neural optimization</div>
  <div class="topic-item">👁 Perceptual quality optimization</div>
  <div class="topic-item">📡 ABR streaming</div>
  <div class="topic-item">🧠 Neural codec wrappers</div>
  <div class="topic-item">∂ Differentiable codec modeling</div>
  <div class="topic-item">📊 Rate-distortion optimization</div>
  <div class="topic-item">🖥 Deep learning for media</div>
</div>

<!-- ══════════════ RESEARCH OVERVIEW ══════════════ -->
<div class="hs">Research Overview</div>

<div class="research-card">
<p>A central challenge in neural video optimization is that standard codecs are fundamentally non-differentiable:</p>

<div class="eq-block">
$$y = \phi(x), \qquad \frac{\partial \phi(x)}{\partial x} \approx 0$$
</div>

<p>This prevents direct end-to-end gradient-based optimization through the codec. In our work <strong>SCALED</strong> (<em>Surrogate-gradient for Codec-Aware Learning of Downsampling in ABR Streaming</em>), we introduce surrogate-gradient approaches enabling neural networks to optimize directly with real codecs such as H.264/x264. We jointly optimize a learned downsampling function \(f(x;\theta_f)\) within the full compression pipeline:</p>

<div class="eq-block">
$$\hat{x} = g\!\left(\phi(f(x;\,\theta_f))\right)$$
</div>

<p>while leveraging surrogate gradients derived from real compression errors during backpropagation — achieving <strong>5.19% BD-BR (PSNR) improvement</strong> over codec-agnostic training approaches.</p>
</div>

<!-- ══════════════ NEWS ══════════════ -->
<div class="hs">Recent Activities</div>

<div class="news-card">
  <div class="news-card-header">
    🇩🇪 &nbsp;December 2025 &nbsp;·&nbsp; PCS 2025, Aachen, Germany
  </div>
  <div class="news-card-body">
    Presented <strong>SCALED</strong> at the Picture Coding Symposium 2025.
    <span class="news-pill">Conference paper</span>
    <span class="news-pill">Poster</span>
    <br/><br/>
    <a href="https://arxiv.org/pdf/2602.00198" target="_blank">📄 PDF (arXiv)</a>
    &nbsp;&nbsp;
    <a href="/publication/scaled">🔍 Paper details</a>
    &nbsp;&nbsp;
    <a href="/talks/">🖼 Poster</a>
  </div>
</div>
