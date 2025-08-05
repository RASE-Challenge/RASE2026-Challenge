---
layout: single
title: "RASE 2026: Radar Acoustic Speech Enhancement"
permalink: /
author_profile: false
classes: wide
toc: false
---

<!-- Page-specific styles -->
<style>
  /* 1) Hide the theme masthead and remove the top gap just for this page */
  .masthead { display: none !important; }
  .initial-content { padding-top: 0 !important; }

  /* 2) Full-bleed helper: lets an element break out to full viewport width */
  .full-bleed {
    width: 100vw;
    position: relative;
    left: 50%;
    right: 50%;
    margin-left: -50vw;
    margin-right: -50vw;
  }

  /* 3) Hero (edge-to-edge gradient bar) */
  .hero {
    text-align: center;
    padding: 96px 20px;
    background: linear-gradient(90deg, #0f4c81 0%, #28a745 100%);
    color: #fff;
  }
  .hero h1 { font-size: clamp(2.2rem, 4.5vw, 3.2rem); margin: 0 0 10px; font-weight: 800; }
  .hero p.lead { font-size: clamp(1.1rem, 2.2vw, 1.5rem); margin: 6px 0; opacity: 0.95; }

  /* 4) Anchor buttons under hero */
  .btn-row { margin-top: 28px; }
  .btn {
    display: inline-block;
    background: #fff;
    color: #0f4c81;
    padding: 10px 16px;
    margin: 6px;
    border-radius: 8px;
    text-decoration: none;
    font-weight: 700;
    border: 1px solid rgba(255,255,255,0.25);
    transition: transform .05s ease, background .15s ease, box-shadow .15s ease;
  }
  .btn:hover { background: #f1f1f1; transform: translateY(-1px); box-shadow: 0 2px 10px rgba(0,0,0,.06); }

  /* 5) Sections */
  section { padding: 60px 20px; max-width: 1100px; margin: 0 auto; }
  section h2 { font-weight: 800; margin-bottom: 12px; }
  section p, section li { font-size: 1.05rem; line-height: 1.65; }
  ul { margin-top: 6px; }

  /* 6) Small footer note */
  .updated { text-align: center; font-size: .9rem; color: #8a8a8a; margin: 18px 0 40px; }
</style>

<!-- Hero Banner (full width) -->
<header class="hero full-bleed">
  <h1>RASE 2026: Radar Acoustic Speech Enhancement</h1>
  <p class="lead">ICASSP 2026 Grand Challenge</p>
  <p>Speech enhancement through glass using mmWave radar</p>

  <div class="btn-row">
    <a href="#about" class="btn">About</a>
    <a href="#dataset" class="btn">Dataset</a>
    <a href="#evaluation" class="btn">Evaluation</a>
    <a href="#baseline" class="btn">Baseline</a>
    <a href="#timeline" class="btn">Timeline</a>
    <a href="#organizers" class="btn">Organizers</a>
    <a href="#contact" class="btn">Contact</a>
  </div>
</header>

<section id="about">
  <h2>About</h2>
  <p>
    The <strong>RASE 2026 Challenge</strong> at <strong>ICASSP 2026</strong> focuses on
    speech enhancement from <strong>mmWave radar</strong> data through glass barriers.
    Participants will receive radar–microphone paired data, develop enhancement models,
    and compete for top rankings.
  </p>
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
  <p><strong>Final score is difficulty‑weighted:</strong> Easy (25%) + Medium (35%) + Hard (40%).</p>
</section>

<section id="baseline">
  <h2>Baseline</h2>
  <p>Baseline PyTorch models include:</p>
  <ul>
    <li>Spectral feature mapping networks</li>
    <li>Phase‑aware enhancement models</li>
    <li>Pre/post‑processing pipelines</li>
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
    <li>✍️ <strong>2‑page Papers (by invite):</strong> December 07, 2025</li>
    <li>✅ <strong>Acceptance Notification:</strong> January 11, 2026</li>
    <li>📌 <strong>Camera‑ready Deadline:</strong> January 18, 2026</li>
  </ul>
</section>

<section id="organizers">
  <h2>Organizers</h2>
  <ul>
    <li>Andy W. H. Khong (NTU Singapore)</li>
    <li>Patrick A. Naylor (Imperial College London)</li>
    <li>Zhi‑Wei Tan (NTU Singapore)</li>
    <li>V. G. Reju (NTU Singapore)</li>
    <li>Ritesh Chandra Tewari (NTU Singapore)</li>
    <li>Ruotong Ding (NTU Singapore)</li>
  </ul>
</section>

<section id="contact">
  <h2>Contact</h2>
  <p>📧 <strong>rase2026@ntu.edu.sg</strong></p>
</section>

<p class="updated">Last updated: August 5, 2025</p>
