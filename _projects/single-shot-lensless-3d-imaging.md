---
layout: page
title: Single-shot Lensless 3D Imaging
description: Joint image and depth reconstruction from a single lensless measurement.
permalink: /research/single-shot-lensless-3d-imaging/
published: true
nav: false
related_publications: false
---

## Overview

This project studies the joint reconstruction of an all-in-focus image and a depth map from a single lensless measurement. A lensless measurement multiplexes scene information from different depths through depth-dependent point spread functions (PSFs), providing depth cues while making the inverse problem highly ill-posed. The goal is to recover both image appearance and scene depth while explicitly respecting the physical image-formation model.

## Motivation

Lensless cameras encode scene information through a mask or diffuser instead of conventional imaging optics. Because the PSF changes with object depth, a single sensor measurement contains depth-dependent information, but contributions from multiple depths remain coupled. Neighboring-depth PSFs can also be highly correlated, making image-depth separation difficult, while directly predicting an image and depth map does not necessarily ensure consistency with the physical forward model.

## Approach

Rather than directly predicting only an all-in-focus image and a depth map, the scene is represented through an intensity representation and a depth-probability representation. A shared encoder and two decoders parameterize these representations, which are combined through a differentiable scene-formation process to form depth-wise scene components. The components are propagated through their corresponding depth-dependent PSFs and summed to synthesize a sensor measurement, which is constrained to agree with the observation. The final image and depth map are derived from the same intermediate scene representation.

> **Figure 1 placeholder:** Method / imaging pipeline.

## Forward Model

$$
y = \sum_k h_k \ast x_k + n
$$

Here, $y$ is the sensor measurement, $h_k$ is the depth-dependent PSF for depth plane $k$, $x_k$ is the scene component at that plane, and $n$ represents measurement noise.

## Key Ideas

- **Physics-constrained scene formation:** The intermediate scene representation is mapped back to the sensor domain through the calibrated depth-dependent forward model.
- **Joint image-depth representation:** The image and depth map are derived from the same scene representation rather than estimated as unrelated outputs.
- **Self-supervised reconstruction:** Optimization is driven by measurement consistency without requiring paired image-depth training data.

## Regularization

Entropy regularization encourages concentrated depth-probability distributions. Semantic or structural regularization uses reconstructed image structure to provide additional guidance for depth estimation; these terms serve as supporting constraints for the reconstruction.

## Results

### Simulation

Representative quantitative and qualitative results will be added here.

> **Figure 2 placeholder:** Simulation reconstruction comparison.

### Real Prototype

Representative quantitative and qualitative results will be added here.

> **Figure 3 placeholder:** Real prototype reconstruction.

### Ablation

Representative quantitative and qualitative results will be added here.

## Relation to My Research

This work is part of a broader interest in computational imaging and computational optics, particularly the use of physical forward models and computational reconstruction to extract information from compact optical systems.
