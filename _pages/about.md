---
permalink: /
title: ""
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
/* ── Home page content styles ── */
.intro-card {
  background: var(--card-bg);
  border: 1px solid var(--card-border);
  border-left: 4px solid var(--blue);
  border-radius: 0 10px 10px 0;
  padding: 1.1em 1.4em;
  margin-bottom: 1.8em;
  font-size: 0.93em;
  line-height: 1.75;
  color: var(--text);
}
.intro-card p { margin: 0.5em 0 0; }
.intro-thesis {
  font-size: 0.9em; color: var(--heading); margin-bottom: 0.3em;
}

/* Research topics */
.topic-grid {
  display: grid; grid-template-columns: repeat(auto-fill, minmax(160px, 1fr));
  gap: 0.6em; margin: 0.8em 0 1.6em;
}
.topic-item {
  background: var(--card-bg); border: 1px solid var(--pill-border);
  border-radius: 8px; padding: 0.6em 0.8em;
  font-size: 0.84em; color: var(--heading); line-height: 1.4;
  display: flex; align-items: center; gap: 0.4em;
}

/* Section headers */
.hs { font-size: 1.05em; font-weight: 700; color: var(--heading);
  border-left: 4px solid var(--blue); padding-left: 0.65em;
  margin: 1.8em 0 0.8em; }

/* Research overview card */
.research-card {
  background: var(--card-bg); border: 1px solid var(--card-border);
  border-radius: 10px; padding: 1.3em 1.5em; margin-bottom: 1.5em;
}
.research-card p { font-size: 0.93em; line-height: 1.8; color: var(--text); margin: 0 0 0.8em; }
.research-card p:last-child { margin-bottom: 0; }
.eq-block {
  background: var(--eq-bg); border-left: 3px solid var(--separator);
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
  position: absolute; left: 0.72em; top: 0.4em; bottom: 0.4em;
  width: 2px;
  background: linear-gradient(to bottom, var(--blue) 0%, var(--blue-light) 60%, var(--card-border) 100%);
  border-radius: 1px;
}
.timeline-item {
  position: relative; margin-bottom: 1.5em;
  opacity: 0; transform: translateX(-10px);
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
  position: absolute; left: -1.68em; top: 0.35em;
  width: 11px; height: 11px; border-radius: 50%;
  background: var(--blue);
  border: 2px solid var(--card-bg);
  box-shadow: 0 0 0 2px var(--blue);
}
.timeline-item.latest::before {
  background: var(--blue-light);
  animation: pulse 2.2s ease-in-out infinite;
}
@keyframes pulse {
  0%, 100% { box-shadow: 0 0 0 2px var(--blue-light), 0 0 0 0 rgba(74,144,217,0.55); }
  50%      { box-shadow: 0 0 0 2px var(--blue-light), 0 0 0 10px rgba(74,144,217,0); }
}
.timeline-date {
  font-size: 0.78em; font-weight: 600; color: var(--blue);
  text-transform: uppercase; letter-spacing: 0.04em; margin-bottom: 0.3em;
}
.timeline-content {
  font-size: 0.92em; line-height: 1.7; color: var(--text);
}
.timeline-content strong { color: var(--heading); }
.timeline-content a { color: var(--blue); font-weight: 600; }
.timeline-pill {
  display: inline-block;
  background: var(--pill-bg); color: var(--pill-text);
  border-radius: 20px; padding: 0.1em 0.6em;
  font-size: 0.78em; border: 1px solid var(--pill-border);
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
<p>My research focuses on <strong>end-to-end rate-distortion optimization</strong> of video streaming systems by jointly learning neural pre-processing \(f\) and post-processing \(g\) around a standard video codec \(\phi\):</p>

<div class="eq-block">
$$\hat{x} = g\!\bigl(\phi(f(x))\bigr), \qquad \min_{\theta_f,\,\theta_g}\; D(\hat{x}, x) + \lambda\, R\!\bigl(f(x)\bigr)$$
</div>

<p>The central challenge is that conventional codecs (H.264, HEVC, ...) are <strong>non-differentiable</strong> — gradients cannot flow through them, preventing standard backpropagation across the full pipeline. My work explores strategies to overcome this barrier: surrogate gradients, differentiable proxies, and codec-aware training schemes.</p>
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
