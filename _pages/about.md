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
.home-hero {
  background: linear-gradient(135deg, #0d1b2a 0%, #1b3a5c 60%, #2c6fad 100%);
  border-radius: 12px; padding: 2em 2.2em 1.8em;
  color: white; margin-bottom: 2em; position: relative; overflow: hidden;
}
.home-hero::after {
  content: ''; position: absolute; bottom: -80px; right: -60px;
  width: 280px; height: 280px; border-radius: 50%;
  background: rgba(255,255,255,0.04); pointer-events: none;
}
.home-hero-name {
  font-size: 1.8em; font-weight: 800; margin: 0 0 0.2em; line-height: 1.2;
}
.home-hero-sub {
  font-size: 0.95em; opacity: 0.8; margin-bottom: 1.2em; line-height: 1.6;
}
.home-hero-sub em { color: #63b3ed; font-style: normal; font-weight: 600; }
.home-badge-row { display: flex; flex-wrap: wrap; gap: 0.5em; margin-bottom: 1.4em; }
.home-badge {
  display: inline-flex; align-items: center; gap: 0.3em;
  background: rgba(255,255,255,0.12); border: 1px solid rgba(255,255,255,0.2);
  border-radius: 20px; padding: 0.25em 0.85em;
  font-size: 0.78em; color: rgba(255,255,255,0.9);
}
.home-links-row { display: flex; flex-wrap: wrap; gap: 0.5em; }
.home-link {
  display: inline-flex; align-items: center; gap: 0.35em;
  padding: 0.4em 1em; border-radius: 6px; font-size: 0.82em; font-weight: 600;
  text-decoration: none !important; transition: transform 0.15s;
}
.home-link:hover { transform: translateY(-1px); }
.hl-scholar  { background: #4285f4; color: white; }
.hl-orcid    { background: #a6ce39; color: #333; }
.hl-linkedin { background: #0077b5; color: white; }
.hl-rg       { background: #00ccbb; color: white; }
.hl-github   { background: #24292e; color: white; }

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

<!-- ══════════════ HERO ══════════════ -->
<div class="home-hero">
  <div class="home-hero-name">Esteban Pesnel</div>
  <div class="home-hero-sub">
    CIFRE PhD candidate &nbsp;·&nbsp; <em>INRIA</em> &amp; <em>MediaKind</em> &nbsp;·&nbsp; team CompACT, Rennes<br/>
    AI-driven video compression &amp; neural video processing
  </div>
  <div class="home-badge-row">
    <span class="home-badge">🎓 INSA Rennes</span>
    <span class="home-badge">✈️ ÉTS Montréal</span>
    <span class="home-badge">📍 Rennes, France</span>
    <span class="home-badge">🎯 PhD 2023–2026</span>
  </div>
  <div class="home-links-row">
    <a class="home-link hl-scholar"  href="https://scholar.google.com/citations?view_op=list_works&hl=fr&user=Jy7NZNwAAAAJ" target="_blank">🎓 Scholar</a>
    <a class="home-link hl-orcid"   href="https://orcid.org/0009-0004-5906-0152" target="_blank">🔬 ORCID</a>
    <a class="home-link hl-linkedin" href="https://www.linkedin.com/in/estebanpesnel" target="_blank">💼 LinkedIn</a>
    <a class="home-link hl-rg"      href="https://www.researchgate.net/profile/Esteban-Pesnel" target="_blank">📊 ResearchGate</a>
    <a class="home-link hl-github"  href="https://github.com/epesnel" target="_blank">💻 GitHub</a>
  </div>
</div>

<!-- ══════════════ ABOUT ══════════════ -->
<div class="hs">About</div>

I am a CIFRE PhD candidate at <strong>INRIA</strong> and <strong>MediaKind</strong> within the CompACT team in Rennes, working on AI-driven video compression and neural video processing. I hold an engineering degree from <strong>INSA Rennes</strong> and studied aerospace engineering at <strong>ÉTS Montréal</strong> (Canada).

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
