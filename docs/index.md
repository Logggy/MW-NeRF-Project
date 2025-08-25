---
layout: home
title: Motivation
nav_order: 1
---
# What is MW-NeRF?

MW-NeRF extends Neural Radiance Fields (NeRFs) to handle **complex lighting and shadows** in **space-based imagery** for spacecraft modeling and reconstruction.

- **Why**: Collision avoidance and risk assessment need fast, lightweight, and accurate shape models.
- **Problem**: Vanilla NeRFs struggle in **shadows**, leading to incomplete reconstructions.
- **Our solution**: **Multi-Wavelength training** → robust features, complete geometry, stable learning.

# Typical NeRF Training Results

NeRFs, on their own, struggle to learn scenes with very complex lighting. In space-based environments, this is extremely clear, as we often get single direct light sources that cast sharp and complete shadows. NeRFs can still train on the visible parts, but this does not completely save us in every aspect of training, since NeRFs learn both visible representations of a scene and the underlying density/shape models occupying them. This can give us successful visual representations!

![Vanilla NeRF Hubble Model](https://raw.githubusercontent.com/Logggy/MW-NeRF-Project/main/assets/nerfanim.mp4)

While failing to learn a full underlying shape model.

![NeRF Outputs Compared to Ground Truth Images](https://raw.githubusercontent.com/Logggy/MW-NeRF-Project/main/assets/hubble_all_50.0m_combined_triplets.pdf)

There's no reason why we should be able to get these shape models by default: the training dataset simply lacks the information to teach the NeRF about what exists in these shadows. MW-NeRF solves this by incorporating data from multiple wavelengths to provide the NeRF with better information where a single wavelength may be lacking.

Explore:
- [Methodology](./methodology.md)
- [Results](./results.md)
- [Contact](./contact.md)
