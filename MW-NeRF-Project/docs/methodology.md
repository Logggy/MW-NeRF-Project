---
layout: page
title: Methodology
nav_order: 2
---

## Dataset
- Hubble model
- 614 images per distance
- 5 distances (50 m–1 km)
- 1 illumination angle

## Baselines & Observations
- **SfM**: fast but discontinuous; holes in geometry.
- **SPC**: excellent quality but requires lots of data and time.
- **Vanilla NeRF**: good quality/low data, but diverges in shadows → incomplete shape.

## MW-NeRF Approach
- Multi-wavelength input channels (e.g., visible + other bands)
- Training objective emphasizes structural consistency in low-light regions
- Stable learning under varying illumination
