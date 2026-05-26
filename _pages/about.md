---
permalink: /
title: "Esteban Pesnel"
author_profile: true
layout: single
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
/* ── Sidebar panel ── */
.sidebar.sticky {
  height: fit-content !important; align-self: flex-start !important;
  background: linear-gradient(160deg, #0d1b2a 0%, #1b3a5c 55%, #2c6fad 100%) !important;
  border-radius: 16px !important; padding: 1.8em 1.2em 1.6em !important;
  position: relative !important; box-shadow: 0 8px 32px rgba(0,0,0,0.22) !important;
  margin-top: 0.8em !important;
}
.sidebar.sticky::before {
  content:''!important; position:absolute!important; top:-50px!important; right:-40px!important;
  width:180px!important; height:180px!important; border-radius:50%!important;
  background:rgba(255,255,255,0.06)!important; pointer-events:none!important; z-index:0!important;
}
.sidebar.sticky::after {
  content:''!important; position:absolute!important; bottom:-60px!important; left:-30px!important;
  width:220px!important; height:220px!important; border-radius:50%!important;
  background:rgba(255,255,255,0.04)!important; pointer-events:none!important; z-index:0!important;
}
.sidebar.sticky .author__avatar,
.sidebar.sticky .author__content,
.sidebar.sticky .author__urls-wrapper { position:relative!important; z-index:1!important; }

.sidebar.sticky .author__avatar {
  overflow:visible!important; display:flex!important;
  justify-content:center!important; margin-bottom:0.6em!important;
}
.sidebar.sticky .author__avatar img {
  border-radius:12px!important; width:210px!important; max-width:210px!important;
  height:210px!important; object-fit:cover!important; border:none!important;
  outline:none!important; box-shadow:0 6px 24px rgba(0,0,0,0.35)!important;
  transition:transform 0.2s!important; display:block!important;
}
.sidebar.sticky .author__avatar img:hover { transform:translateY(-2px)!important; }
.sidebar.sticky .author__name {
  color:white!important; font-size:1.05em!important; font-weight:700!important;
  text-align:center!important; margin-top:0.7em!important;
}
.sidebar.sticky .author__pronouns { color:rgba(255,255,255,0.5)!important; text-align:center!important; }
.sidebar.sticky .author__bio {
  color:rgba(255,255,255,0.72)!important; font-size:0.82em!important;
  line-height:1.6!important; text-align:center!important; margin-bottom:0.8em!important;
}
.sidebar.sticky p, .sidebar.sticky li:not(.author__urls li) {
  color:rgba(255,255,255,0.65)!important; font-size:0.8em!important;
}
.sidebar.sticky .author__urls-wrapper button {
  background:rgba(255,255,255,0.12)!important; color:rgba(255,255,255,0.9)!important;
  border:1px solid rgba(255,255,255,0.25)!important; border-radius:20px!important;
  font-size:0.8em!important; padding:0.3em 1em!important; width:100%!important;
}
.sidebar.sticky .author__urls {
  display:flex!important; flex-wrap:wrap!important; gap:5px!important;
  justify-content:center!important; padding:0.3em 0 0!important;
  list-style:none!important; margin:0!important;
}
.sidebar.sticky .author__urls li {
  display:inline-flex!important; list-style:none!important;
  background:transparent!important; border:none!important; padding:0!important;
  transition:transform 0.15s!important;
}
.sidebar.sticky .author__urls li:hover { transform:translateY(-2px)!important; }
.sidebar.sticky .author__urls li a {
  display:inline-flex!important; align-items:center!important; gap:0.3em!important;
  padding:0.28em 0.8em!important; border-radius:20px!important;
  font-size:0.75em!important; font-weight:600!important;
  color:white!important; text-decoration:none!important; white-space:nowrap!important;
  background:rgba(255,255,255,0.18)!important;
  box-shadow:0 2px 6px rgba(0,0,0,0.2)!important; transition:filter 0.15s!important;
}
.sidebar.sticky .author__urls li a:hover { filter:brightness(1.2)!important; }
.sidebar.sticky .author__urls a i,
.sidebar.sticky .author__urls a svg,
.sidebar.sticky .author__urls a img,
.sidebar.sticky .author__urls a [class*="fa-"] { display:none!important; }
.sidebar.sticky .author__urls a[href*="mailto"]::before          { content:"📧 "; }
.sidebar.sticky .author__urls a[href*="mailto"]                  { background:#e53e3e!important; }
.sidebar.sticky .author__urls a[href*="scholar.google"]::before  { content:"🎓 "; }
.sidebar.sticky .author__urls a[href*="scholar.google"]          { background:#4285f4!important; }
.sidebar.sticky .author__urls a[href*="orcid"]::before           { content:"🔬 "; }
.sidebar.sticky .author__urls a[href*="orcid"]                   { background:#78b13f!important; }
.sidebar.sticky .author__urls a[href*="researchgate"]::before    { content:"📊 "; }
.sidebar.sticky .author__urls a[href*="researchgate"]            { background:#00b0a0!important; }
.sidebar.sticky .author__urls a[href*="semanticscholar"]::before { content:"🧠 "; }
.sidebar.sticky .author__urls a[href*="semanticscholar"]         { background:#7c3aed!important; }
.sidebar.sticky .author__urls a[href*="github"]::before          { content:"💻 "; }
.sidebar.sticky .author__urls a[href*="github"]                  { background:#24292e!important; }
.sidebar.sticky .author__urls a[href*="linkedin"]::before        { content:"💼 "; }
.sidebar.sticky .author__urls a[href*="linkedin"]                { background:#0077b5!important; }

/* ── Home page content styles ── */
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

/* ── Timeline ── */
.timeline {
  position: relative;
  padding-left: 2.2em;
  margin: 0.5em 0 1em;
}
.timeline::before {
  content: '';
  position: absolute;
  left: 0.72em;
  top: 0.4em;
  bottom: 0.4em;
  width: 2px;
  background: linear-gradient(to bottom, #2c6fad 0%, #90cdf4 60%, #c3daf7 100%);
  border-radius: 1px;
}
.timeline-item {
  position: relative;
  margin-bottom: 1.5em;
  opacity: 0;
  transform: translateX(-10px);
  animation: timeline-in 0.7s ease forwards;
}
.timeline-item:nth-child(1) { animation-delay: 0.15s; }
.timeline-item:nth-child(2) { animation-delay: 0.35s; }
.timeline-item:nth-child(3) { animation-delay: 0.55s; }
.timeline-item:nth-child(4) { animation-delay: 0.75s; }
.timeline-item:nth-child(5) { animation-delay: 0.95s; }
@keyframes timeline-in {
  to { opacity: 1; transform: translateX(0); }
}
.timeline-item::before {
  content: '';
  position: absolute;
  left: -1.68em;
  top: 0.35em;
  width: 11px;
  height: 11px;
  border-radius: 50%;
  background: #2c6fad;
  border: 2px solid white;
  box-shadow: 0 0 0 2px #2c6fad;
}
.timeline-item.latest::before {
  background: #4a90d9;
  animation: pulse 2.2s ease-in-out infinite;
}
@keyframes pulse {
  0%, 100% { box-shadow: 0 0 0 2px #4a90d9, 0 0 0 0 rgba(74,144,217,0.55); }
  50%      { box-shadow: 0 0 0 2px #4a90d9, 0 0 0 10px rgba(74,144,217,0); }
}
.timeline-date {
  font-size: 0.78em;
  font-weight: 600;
  color: #2c6fad;
  text-transform: uppercase;
  letter-spacing: 0.04em;
  margin-bottom: 0.3em;
}
.timeline-content {
  font-size: 0.92em;
  line-height: 1.7;
  color: #2d3748;
}
.timeline-content strong { color: #1b3a5c; }
.timeline-content a { color: #2c6fad; font-weight: 600; }
.timeline-pill {
  display: inline-block;
  background: #ebf4ff; color: #2b6cb0;
  border-radius: 20px; padding: 0.1em 0.6em;
  font-size: 0.78em; border: 1px solid #bee3f8;
  margin: 0 0.15em; vertical-align: middle;
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

<!-- ══════════════ NEWS / TIMELINE ══════════════ -->
<div class="hs">Recent Activities</div>

<div class="timeline">

  <div class="timeline-item latest">
    <div class="timeline-date">🇩🇪 December 2025 · PCS 2025, Aachen</div>
    <div class="timeline-content">
      Presented <strong>SCALED</strong> at the Picture Coding Symposium 2025.
      <span class="timeline-pill">Conference paper</span>
      <span class="timeline-pill">Poster</span><br/>
      <a href="https://arxiv.org/pdf/2602.00198" target="_blank">📄 PDF</a>
      &nbsp;·&nbsp;
      <a href="/publication/scaled">🔍 Details</a>
      &nbsp;·&nbsp;
      <a href="/talks/">🖼 Poster</a>
    </div>
  </div>

</div>
