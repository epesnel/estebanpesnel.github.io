---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<style>
.cv-section { margin-bottom: 2em; }
.cv-entry { margin-bottom: 1.4em; }
.cv-entry-header { display: flex; justify-content: space-between; align-items: baseline; flex-wrap: wrap; }
.cv-date { color: #666; font-size: 0.9em; white-space: nowrap; }
.cv-title { font-weight: 600; font-size: 1.05em; }
.cv-subtitle { color: #444; font-style: italic; }
.cv-tags { margin-top: 0.3em; }
.cv-tag { display: inline-block; background: #f0f0f0; border-radius: 3px; padding: 1px 7px; font-size: 0.78em; margin: 2px 2px 2px 0; color: #444; }
.cv-tag-blue { background: #deeaf7; color: #1a5276; }
.cv-tag-green { background: #d5f0e0; color: #1a6b3c; }
.cv-divider { border: none; border-top: 1px solid #e0e0e0; margin: 0.5em 0 1.2em 0; }
.skill-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(180px, 1fr)); gap: 0.5em; }
.skill-item { background: #f8f8f8; border-left: 3px solid #4a90d9; padding: 0.3em 0.6em; font-size: 0.9em; }
.highlight-box { background: #f7fbff; border-left: 4px solid #4a90d9; padding: 0.6em 1em; margin: 0.5em 0; font-size: 0.92em; }
</style>

---

## 🎓 Education

<hr class="cv-divider"/>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">Ph.D. — Signal Processing, Artificial Intelligence & Video Compression</span>
<span class="cv-date">Jun 2023 – Jun 2026</span>
</div>
<div class="cv-subtitle">Université de Rennes · INRIA team COMPACT · MediaKind (CIFRE)</div>
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
<span class="cv-title">M.Eng. — Aerospace & Aeronautical Engineering (Exchange)</span>
<span class="cv-date">Sep 2022 – Jan 2023</span>
</div>
<div class="cv-subtitle">École de technologie supérieure (ÉTS) · Montréal, QC, Canada</div>

Selected courses: Fly-by-wire systems (MGA804), Video communication systems (MTI810), DSP architecture (SYS835), Introduction to avionics (GPA745).
<div class="cv-tags">
<span class="cv-tag">C++</span>
<span class="cv-tag">DSP</span>
<span class="cv-tag">Embedded Systems</span>
<span class="cv-tag">Avionics</span>
</div>
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">M.Ing. — Electronic & Computer Engineering</span>
<span class="cv-date">2020 – 2023</span>
</div>
<div class="cv-subtitle">INSA Rennes (Institut National des Sciences Appliquées)</div>

Embedded systems design (hardware & software), digital/analog signal processing, image analysis, artificial intelligence (NN, CNN, transfer learning, GANs), VHDL, real-time systems.
<div class="cv-tags">
<span class="cv-tag">C/C++</span>
<span class="cv-tag">VHDL</span>
<span class="cv-tag">Signal Processing</span>
<span class="cv-tag">Neural Networks</span>
<span class="cv-tag">MATLAB</span>
</div>
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">CUPGE — Computer Science & Engineering (Preparatory cycle)</span>
<span class="cv-date">2018 – 2020</span>
</div>
<div class="cv-subtitle">ESIR — École Supérieure d'Ingénieurs de Rennes</div>

Rank: **4th / 45**. Foundations of IT, functional and OO programming, digital/analog electronics, mathematical engineering.
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">Baccalauréat Scientifique — SVT, option Physique-Chimie</span>
<span class="cv-date">2015 – 2018</span>
</div>
<div class="cv-subtitle">Lycée Anita Conti · Mention Bien</div>
</div>

---

## 💼 Experience

<hr class="cv-divider"/>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">PhD Researcher — Neural Video Compression</span>
<span class="cv-date">Aug 2023 – present</span>
</div>
<div class="cv-subtitle">MediaKind · Rennes, France (Hybrid) — CIFRE Partnership with INRIA</div>

- Developed surrogate gradient methods enabling end-to-end training of neural networks through non-differentiable video codecs (H.264/AVC, H.266/VVC).
- Proposed a geometric interpretation of the SCALED surrogate gradient as an oblique projection, establishing its MSE-optimality under intensity-shift invariance.
- Extended the framework to full neural wrapper optimization (pre- and post-processing), achieving BD-Rate (PSNR) reductions up to **−23.59%** on x264 and **−20.07%** on VVenC.
- Paper accepted at **PCS 2025**, Aachen (IEEE Signal Processing Society).
<div class="cv-tags">
<span class="cv-tag cv-tag-blue">PyTorch</span>
<span class="cv-tag cv-tag-blue">x264 / VVenC</span>
<span class="cv-tag cv-tag-blue">Surrogate Gradients</span>
<span class="cv-tag cv-tag-blue">U-Net</span>
<span class="cv-tag cv-tag-blue">BD-Rate</span>
<span class="cv-tag cv-tag-blue">PSNR / SSIM / VMAF</span>
</div>
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">Part-time Lecturer</span>
<span class="cv-date">Mar 2024 – Jun 2025</span>
</div>
<div class="cv-subtitle">Université de Rennes · Rennes, France (On-site)</div>

Supervised practical courses across three teaching units:
- **ACV** — Video compression basics (ESIR 2nd year)
- **AI & Data Science** — M2 EEEA and ISTIC
- **Python / C++ Programming** — M2 SIVOS, ISTIC
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">Video Codec Research Intern</span>
<span class="cv-date">Jan 2023 – Jul 2023</span>
</div>
<div class="cv-subtitle">MediaKind · Cesson-Sévigné, France</div>

- Designed fast algorithms for VVC/HEVC intra/inter partitioning.
- Built a prediction model to estimate the optimal split pattern for a given coding unit, reducing encoding complexity.
<div class="cv-tags">
<span class="cv-tag">H.266 / VVC</span>
<span class="cv-tag">HEVC</span>
<span class="cv-tag">Video Compression</span>
<span class="cv-tag">C++</span>
</div>
</div>

<div class="cv-entry">
<div class="cv-entry-header">
<span class="cv-title">Video Research Intern</span>
<span class="cv-date">May 2022 – Aug 2022</span>
</div>
<div class="cv-subtitle">Haivision · Rennes, France</div>

- AV1 / VP9 transcoding evaluation for social network delivery pipelines.
- Subjective and objective quality assessments (VMAF, PSNR, BD-Rate).
- Real-time analysis on Intel platform with SVT optimizations.
- Developed a full performance analysis tool (GStreamer / libx264, Shell / Python / JS).
- Integrated ML algorithms in C for content-aware preset prediction in H.264.
<div class="cv-tags">
<span class="cv-tag">AV1</span>
<span class="cv-tag">VP9</span>
<span class="cv-tag">VMAF</span>
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
<div class="cv-subtitle">Harmonic · France</div>

Study of the impact of AI-based upscaling (Pixop) followed by downscaling on perceived quality and H.264/H.265 encoding performance.
<div class="cv-tags">
<span class="cv-tag">Super-resolution</span>
<span class="cv-tag">H.264 / H.265</span>
<span class="cv-tag">Perceptual Quality</span>
</div>
</div>

---

## 🛠 Skills

<hr class="cv-divider"/>

**Programming & Frameworks**
<div class="skill-grid">
<div class="skill-item">Python (advanced)</div>
<div class="skill-item">C / C++ (advanced)</div>
<div class="skill-item">PyTorch</div>
<div class="skill-item">Shell / Bash</div>
<div class="skill-item">MATLAB</div>
<div class="skill-item">VHDL</div>
<div class="skill-item">JavaScript</div>
</div>

**Video & Compression**
<div class="skill-grid">
<div class="skill-item">H.264 / AVC (x264)</div>
<div class="skill-item">H.265 / HEVC</div>
<div class="skill-item">H.266 / VVC (VVenC)</div>
<div class="skill-item">AV1 / VP9</div>
<div class="skill-item">ABR Streaming</div>
<div class="skill-item">Bitrate Ladder</div>
<div class="skill-item">VMAF / PSNR / SSIM</div>
<div class="skill-item">BD-Rate Analysis</div>
</div>

**Machine Learning & AI**
<div class="skill-grid">
<div class="skill-item">Deep Learning</div>
<div class="skill-item">CNN / U-Net</div>
<div class="skill-item">GANs</div>
<div class="skill-item">Transfer Learning</div>
<div class="skill-item">Differentiable Programming</div>
<div class="skill-item">Surrogate Gradients</div>
<div class="skill-item">Rate-Distortion Optimization</div>
</div>

---

## 📄 Publications

<hr class="cv-divider"/>

<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

---

## 🎤 Talks

<hr class="cv-divider"/>

<ul>{% for post in site.talks reversed %}
  {% include archive-single-talk-cv.html %}
{% endfor %}</ul>

---

## 🏫 Teaching

<hr class="cv-divider"/>

<ul>{% for post in site.teaching reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

---

## 🌍 Languages

<hr class="cv-divider"/>

| Language | Level |
|----------|-------|
| 🇫🇷 French | Native |
| 🇬🇧 English | Full professional proficiency — TOEIC **935 / 990** (2022) |
| 🇪🇸 Spanish | Limited professional proficiency |

---


