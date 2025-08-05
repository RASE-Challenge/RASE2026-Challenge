---
layout: single
title: "RASE 2026: Radar Acoustic Speech Enhancement"
permalink: /
author_profile: false
classes: wide
hide_nav: true
---

<!-- Hero Banner -->
<header style="text-align: center; padding: 100px 20px; background: linear-gradient(to right, #0f4c81, #28a745); color: white;">
  <h1 style="font-size: 3em;">RASE 2026: Radar Acoustic Speech Enhancement</h1>
  <p style="font-size: 1.5em;">ICASSP 2026 Grand Challenge</p>
  <p>Speech enhancement through glass using mmWave radar</p>
  <div style="margin-top: 30px;">
    <a href="#about" class="btn">About</a>
    <a href="#dataset" class="btn">Dataset</a>
    <a href="#evaluation" class="btn">Evaluation</a>
    <a href="#baseline" class="btn">Baseline</a>
    <a href="#timeline" class="btn">Timeline</a>
    <a href="#organizers" class="btn">Organizers</a>
    <a href="#contact" class="btn">Contact</a>
  </div>
</header>

<style>
  .btn {
    background: white;
    color: #0f4c81;
    padding: 10px 15px;
    margin: 5px;
    border-radius: 5px;
    text-decoration: none;
    font-weight: bold;
  }
  .btn:hover {
    background: #e8e8e8;
  }
  section {
    padding: 60px 20px;
    max-width: 1500px;
    margin: auto;
  }
  h2 {
    border-bottom: 2px solid #ccc;
    padding-bottom: 5px;
  }
</style>

---

<section id="about">
  <h2>About</h2>
  <p>The <strong>RASE 2026 Challenge</strong> at <strong>ICASSP 2026</strong> focuses on speech enhancement from <strong>mmWave radar</strong> data through glass barriers. Participants will receive radar-microphone paired data, develop enhancement models, and compete for top rankings.</p>
</section>

<section id="dataset">
  <h2>Dataset</h2>
  <p>Radar signals are recorded using the <strong>TI AWR2243 mmWave radar</strong>. The challenge includes 3 difficulty levels:</p>
  <ul>
    <li><strong>Loudspeaker diaphragm</strong> (simplest)</li>
    <li><strong>Secondary surface vibrations</strong> (moderate)</li>
    <li><strong>Laptop screen in a virtual meeting</strong> (most challenging)</li>
  </ul>
  <p>Paired microphone recordings are provided in <code>.wav</code> format. No radar processing knowledge is required.</p>
</section>

<section id="evaluation">
  <h2>Evaluation</h2>
  <p>Submissions will be evaluated using:</p>
  <ul>
    <li><strong>PESQ</strong> – Perceptual Evaluation of Speech Quality</li>
    <li><strong>ESTOI</strong> – Extended Short-Time Objective Intelligibility</li>
    <li><strong>DNSMOS</strong> – Deep Noise Suppression Mean Opinion Score</li>
    <li><strong>MFCC Cosine Similarity</strong></li>
  </ul>
  <p>Final score is difficulty-weighted: Easy (25%) + Medium (35%) + Hard (40%)</p>
</section>

<section id="baseline">
  <h2>Baseline</h2>
  <p>Baseline PyTorch models include:</p>
  <ul>
    <li>Spectral feature mapping networks</li>
    <li>Phase-aware enhancement models</li>
    <li>Pre/post-processing pipelines</li>
  </ul>
  <p><strong>Baseline Release:</strong> September 07, 2025</p>
</section>

<section id="timeline">
  <h2>Timeline</h2>
  <ul>
    <li>📅 <strong>Registration Starts:</strong> September 07, 2025</li>
    <li>📂 <strong>Data & Baseline Release:</strong> September 07, 2025</li>
    <li>🧪 <strong>Submission Deadline:</strong> November 14, 2025</li>
    <li>🏆 <strong>Ranking Announcement:</strong> November 24, 2025</li>
    <li>✍️ <strong>2-page Papers:</strong> December 07, 2025</li>
    <li>✅ <strong>Acceptance Notification:</strong> January 11, 2026</li>
    <li>📌 <strong>Camera-ready Deadline:</strong> January 18, 2026</li>
  </ul>
</section>

<section id="organizers">
  <h2>Organizers</h2>
  <ul>
    <li>Andy W. H. Khong (NTU Singapore)</li>
    <li>Patrick A. Naylor (Imperial College London)</li>
    <li>Zhi-Wei Tan (NTU Singapore)</li>
    <li>V. G. Reju (NTU Singapore)</li>
    <li>Ritesh Chandra Tewari (NTU Singapore)</li>
    <li>Ruotong Ding (NTU Singapore)</li>
  </ul>
</section>

<section id="contact">
  <h2>Contact</h2>
  <p>📧 <strong>rase2026@ntu.edu.sg</strong></p>
</section>

---

<p style="text-align: center; font-size: small; color: gray;">Last updated: August 5, 2025</p>
