---
layout: page
title: Research
permalink: /research/
description: Research interests and current projects in computational imaging.
nav: true
nav_order: 2
---

My research focuses on computational imaging, with particular interests in lensless imaging, inverse problems, and three-dimensional reconstruction. I am interested in combining physical image formation with computational reconstruction to recover information that is difficult to obtain directly using conventional imaging systems.
{: .research-overview}

<section class="research-direction" markdown="1">

## Depth-Aware Lensless Imaging

My recent research explores how depth-dependent image formation can be exploited and modeled for three-dimensional lensless imaging. This direction includes both inverse reconstruction from depth-encoded measurements and the physical modeling of continuously varying depth-dependent point spread functions.

<div class="research-work" markdown="1">

<figure class="research-visual">
  <!-- Replace this labeled space with a verified representative figure and caption. -->
  <div class="figure-placeholder">
    <span>Representative figure</span>
    <span class="placeholder-note">To be added.</span>
  </div>
</figure>

<div class="research-work-text" markdown="1">

### Continuous-Depth PSF Modeling

_Aug. 2026 – Present_

Most lensless 3D imaging models represent continuous scenes using a finite set of discretely calibrated PSFs. My current work investigates how measured PSFs evolve continuously along the axial dimension, including systematic spatial scaling, corresponding spectral variation, and depth-dependent spatial shifts. The goal is to develop a more continuous description of depth-dependent image formation and reduce the mismatch between discrete calibration models and real scenes.

</div>
</div>

<div class="research-work" markdown="1">

<figure class="research-visual">
  <!-- Replace this labeled space with a verified representative figure and caption. -->
  <div class="figure-placeholder">
    <span>Representative figure</span>
    <span class="placeholder-note">To be added.</span>
  </div>
</figure>

<div class="research-work-text" markdown="1">

### Single-Shot Lensless 3D Reconstruction

_Sept. 2025 – Present_

This work investigates joint reconstruction of an all-in-focus image and scene depth from a single lensless measurement. A physics-constrained layered scene representation jointly models scene intensity and depth allocation, while calibrated depth-dependent PSFs map the reconstructed scene back to the sensor domain. Measurement consistency directly constrains the recovered scene, with additional regularization used to refine the image-depth decomposition.

</div>
</div>

</section>

<section class="research-direction" markdown="1">

## Low-Light Lensless Imaging

Low-light conditions make lensless reconstruction particularly challenging because measurement noise can strongly interfere with computational inversion and per-measurement optimization.

### Unsupervised Lensless Reconstruction in Low-Light Conditions

_Mar. 2025 – Sept. 2025_

This work investigates unsupervised lensless reconstruction under low-SNR measurements. Local–global structural consistency and adaptive partial convolution are used to preserve image structure while reducing the influence of noise-dominated regions, while geometric equivariance encourages transformation-consistent reconstruction.

**Representative Publication:**

Zeyu Chang\*, Tianjiao Zeng, Xiaoling Zhang. “Unsupervised Lensless Image Reconstruction Driven by Structure Consistency Modeling in Low-Light Scenarios.” Fifth International Computational Imaging Conference (CITA 2025), Proc. SPIE 14000, 1400022, 2026.

</section>
