---
permalink: /
title: "Esteban Pesnel's homepage"
description: "PhD Student in Video Compression & Deep Learning. Research on neural codec wrappers, surrogate gradients, and ABR streaming. INRIA CompACT & MediaKind, Rennes."
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
/* ── Home - Apple-like ── */
.intro-card {
  background: var(--card-bg);
  -webkit-backdrop-filter: saturate(180%) blur(20px);
  backdrop-filter: saturate(180%) blur(20px);
  border: 1px solid var(--card-border);
  border-radius: var(--radius, 16px);
  padding: 1.6em 1.8em;
  margin-bottom: 2.5em;
  font-size: 0.95em;
  line-height: 1.85;
  color: var(--text);
}
.intro-card p { margin: 0.6em 0 0; }
.intro-thesis {
  font-size: 0.92em; color: var(--heading); margin-bottom: 0.4em;
  font-weight: 600;
}

.topic-grid {
  display: grid; grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 0.8em; margin: 1em 0 2em;
}
.topic-item {
  background: linear-gradient(135deg, var(--card-bg) 0%, rgba(41,151,255,0.06) 100%);
  border: 1px solid var(--card-border);
  -webkit-backdrop-filter: saturate(180%) blur(20px);
  backdrop-filter: saturate(180%) blur(20px);
  border-radius: var(--radius-sm, 10px); padding: 0.85em 1.1em;
  font-size: 0.84em; color: var(--text-secondary, #6e6e73); line-height: 1.4;
  display: flex; align-items: center; gap: 0.5em;
  transition: all 0.4s cubic-bezier(0.25,0.46,0.45,0.94);
  position: relative; overflow: hidden;
}
.topic-item::before {
  content: ''; position: absolute; top: 0; left: 0; right: 0; bottom: 0;
  background: linear-gradient(135deg, transparent 60%, rgba(255,140,66,0.06) 100%);
  pointer-events: none;
}
.topic-item:hover {
  transform: translateY(-3px) scale(1.03);
  box-shadow: 0 8px 24px rgba(0,0,0,0.2);
  border-color: var(--accent);
  background: linear-gradient(135deg, var(--card-bg) 0%, rgba(41,151,255,0.14) 100%);
  color: var(--text-primary);
}

.hs {
  font-size: 1.3em; font-weight: 700; color: var(--heading);
  letter-spacing: -0.03em;
  border-left: none; padding-left: 0;
  margin: 2.5em 0 1em;
}

.research-card {
  background: var(--card-bg); border: 1px solid var(--card-border);
  -webkit-backdrop-filter: saturate(180%) blur(20px);
  backdrop-filter: saturate(180%) blur(20px);
  border-radius: var(--radius, 16px); padding: 1.8em 2em; margin-bottom: 2em;
}
.research-card p { font-size: 0.95em; line-height: 1.85; color: var(--text); margin: 0 0 1em; }
.research-card p:last-child { margin-bottom: 0; }
.eq-block {
  background: var(--eq-bg);
  border-radius: var(--radius-sm, 10px);
  border-left: none;
  padding: 1em 1.4em;
  margin: 1em 0; overflow-x: auto; text-align: center;
}

/* ── Timeline ── */
.timeline {
  position: relative;
  padding-left: 2.2em;
  margin: 0.5em 0 1.5em;
}
.timeline::before {
  content: '';
  position: absolute; left: 0.72em; top: 0.4em; bottom: 0.4em;
  width: 1px;
  background: linear-gradient(to bottom, var(--accent, #2997ff) 0%, var(--separator) 100%);
}
.timeline-item {
  position: relative; margin-bottom: 1.8em;
  opacity: 0; transform: translateY(10px);
  animation: timeline-in 0.6s cubic-bezier(0.25,0.46,0.45,0.94) forwards;
}
.timeline-item:nth-child(1) { animation-delay: 0.15s; }
.timeline-item:nth-child(2) { animation-delay: 0.3s; }
.timeline-item:nth-child(3) { animation-delay: 0.45s; }
.timeline-item:nth-child(4) { animation-delay: 0.6s; }
.timeline-item:nth-child(5) { animation-delay: 0.75s; }
@keyframes timeline-in {
  to { opacity: 1; transform: translateY(0); }
}
.timeline-item::before {
  content: '';
  position: absolute; left: -1.68em; top: 0.4em;
  width: 8px; height: 8px; border-radius: 50%;
  background: var(--accent, #2997ff);
  border: 2px solid var(--bg, #000);
  box-shadow: 0 0 0 2px var(--accent, #2997ff);
}
.timeline-item.latest::before {
  background: var(--accent, #2997ff);
  animation: pulse 2.5s ease-in-out infinite;
}
@keyframes pulse {
  0%, 100% { box-shadow: 0 0 0 2px var(--accent, #2997ff), 0 0 0 0 rgba(41,151,255,0.4); }
  50%      { box-shadow: 0 0 0 2px var(--accent, #2997ff), 0 0 0 10px rgba(41,151,255,0); }
}
.timeline-date {
  font-size: 0.76em; font-weight: 600; color: var(--accent, #2997ff);
  text-transform: uppercase; letter-spacing: 0.05em; margin-bottom: 0.4em;
}
.timeline-content {
  font-size: 0.92em; line-height: 1.75; color: var(--text);
}
.timeline-content strong { color: var(--heading); }
.timeline-content a { color: var(--accent, #2997ff); font-weight: 500; }
.timeline-pill {
  display: inline-block;
  background: var(--pill-bg); color: var(--pill-text);
  border-radius: 20px; padding: 0.15em 0.65em;
  font-size: 0.76em; border: 1px solid var(--pill-border);
  margin: 0 0.15em; vertical-align: middle;
}
</style>

<!-- ══════════════ INTRO ══════════════ -->
<div class="intro-card">
  <p>I'm a PhD student jointly affiliated with <strong>INRIA</strong> (team CompACT) and <strong>MediaKind</strong> in Rennes, France. My research sits at the intersection of deep learning and video compression - designing neural networks that make standard codecs more efficient.</p>
  <p>Before starting my PhD, I graduated from <strong>INSA Rennes</strong> in electronics &amp; computer engineering, with an exchange semester in aerospace engineering at <strong>ÉTS Montréal</strong>.</p>
</div>

<!-- ══════════════ RESEARCH TOPICS ══════════════ -->
<div class="hs">Research Focus</div>

<div class="topic-grid">
  <div class="topic-item">🔁 Codec-aware neural optimization</div>
  <div class="topic-item">📡 ABR streaming</div>
  <div class="topic-item">🧠 Neural codec wrappers</div>
  <div class="topic-item">∂ Differentiable codec modeling</div>
  <div class="topic-item">📊 Rate-distortion optimization</div>
  <div class="topic-item">⚡ Lightweight architecture</div>
</div>

<!-- ══════════════ RESEARCH OVERVIEW ══════════════ -->
<div class="hs">Research Overview</div>

<div class="research-card">
<p>My research focuses on <strong>end-to-end rate-distortion optimization</strong> of video streaming systems by jointly learning neural pre-processing \(f\) and post-processing \(g\) around a standard video codec \(\phi\):</p>

<div class="eq-block">
$$\hat{x} = g\!\bigl(\phi(f(x))\bigr), \qquad \min_{\theta_f,\,\theta_g}\; D(\hat{x}, x) + \lambda\, R\!\bigl(f(x)\bigr)$$
</div>

<p>The central challenge is that conventional codecs (H.264, HEVC, ...) are <strong>non-differentiable</strong> - gradients cannot flow through them, preventing standard backpropagation across the full pipeline. My work explores strategies to overcome this barrier: surrogate gradients, differentiable proxies, and codec-aware training schemes.</p>
</div>

<!-- ══════════════ NEWS / TIMELINE ══════════════ -->
<div class="hs">Recent Activities</div>

<div class="timeline">

  <div class="timeline-item latest">
    <div class="timeline-date">🇩🇪 December 2025 · PCS 2025, Aachen</div>
    <div class="timeline-content">
      Presented <strong>SCALED</strong> at the Picture Coding Symposium 2025 !
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
