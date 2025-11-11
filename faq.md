---
layout: single          # or "default" / whatever your theme uses
title: "FAQ"
permalink: /faq/
author_profile: false
toc: true
---

# Frequently Asked Questions

## Who can participate in the RASE 2026 Challenge?
Anyone from academia or industry with interest in speech enhancement, radar sensing, or machine learning is welcome to participate.

## How do I register?
Please use the registration form linked on the main page under the **Timeline** section.

## When will the dataset and baseline be released?
The data and baseline are scheduled to be released on **September 20, 2025**.

## Are we allowed to use external data?
No. As stated in the Participation Guidelines, only the provided dataset may be used. External data or augmentation is not allowed.

## How will submissions be evaluated?
Submissions are evaluated using PESQ, ESTOI, DNSMOS, and MFCC cosine similarity, with difficulty-weighted scoring (40% easy, 60% hard).

## Who should I contact for more questions?
You can email the organizers at **rase-challenge@ntu.edu.sg**.

## Can we modify files beyond src/models/, src/config/, and train.py (e.g., datamodule.py for extra preprocessing/augmentation)?

Short answer: It’s discouraged.

Details: The organizers would likeinnovation to focus on deep learning architecture, not on additional preprocessing or data augmentation. Prioritize changes to your model definition and configuration over data-pipeline tweaks.

## Are there constraints on model size?

Short answer: Yes, by compute/time.

Details: Your model must (a) run on a single RTX 6000 Ada (48 GB) and (b) finish testing within 6 hours. It’s recommended to validate your setup on the official platform—if it passes there, it will pass during the test phase.

## Is a two-stage training strategy allowed (stage 1 trains a model, save checkpoint; stage 2 initializes from that checkpoint and continues training)?

Short answer: Allowed with conditions.

Details:

Data restriction: Both stages must be trained only on the official challenge dataset (fairness/consistency).

Training budget: The total training across stages must be < 300 epochs.

Reporting: For publications, include ablation studies showing why the two-stage approach beats training from scratch.

## Is the submission procedure different for the test phase?

Short answer: No.

Details: The test submission follows the same procedure as validation (e.g., results & metadata upload flow).

## Is it allowed to create additional degraded data (e.g., by adding Gaussian noise to clean voice samples) for training or evaluation?

Short answer: No.

Details: Creating any additional degraded data, including by adding Gaussian noise or other distortions to clean voice samples, is considered data augmentation and is forbidden. Please focus solely on the machine learning and deep learning model design, training, and optimization using the provided data without generating new degraded variants.
