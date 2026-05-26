---
layout: archive
title: ""
permalink: /resume/
author_profile: false
redirect_from:
  - /cv
  - /cv/
---

{% include base_path %}

<style>

/* ── Entries ── */
.cv-entry { margin-bottom: 1.6em; }
.cv-entry-header { display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 0.4em; }
.cv-date { color: var(--text-muted); font-size: 0.88em; white-space: nowrap; }
.cv-title { font-weight: 600; font-size: 1.05em; color: var(--title); }
.cv-subtitle { color: var(--text-muted); font-style: italic; margin: 0.15em 0 0.4em 0; }
.cv-tags { margin-top: 0.4em; }
.cv-tag { display: inline-block; background: var(--blue-pale); border-radius: 3px; padding: 1px 7px; font-size: 0.78em; margin: 2px 2px 2px 0; color: var(--text-muted); }
.cv-tag-blue { background: var(--pill-bg); color: var(--pill-text); }
.cv-tag-green { background: var(--pill-bg); color: #48bb78; }
.cv-divider { border: none; border-top: 1px solid var(--card-border); margin: 0.4em 0 1.2em 0; }
.skill-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(180px, 1fr)); gap: 0.5em; margin-bottom: 1em; }
.skill-item { background: var(--card-bg); border-left: 3px solid var(--blue-light); padding: 0.3em 0.6em; font-size: 0.88em; color: var(--text); }
.highlight-box { background: var(--card-bg); border-left: 4px solid var(--blue-light); padding: 0.6em 1em; margin: 0.5em 0; font-size: 0.91em; line-height: 1.7; color: var(--text); }
.logo { height: 16px; vertical-align: -2px; margin-right: 4px; object-fit: contain; border-radius: 3px; background: rgba(255,255,255,0.9); padding: 2px 4px; }
.skill-cat { font-size: 0.95em; font-weight: 600; margin: 0.8em 0 0.4em 0; color: var(--heading); }

</style>


<div class="strip-wrapper">
<div class="strip-bar"><div class="strip-bar-inner"><span class="strip-bar-text">Resume</span></div></div>
<div class="strip-content">

<h2>&#127891; Education</h2>
<hr class="cv-divider"/>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">
Ph.D. — Signal Processing, Artificial Intelligence &amp; Video Compression
</span>
<span class="cv-date">Jun 2023 – Jun 2026</span>
</div>
<div class="cv-subtitle"><img class="logo" src="{{ base_path }}/images/logos/univ-rennes.png" alt="Université de Rennes"> Université de Rennes &middot; <img class="logo" src="{{ base_path }}/images/logos/inria.png" alt="INRIA"> INRIA team COMPACT &middot; <img class="logo" src="{{ base_path }}/images/logos/mediakind.svg" alt="MediaKind"> MediaKind (CIFRE)</div>
<div class="highlight-box">
<strong>Thesis:</strong> "Learned video downscaling for end-to-end Rate-Distortion optimization of video streaming systems"<br/>
<strong>Industrial supervisors:</strong> J. Le Tanou, M. Ropert (MediaKind)<br/>
<strong>Academic supervisors:</strong> T. Maugey, A. Roumy (INRIA)
</div>
<div class="cv-tags">
<span class="cv-tag cv-tag-blue">Deep Learning</span>
<span class="cv-tag cv-tag-blue">Video Compression</span>
<span class="cv-tag cv-tag-blue">Rate-Distortion Optimization</span>
<span class="cv-tag cv-tag-blue">Surrogate Gradients</span>
<span class="cv-tag cv-tag-blue">ABR Streaming</span>
</div>
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">
M.Ing. — Electronic &amp; Computer Engineering
</span>
<span class="cv-date">2020 – 2023</span>
</div>
<div class="cv-subtitle"><img class="logo" src="{{ base_path }}/images/logos/insa-rennes.png" alt="INSA Rennes"> INSA Rennes — Institut National des Sciences Appliquées</div>
<p>Embedded systems design (hardware &amp; software), digital/analog signal processing, image analysis, AI (NN, CNN, transfer learning, GANs), VHDL, real-time systems.</p>
<div class="cv-tags">
<span class="cv-tag">C/C++</span>
<span class="cv-tag">Signal Processing</span>
<span class="cv-tag">Deep learning</span>
</div>
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">
M.Eng. — Aerospace &amp; Aeronautical Engineering (Exchange semester)
</span>
<span class="cv-date">Sep 2022 – Jan 2023</span>
</div>
<div class="cv-subtitle"><img class="logo" src="{{ base_path }}/images/logos/ets-montreal.svg" alt="ÉTS Montréal"> École de technologie supérieure (ÉTS) &middot; Montréal, QC, Canada</div>
<p>Selected courses: fly-by-wire systems (MGA804), video communication systems (MTI810), DSP architecture (SYS835), introduction to avionics (GPA745).</p>
<div class="cv-tags">
<span class="cv-tag">C++</span>
<span class="cv-tag">DSP</span>
<span class="cv-tag">Avionics</span>
</div>
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">
CUPGE — Computer Science &amp; Engineering (Preparatory cycle)
</span>
<span class="cv-date">2018 – 2020</span>
</div>
<div class="cv-subtitle"><img class="logo" src="{{ base_path }}/images/logos/esir.png" alt="ESIR"> ESIR — École Supérieure d'Ingénieurs de Rennes</div>
<p>Rank: <strong>4th / 45</strong>. Foundations of IT, functional and OO programming, digital/analog electronics, mathematical engineering.</p>
</div>

<hr style="border: none; border-top: 1px solid var(--card-border); margin: 2em 0;"/>

<h2>&#128188; Experience</h2>
<hr class="cv-divider"/>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">
PhD Researcher — Neural Video Compression
</span>
<span class="cv-date">Aug 2023 – present</span>
</div>
<div class="cv-subtitle"><img class="logo" src="{{ base_path }}/images/logos/mediakind.svg" alt="MediaKind"> MediaKind &middot; Rennes, France (Hybrid) — CIFRE Partnership with <img class="logo" src="{{ base_path }}/images/logos/inria.png" alt="INRIA"> INRIA</div>
<ul>
<li>Developed surrogate gradient methods enabling end-to-end training through non-differentiable codecs (H.264/AVC, H.266/VVC).</li>
<li>Proposed a geometric interpretation of the SCALED surrogate gradient as an oblique projection, establishing its MSE-optimality under intensity-shift invariance.</li>
<li>Extended the framework to full neural wrapper optimization (pre- and post-processing), achieving BD-Rate (PSNR) reductions up to <strong>−23.59%</strong> on x264 and <strong>−20.07%</strong> on VVenC.</li>
<li>Paper accepted at <strong>PCS 2025</strong>, Aachen (IEEE Signal Processing Society).</li>
</ul>
<div class="cv-tags">
<span class="cv-tag cv-tag-blue">PyTorch/TensorFlow</span>
<span class="cv-tag cv-tag-blue">Deep learning</span>
<span class="cv-tag cv-tag-blue">Differentiable programming</span>
</div>
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">
Part-time Lecturer
</span>
<span class="cv-date">Mar 2024 – Jun 2025</span>
</div>
<div class="cv-subtitle"><img class="logo" src="{{ base_path }}/images/logos/univ-rennes.png" alt="Université de Rennes"> Université de Rennes &middot; Rennes, France (On-site)</div>
<ul>
<li><strong>ACV</strong> — Video compression basics (ESIR 2nd year)</li>
<li><strong>AI &amp; Data Science</strong> — M2 EEEA and ISTIC</li>
<li><strong>Python / C++ Programming</strong> — M2 SIVOS, ISTIC</li>
</ul>
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">Video Codec Research Intern</span>
<span class="cv-date">Jan 2023 – Jul 2023</span>
</div>
<div class="cv-subtitle"><img class="logo" src="{{ base_path }}/images/logos/mediakind.svg" alt="MediaKind"> MediaKind &middot; Cesson-Sévigné, France</div>
<ul>
<li>Designed fast algorithms for VVC/HEVC intra/inter partitioning.</li>
<li>Built a prediction model to estimate the optimal split pattern for a given coding unit, reducing encoding complexity.</li>
</ul>
<div class="cv-tags">
<span class="cv-tag">H.266 / VVC</span>
<span class="cv-tag">HEVC</span>
<span class="cv-tag">Partitioning</span>
<span class="cv-tag">C++</span>
</div>
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">Video Research Intern</span>
<span class="cv-date">May 2022 – Aug 2022</span>
</div>
<div class="cv-subtitle"><img class="logo" src="{{ base_path }}/images/logos/haivision.png" alt="Haivision"> Haivision &middot; Rennes, France</div>
<ul>
<li>AV1 / VP9 transcoding evaluation for social network delivery pipelines.</li>
<li>Subjective and objective quality assessments (VMAF, PSNR, BD-Rate).</li>
<li>Real-time analysis on Intel platform with SVT optimizations.</li>
<li>Developed a full performance analysis tool (GStreamer / libx264) in Shell / Python / JS.</li>
<li>Integrated ML algorithms in C for content-aware preset prediction in H.264.</li>
</ul>
<div class="cv-tags">
<span class="cv-tag">AV1</span>
<span class="cv-tag">VP9</span>
<span class="cv-tag">Python</span>
<span class="cv-tag">Shell</span>
<span class="cv-tag">Parallel Programming</span>
</div>
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">Video Research Intern</span>
<span class="cv-date">Jun 2021 – Aug 2021</span>
</div>
<div class="cv-subtitle"><img class="logo" src="{{ base_path }}/images/logos/harmonic.png" alt="Harmonic"> Harmonic &middot; France</div>
<p>Study of the impact of AI-based upscaling (Pixop) followed by downscaling on perceived quality and H.264/H.265 encoding performance.</p>
<div class="cv-tags">
<span class="cv-tag">Super-resolution</span>
<span class="cv-tag">H.264 / H.265</span>
<span class="cv-tag">Perceptual Quality</span>
</div>
</div>

<hr style="border: none; border-top: 1px solid var(--card-border); margin: 2em 0;"/>

<h2>&#128736; Skills</h2>
<hr class="cv-divider"/>

<p class="skill-cat">Programming &amp; Frameworks</p>
<div class="skill-grid">
<div class="skill-item">Python (advanced)</div>
<div class="skill-item">C / C++ (advanced)</div>
<div class="skill-item">PyTorch/TensorFlow</div>
<div class="skill-item">VHDL</div>
</div>

<p class="skill-cat">Video &amp; Compression</p>
<div class="skill-grid">
<div class="skill-item">H.264 / AVC (x264)</div>
<div class="skill-item">H.265 / HEVC</div>
<div class="skill-item">H.266 / VVC (VVenC)</div>
<div class="skill-item">AV1 / VP9</div>
<div class="skill-item">ABR Streaming</div>
<div class="skill-item">Bitrate Ladder</div>
</div>

<p class="skill-cat">Machine Learning &amp; AI</p>
<div class="skill-grid">
<div class="skill-item">Deep Learning</div>
<div class="skill-item">CNN / U-Net</div>
<div class="skill-item">Differentiable Programming</div>
<div class="skill-item">Surrogate Gradients</div>
</div>

<hr style="border: none; border-top: 1px solid var(--card-border); margin: 2em 0;"/>

<h2>&#128196; Publications</h2>
<hr class="cv-divider"/>

<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

<hr style="border: none; border-top: 1px solid var(--card-border); margin: 2em 0;"/>

<h2>&#127908; Talks</h2>
<hr class="cv-divider"/>

<ul>{% for post in site.talks reversed %}
  {% include archive-single-talk-cv.html %}
{% endfor %}</ul>

<hr style="border: none; border-top: 1px solid var(--card-border); margin: 2em 0;"/>

<h2>&#127979; Teaching</h2>
<hr class="cv-divider"/>

<ul>{% for post in site.teaching reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

<hr style="border: none; border-top: 1px solid var(--card-border); margin: 2em 0;"/>

<h2>&#127757; Languages</h2>
<hr class="cv-divider"/>

<table>
<thead><tr><th>Language</th><th>Level</th></tr></thead>
<tbody>
<tr><td>&#127467;&#127479; French</td><td>Native</td></tr>
<tr><td>&#127468;&#127463; English</td><td>Full professional proficiency — TOEIC <strong>935 / 990</strong> (2022)</td></tr>
<tr><td>&#127466;&#127480; Spanish</td><td>Limited professional proficiency</td></tr>
</tbody>
</table>

</div>
</div>
