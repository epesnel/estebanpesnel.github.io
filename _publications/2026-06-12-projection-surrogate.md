---
layout: single
collection: publications
category: conferences
permalink: /publication/projection-surrogate
title: "A Projection-Based Surrogate Gradient Interpretation for Neural Codec Wrappers"
excerpt: 'Reinterpreting surrogate gradients as first-order local codec approximations, enabling full neural wrapping with up to -23.59% BD-Rate gains.'
date: 2026-06-12
venue: 'Submitted to IEEE MMSP 2026'
paperurl: 'https://hal.science/hal-05653605v1'
author_profile: false
publisher_logo: "logos/ieee-sps.png"
---

{% include base_path %}

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
.sp-result .val { font-size: 1.5em; font-weight: 800; }
.sp-result .lbl { font-size: 0.7em; opacity: 0.88; margin-top: 0.3em; line-height: 1.4; }

/* ── Publisher logo ── */
.sp-publisher {
  display: flex; justify-content: flex-end; align-items: center;
  gap: 0.6em; margin-top: 2em; padding-top: 1em;
  border-top: 1px solid var(--separator);
}
.sp-publisher img {
  height: 32px; width: auto; object-fit: contain;
  opacity: 0.35;
  transition: opacity 0.3s;
}
.sp-publisher img:hover { opacity: 0.7; }
.sp-publisher span {
  font-size: 0.7em; color: var(--text-tertiary); font-weight: 500;
}
</style>

<div class="sp">

<!-- ════════════ HERO ════════════ -->
<div class="sp-hero">
  <div class="sp-hero-logos">
    <img src="{{ base_path }}/images/logos/inria_white.png" alt="INRIA" />
    <img src="{{ base_path }}/images/logos/mediakind.svg" alt="MediaKind" />
  </div>
  <div class="sp-hero-venue">📝 Submitted to IEEE MMSP 2026</div>
  <div class="sp-hero-title">
    A <em>Projection-Based</em> Surrogate Gradient Interpretation<br/>for Neural Codec Wrappers
  </div>
  <div class="sp-authors">
    <span class="me">Esteban Pesnel</span><sup>*†</sup>,
    Julien Le Tanou<sup>*</sup>,
    Michael Ropert<sup>*</sup>,
    Aline Roumy<sup>†</sup>,
    Thomas Maugey<sup>†</sup>
  </div>
  <div class="sp-affiliations">
    <sup>*</sup>MediaKind, Rennes, France &nbsp;&nbsp;
    <sup>†</sup>INRIA, Rennes, France - team COMPACT
  </div>
  <div class="sp-tags">
    <span class="sp-tag">Neural Wrappers</span>
    <span class="sp-tag">End-to-end Optimization</span>
    <span class="sp-tag">Codec Modeling</span>
    <span class="sp-tag">Surrogate Gradient</span>
  </div>
  <div class="sp-buttons">
    <a class="sp-btn sp-btn-primary" href="https://hal.science/hal-05653605v1" target="_blank">📄 HAL preprint</a>
  </div>
</div>

<!-- ════════════ ABSTRACT ════════════ -->
<div class="sp-section">
<div class="sp-section-title">Abstract</div>
<div class="sp-abstract">
Neural wrappers are learned pre- and postprocessing networks designed to enhance the performance of conventional video codecs. Although these approaches can significantly improve compression efficiency, training them remains challenging due to the non-differentiability of video codecs, which arises from the multiple discrete decisions involved in the encoding process. Surrogate gradients have recently emerged as an effective solution for enabling end-to-end learning with conventional codecs. They offer two main advantages: they avoid training an additional network to mimic the codec, and they can improve compression performance. In particular, the recently proposed SCALED method, which leverages the true compression error, has shown strong results for training neural pre-processors such as downscalers. However, this SCALED gradient was originally introduced as a reparameterization trick, which limits its interpretability. In this paper, we show that this surrogate gradient can be interpreted as a <strong>first-order local approximation of the video codec</strong>, providing insight into its effectiveness. We further demonstrate that it is effective not only for learning downscaling operations, but also for the more challenging task of full neural wrapping with pre- and post-processing networks. Finally, we show that the approach generalizes well across different video codecs, quality factors, and tasks, including multiple downscaling ratios, yielding <strong>BD-Rate (PSNR) reductions of up to -23.59% on x264 and -20.07% on VVenC</strong> relative to standard resampling baselines.
</div>
</div>

<!-- ════════════ METHOD ════════════ -->
<div class="sp-section">
<div class="sp-section-title">Key Idea: Modeling the Codec as a Projection</div>

<p>A video codec \(\phi\) can be decomposed as an identity mapping plus a compression error \(\boldsymbol{\epsilon}\):</p>

<div class="sp-eq">
$$\boldsymbol{\hat{y}} = \phi(\boldsymbol{y}) = \boldsymbol{y} + \boldsymbol{\epsilon}$$
<div class="sp-eq-label">Codec decomposition</div>
</div>

<p>Since \(\phi\) is non-differentiable, we need a tractable approximation for backpropagation. We observe empirically that real codecs are <strong>approximately idempotent</strong> (\(\phi^2 \approx \phi\)), <strong>intensity-shift invariant</strong> (\(\phi(\boldsymbol{y}+\delta\boldsymbol{1}) \approx \phi(\boldsymbol{y})+\delta\boldsymbol{1}\)), and that their <strong>centered compression error is orthogonal to the codec output</strong> (\((\boldsymbol{\epsilon}-\bar{\boldsymbol{\epsilon}})^T\boldsymbol{\hat{y}} \approx 0\)). These properties suggest modeling \(\phi\) as a <strong>linear projection</strong> \(\mathbf{P}\), characterized by a projection direction \(\boldsymbol{u}\) and a subspace vector \(\boldsymbol{v}\):</p>

<div class="sp-eq">
$$\hat{\phi}(\boldsymbol{y}) = \mathbf{P}\boldsymbol{y} = \left(\mathbf{I} - \frac{\boldsymbol{u}\,\boldsymbol{v}^T}{\boldsymbol{v}^T\boldsymbol{u}}\right)\boldsymbol{y}$$
<div class="sp-eq-label">Linear projection model of the codec</div>
</div>

<p>The projection direction is naturally \(\boldsymbol{u} = \boldsymbol{\epsilon}\) (the codec shifts the input by the error vector). Intensity-shift invariance requires \(\boldsymbol{v}\) to be zero-mean, and minimizing the MSE between the true codec and its projection model yields \(\boldsymbol{v}^* = \boldsymbol{\epsilon} - \bar{\boldsymbol{\epsilon}}\) (the centered compression error), which satisfies the orthogonality constraint. The resulting <strong>MSE-optimal projector</strong> and its Jacobian are:</p>

<div class="sp-eq">
$$\mathbf{J}_{\text{Proj}} = \mathbf{I} - \frac{\boldsymbol{\epsilon}\,(\boldsymbol{\epsilon} - \bar{\boldsymbol{\epsilon}})^T}{N\,\sigma^2_{\boldsymbol{\epsilon}}} = \mathbf{J}_{\text{SCALED}}$$
<div class="sp-eq-label">Projection-based surrogate Jacobian = SCALED gradient</div>
</div>

<p>This Jacobian is exactly equal to the SCALED surrogate gradient from <a href="/publication/scaled">our previous work</a>. This projection-based interpretation explains <em>why</em> SCALED works: its eigenvalues are bounded in \(\{0, 1\}\), preventing gradient explosion; it adapts instantly to any codec or quality setting (zero-shot); and it relies on true compression errors rather than learned approximations.</p>
</div>

<!-- ════════════ KEY RESULTS ════════════ -->
<div class="sp-section">
<div class="sp-section-title">Key Results</div>

<div class="sp-results">
  <div class="sp-result sp-result-a">
    <div class="val">-23.59%</div>
    <div class="lbl">BD-Rate PSNR<br/>on x264</div>
  </div>
  <div class="sp-result sp-result-b">
    <div class="val">-20.07%</div>
    <div class="lbl">BD-Rate PSNR<br/>on VVenC</div>
  </div>
  <div class="sp-result sp-result-c">
    <div class="val">2 codecs</div>
    <div class="lbl">x264 & VVenC<br/>validated</div>
  </div>
</div>
</div>

<!-- ════════════ CONTRIBUTIONS ════════════ -->
<div class="sp-section">
<div class="sp-section-title">Contributions</div>
<div class="sp-grid">
  <div class="sp-card">
    <strong>🔍 New interpretation</strong>
    Reinterprets the SCALED surrogate gradient as a first-order local approximation of the codec.
  </div>
  <div class="sp-card">
    <strong>🔁 Beyond downscaling</strong>
    Extends surrogate gradient training from downscaling-only to full neural codec wrappers (pre + post processing).
  </div>
  <div class="sp-card">
    <strong>📊 Multi-codec validation</strong>
    Demonstrated on both x264 (H.264) and VVenC (VVC/H.266) with large BD-Rate improvements.
  </div>
</div>
</div>

<div class="sp-publisher">
  <span>Submitted to</span>
  <img src="{{ base_path }}/images/logos/ieee-sps.png" alt="IEEE Signal Processing Society" />
</div>

</div><!-- end .sp -->
