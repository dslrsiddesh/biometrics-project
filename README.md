# Finger Nails as Transient Biometrics

This repository contains the implementation and experiments for the course project
**"Finger Nails as Transient Biometrics"**, carried out as part of the
*Introduction to Biometrics* course.

The work investigates fingernail images as a **transient biometric trait**, where
the biometric signature naturally changes over time, addressing privacy concerns
associated with permanent biometric identifiers.

---

## Problem Statement

Traditional biometric systems rely on permanent traits such as fingerprints and iris,
which can lead to long-term privacy risks if compromised. This project explores the
idea of **transient biometrics**, focusing on fingernails whose appearance changes
over a short duration due to natural growth.

---

## Methodology

The biometric pipeline implemented in this project consists of:

- **Preprocessing**
  - Fingernail region detection and normalization
  - Resizing to a fixed resolution

- **Feature Extraction**
  - Local Binary Patterns (LBP) for texture-based representation
  - SIFT and BRISK descriptors for keypoint-based features

- **Matching**
  - Histogram-based cosine similarity for LBP features
  - Nearest-neighbor matching for SIFT/BRISK descriptors

- **Score Fusion**
  - Geometric mean fusion of LBP, SIFT, and BRISK match scores

---

## Dataset

- Transient Biometrics Nails Dataset (TBND)
- Fingernail images from multiple subjects
- Images captured across different time intervals (same day, next day, one month)

---

## Evaluation

- Verification experiments performed across short-term and long-term intervals
- Majority of subjects (~79.6%) show reduced matching scores over longer intervals
- Results validate fingernails as a transient biometric trait

---

## Results Summary

- Fingernail patterns exhibit noticeable changes within a short time span
- Matching performance degrades over longer intervals
- Supports the feasibility of privacy-preserving transient biometrics

