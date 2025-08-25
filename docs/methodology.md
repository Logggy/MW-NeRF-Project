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

![Example Images](https://raw.githubusercontent.com/Logggy/MW-NeRF-Project/main/assets/combined_datasets_no_colorbars.png)

## MW-NeRF Approach
MW-NeRF adds a new network to the traditional NeRF architecture dedicated to learning a color representation for a scene at an additional wavelength. This gives us two learned color representations, which both share the same underlying learned shape model for whatever is present in a scene. In the MW-NeRF paper we train on Optical and Infrared data, where the infrared is guaranteed to possess the shape information required to complete the shape model, since the visible data cannot on its own.

![MW-NeRF Pipeline](https://raw.githubusercontent.com/Logggy/MW-NeRF-Project/main/assets/mwnerfsat.png)

Training on the same optical data alongside IR data gives us accurate learned visual representations, with complete shape models.

![MW-NeRF Side-by-side Results](https://raw.githubusercontent.com/Logggy/MW-NeRF-Project/main/assets/hubble_ir_triplets.png)
