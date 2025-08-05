---
layout: single
title: "RASE 2026: Radar Acoustic Speech Enhancement"
permalink: /
author_profile: false
---

## About

The **Radar Acoustic Speech Enhancement (RASE) Challenge 2026** is an official **ICASSP Grand Challenge** that invites researchers and practitioners in speech processing, machine learning, and signal enhancement to tackle a novel task: reconstructing intelligible, full-bandwidth speech from degraded signals captured using **millimeter-wave (mmWave) radar** — even through glass walls.

Conventional microphones struggle in noisy or occluded environments. mmWave FMCW radar offers a non-contact alternative by capturing surface vibrations induced by speech. However, radar-captured signals are often band-limited and noisy. This challenge aims to bridge the gap between radar sensing and high-quality speech reconstruction.

---

## Dataset

Participants will receive a curated dataset comprising paired radar-captured and microphone-recorded speech. The data is collected using a **TI AWR2243BOOST mmWave FMCW radar** through a **glass-walled meeting room**.

### Data Scenarios

1. **Direct diaphragm vibration** (Simplest case)  
   Radar captures strong vibrations directly from a loudspeaker diaphragm.

2. **Secondary surface vibration** (Moderate case)  
   Vibrations are induced on a desktop casing near the loudspeaker.

3. **Laptop screen in virtual meeting** (Most challenging)  
   Radar captures subtle vibrations from the laptop screen during speech playback in a simulated meeting setup.

### Notes
- All recordings are provided in `.wav` format.
- Raw radar signals are not shared — no radar signal processing expertise is needed.
- The dataset is split into training, development, and test sets.
- Registered participants will receive access.

---

## Evaluation

Submissions will be evaluated using four standard metrics:

- **PESQ** – Perceptual Evaluation of Speech Quality  
- **ESTOI** – Extended Short-Time Objective Intelligibility  
- **DNSMOS** – Deep Noise Suppression Mean Opinion Score  
- **MFCC Cosine Similarity**  

Each difficulty level contributes a weighted score:
- Easy: 25%
- Medium: 35%
- Hard: 40%

Top-5 teams will be invited to present their work at ICASSP 2026.

---

## Baseline

Baseline deep learning models implemented in PyTorch will be provided to help participants kickstart their solutions. These include:

- Spectral mapping networks  
- Phase-aware enhancement techniques  
- Feature extraction and post-processing tools

📦 **Release date**: September 07, 2025

---

## Participation Guidelines

To ensure fairness and reproducibility:

- Use only the provided dataset — external data or augmentation is not allowed.
- Train models from scratch (no pre-trained or fine-tuned models).
- Max 300 training epochs allowed.
- Submit code, trained weights, and environment (Docker or requirements file).
- Participants retain all intellectual property rights.

---

## Timeline

- 📅 **Registration Opens**: September 07, 2025  
- 📂 **Dataset & Baseline Release**: September 07, 2025  
- 🧪 **Submission Deadline**: November 14, 2025  
- 🏆 **Ranking Announcement**: November 24, 2025  
- ✍️ **2-page Papers (invite only)**: December 07, 2025  
- ✅ **Paper Acceptance Notification**: January 11, 2026  
- 📌 **Camera-ready Deadline**: January 18, 2026

---

## Organizers

<table>
  <tr>
    <td align="center">
      <img src="/assets/images/organizers/andy.png" width="140"><br>
      <strong>Andy W. H. Khong</strong><br>NTU Singapore (Chair)
    </td>
    <td align="center">
      <img src="/assets/images/organizers/naylor.png" width="140"><br>
      <strong>Patrick A. Naylor</strong><br>Imperial College London (Co-chair)
    </td>
    <td align="center">
      <img src="/assets/images/organizers/zhiwei.png" width="140"><br>
      <strong>Zhi-Wei Tan</strong><br>NTU Singapore
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="/assets/images/organizers/reju.png" width="140"><br>
      <strong>V. G. Reju</strong><br>NTU Singapore
    </td>
    <td align="center">
      <img src="/assets/images/organizers/ritesh.png" width="140"><br>
      <strong>Ritesh C. Tewari</strong><br>NTU Singapore
    </td>
    <td align="center">
      <img src="/assets/images/organizers/ruotong.png" width="140"><br>
      <strong>Ruotong Ding</strong><br>NTU Singapore
    </td>
  </tr>
</table>


---

## Contact

📧 For inquiries, email us at: **rase_challenge@ntu.edu.sg**

---

_Last updated: August 5, 2025_
