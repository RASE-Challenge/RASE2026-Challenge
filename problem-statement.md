---
title: Problem Statement
layout: single
permalink: /problem-statement/
---

The **Radar Acoustic Speech Enhancement (RASE) Challenge 2026** focuses on reconstructing intelligible, full-bandwidth speech from signals captured using mmWave radar. The figures below illustrate the two main data scenarios in this challenge and highlight the difficulty of the task.

**Figures 1 and 2** show four panels comparing clean speech (left) with radar-captured speech (right) for two different scenarios.

---

## Figure 1: Direct Diaphragm Vibration (Task 1)

The left plots show the waveform and spectrogram of the clean reference speech played through a loudspeaker. The right plots show the corresponding radar-captured signal obtained by sensing the **direct vibration of the loudspeaker diaphragm**. While speech content is clearly visible in the clean spectrogram, the radar signal appears noisier and exhibits a limited bandwidth. This represents the **simpler case**, where the radar has a strong vibrating source.

<figure>
  <img src="{{ '/assets/images/rase_fig1.png' | relative_url }}"
     alt="Figure 1: Clean vs radar-captured speech for direct diaphragm vibration (waveform and spectrogram)">
  <figcaption><strong>Figure 1.</strong> Direct diaphragm vibration (Task 1): clean (left) vs radar-captured (right).</figcaption>
</figure>

---

## Figure 2: Secondary Surface Vibration (Task 2)

The left plots again show the clean speech waveform and spectrogram, but here the radar senses vibrations from a **thin aluminium foil** placed near the loudspeaker. The radar-captured signal (right) is significantly more noisy, and speech components in the spectrogram are almost buried under the noise floor. This represents the **more challenging case**, where speech must be recovered from very weak, indirect surface vibrations.

<figure>
  <img src="{{ '/assets/images/rase_fig2.png' | relative_url }}"
     alt="Figure 2: Clean vs radar-captured speech for secondary surface vibration (waveform and spectrogram)">
  <figcaption><strong>Figure 2.</strong> Secondary surface vibration (Task 2): clean (left) vs radar-captured (right).</figcaption>
</figure>

---

## Core Challenge

These examples highlight the core difficulty of RASE 2026: **transforming noisy, band-limited radar signals into natural-sounding, intelligible speech**. Participants are expected to design signal-processing and machine-learning models that enhance radar-captured signals and reconstruct high-quality speech suitable for human listening and downstream speech tasks.
