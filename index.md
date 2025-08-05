---
layout: null
title: ""
permalink: /
author_profile: false
classes: wide
toc: false
---

<!-- Page-specific styles -->
<style>
  body {
  overflow-x: hidden;
}

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
  
    /* 7) Remove RSS feed icon in footer */
    .page__footer {
  display: none !important;
}
  /* 8) Remove excess spacing between sections */
section {
  margin-bottom: 5px !important;
  padding-bottom: 0 !important;
}

  }

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
    <a href="#guidelines" class="btn">Guidelines</a>
    <a href="#timeline" class="btn">Timeline</a>
    <a href="#organizers" class="btn">Organizers</a>
    <a href="#contact" class="btn">Contact</a>
  </div>
</header>

<section id="about">
  <h2>Call for Participation</h2>
  <p>
    The <strong>Radar Acoustic Speech Enhancement (RASE) Challenge 2026</strong> is an official <strong>ICASSP Grand Challenge</strong> that invites researchers and practitioners in speech processing, machine learning, and signal enhancement to tackle a novel task: reconstructing intelligible, full-bandwidth speech from degraded signals captured using <strong>millimeter-wave (mmWave) radar</strong> — even through glass walls.
  </p>
  <p>
    Conventional microphones struggle in noisy or occluded environments. mmWave FMCW radar offers a non-contact alternative by capturing surface vibrations induced by speech. However, radar-captured signals are often band-limited and noisy. This challenge aims to bridge the gap between radar sensing and high-quality speech reconstruction.
  </p>
</section>

<section id="dataset">
  <h2>Dataset</h2>
  <p>
    Participants will receive a curated dataset comprising paired radar-captured and microphone-recorded speech. The data is collected using a 
    <strong>TI AWR2243BOOST mmWave FMCW radar</strong> through a <strong>glass-walled meeting room</strong>.
  </p>

  <h3>Data Scenarios</h3>
  <ul>
    <li><strong>Direct diaphragm vibration</strong> (Simplest case)<br>
      Radar captures strong vibrations directly from a loudspeaker diaphragm.
    </li>
    <li><strong>Secondary surface vibration</strong> (Moderate case)<br>
      Vibrations are induced on a desktop casing near the loudspeaker.
    </li>
    <li><strong>Laptop screen in virtual meeting</strong> (Most challenging)<br>
      Radar captures subtle vibrations from the laptop screen during speech playback in a simulated meeting setup.
    </li>
  </ul>

  <h3>Notes</h3>
  <ul>
    <li>All recordings are provided in <code>.wav</code> format.</li>
    <li>Raw radar signals are <strong>not shared</strong> — no radar signal processing expertise is needed.</li>
    <li>The dataset is split into <strong>training</strong>, <strong>development</strong>, and <strong>test</strong> sets.</li>
    <li><strong>Registered participants</strong> will receive access.</li>
  </ul>
</section>


<section id="evaluation">
  <h2>Evaluation</h2>
  <p>Submissions will be evaluated using four standard metrics:</p>
  <ul>
    <li><strong>PESQ</strong> – Perceptual Evaluation of Speech Quality</li>
    <li><strong>ESTOI</strong> – Extended Short-Time Objective Intelligibility</li>
    <li><strong>DNSMOS</strong> – Deep Noise Suppression Mean Opinion Score</li>
    <li><strong>MFCC Cosine Similarity</strong></li>
  </ul>

  <p><strong>Difficulty-weighted scoring:</strong></p>
  <ul>
    <li>Easy: 25%</li>
    <li>Medium: 35%</li>
    <li>Hard: 40%</li>
  </ul>

  <p><strong>Top‑5 teams</strong> will be invited to present their work at <strong>ICASSP 2026</strong>.</p>
</section>


<section id="baseline">
  <h2>Baseline</h2>
  <p>Baseline deep learning models implemented in <strong>PyTorch</strong> will be provided to help participants kickstart their solutions. These include:</p>
  <ul>
    <li>Spectral mapping networks</li>
    <li>Phase-aware enhancement techniques</li>
    <li>Feature extraction and post-processing tools</li>
  </ul>
  <p>📦 <strong>Release date:</strong> September 07, 2025</p>
</section>

<section id="guidelines">
  <h2>Participation Guidelines</h2>
  <p>To ensure fairness and reproducibility:</p>
  <ul>
    <li>Use only the provided dataset — external data or augmentation is not allowed.</li>
    <li>Train models from scratch (no pre-trained or fine-tuned models).</li>
    <li>Maximum of 300 training epochs allowed.</li>
    <li>Submit code, trained weights, and environment (Docker or requirements file).</li>
    <li>Participants retain all intellectual property rights.</li>
  </ul>
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

  <div style="display: flex; flex-wrap: nowrap; overflow-x: auto; gap: 40px; justify-content: center;">
    <div style="text-align: center;">
      <img src="/assets/images/organizers/andy.png" width="140"><br>
      <strong>Andy W. H. Khong</strong><br>NTU Singapore (Chair)
    </div>
    <div style="text-align: center;">
      <img src="/assets/images/organizers/naylor.png" width="140"><br>
      <strong>Patrick A. Naylor</strong><br>Imperial College London (Co-chair)
    </div>
    <div style="text-align: center;">
      <img src="/assets/images/organizers/zhiwei.png" width="140"><br>
      <strong>Zhi‑Wei Tan</strong><br>NTU Singapore
    </div>
    <div style="text-align: center;">
      <img src="/assets/images/organizers/reju.png" width="140"><br>
      <strong>V. G. Reju</strong><br>NTU Singapore
    </div>
    <div style="text-align: center;">
      <img src="/assets/images/organizers/ritesh.png" width="140"><br>
      <strong>Ritesh C. Tewari</strong><br>NTU Singapore
    </div>
    <div style="text-align: center;">
      <img src="/assets/images/organizers/ruotong.png" width="140"><br>
      <strong>Ruotong Ding</strong><br>NTU Singapore
    </div>
  </div>
</section>


<section id="contact">
  <h2>Contact</h2>
  <p>📧 <strong>rase_challenge@ntu.edu.sg</strong></p>
</section>

<p class="updated">Last updated: August 5, 2025</p>
