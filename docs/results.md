---
layout: page
title: Results
nav_order: 3
---

## Plotting Conventions

All training data was arranged in a spherical grid surrounding the object being depicted in each scene. We have chosen to display the metrics calculated between each of these images and their NeRF renderings on two polar plots for the northern and southern hemispheres of this grid. The layout of the training images are shown here: 

![MW-NeRF Side-by-side Results](https://raw.githubusercontent.com/Logggy/MW-NeRF-Project/main/assets/TrainingSet.png)

For the final metric polar plots, we interpolate between each of these points to get smooth heatmaps depicting the performance of the model at each point.

## Total Intensity Percent Error and Structural Similarity Index Measure Results

### Vis-only Training

![MW-NeRF Side-by-side Results](https://raw.githubusercontent.com/Logggy/MW-NeRF-Project/main/assets/hubble_percent.png)

![MW-NeRF Side-by-side Results](https://raw.githubusercontent.com/Logggy/MW-NeRF-Project/main/assets/hubble_ssim.png)

### MW-NeRF Model

![MW-NeRF Side-by-side Results](https://raw.githubusercontent.com/Logggy/MW-NeRF-Project/main/assets/hubble_ir_percent.png)

![MW-NeRF Side-by-side Results](https://raw.githubusercontent.com/Logggy/MW-NeRF-Project/main/assets/hubble_ir_ssim.png)

### Results discussion

Please consult the paper for more in-depth discussion on results and metrics. The comparison presented here describes current percent-error difficulties in shadowed regions, while showing that structural similarity in these regions still performs very well. This shows that while NeRFs may struggle in shadowed regions with percent error analysis, human eye observations of the compared outputs would identify that they look very much the same.

**Summary**: MW-NeRF shows improved completeness and stability over visible-only NeRFs in shadowed scenes.
