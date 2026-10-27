# Day 14 – Week-2 Peer Visual Comparison

##  Objective

The objective of Day 14 was to compare the outputs of classical image enhancement methods visually and quantitatively, discuss artifacts and difficult scenes, record peer observations, and prepare the Week-2 project package.

The classical enhancement methods compared were:

- CLAHE
- Gamma Correction
- White Balance

The comparison was performed using the prepared Dataset V1 and corresponding target images.

##  Classical Methods Compared

### CLAHE

CLAHE (Contrast Limited Adaptive Histogram Equalization) improves local image contrast and visibility, especially in dark and low-contrast regions.

### Gamma Correction

Gamma Correction adjusts image brightness using a nonlinear transformation and can improve the visibility of dark regions.

### White Balance

White Balance attempts to correct color and illumination imbalance in underwater images.

##  Quantitative Comparison

The classical baseline methods were evaluated using PSNR and SSIM.

| Method | PSNR | SSIM |
|---|---:|---:|
| CLAHE | 10.99 | 0.4346 |
| Gamma Correction | 10.93 | 0.4821 |
| White Balance | 10.44 | 0.4611 |

### Observations

- CLAHE achieved the highest PSNR of 10.99.
- Gamma Correction achieved the highest SSIM of 0.4821.
- White Balance achieved the lowest PSNR of 10.44.
- Classical methods provided some improvement but did not completely reproduce the quality of the target images.

##  Visual Comparison

A representative visual comparison was created using:

- Input image
- Target image
- CLAHE output
- Gamma Correction output
- White Balance output

### Visual Observations

- The input image has low visibility and poor illumination.
- The target image is clearer and provides better visibility of objects and scene details.
- CLAHE improves local contrast and makes some details more visible.
- Gamma Correction provides a small brightness improvement.
- White Balance provides limited visual improvement in severely degraded images.

##  Difficult Scenes

The difficult conditions identified during the Dataset V1 EDA included:

- Very dark images
- Low-contrast images
- Poorly illuminated scenes
- Scenes where object details are difficult to distinguish
- Images where enhancement may introduce unwanted texture or artifacts

Representative difficult scenes were selected for visual comparison.

##  Artifact Analysis

### CLAHE

- Improves local contrast.
- May increase unwanted texture or noise in dark regions.
- Can produce an uneven appearance in some areas.

### Gamma Correction

- Improves brightness.
- May provide limited detail recovery.
- Some dark regions can remain difficult to see.

### White Balance

- Attempts to correct color and illumination.
- May provide limited improvement in severely dark scenes.
- Does not directly recover missing image details.

##  Peer Visual Comparison

The outputs were compared visually with peers without sharing implementation code.

The comparison focused on:

- Overall brightness
- Object visibility
- Contrast improvement
- Detail preservation
- Artifacts
- Similarity to the target
- Performance on difficult scenes

### Peer Observations

- CLAHE provides stronger local contrast improvement.
- Gamma Correction provides a relatively natural brightness improvement.
- White Balance provides limited improvement in severely degraded scenes.
- Very dark images remain difficult for all three methods.
- No classical method consistently matches the clarity of the target images.

Actual peer comments can be added after the peer discussion.

##  Peer Insight

The visual comparison indicates that classical enhancement methods can improve certain aspects of underwater images, but their ability to recover hidden details is limited.

CLAHE is useful for improving local contrast, while Gamma Correction mainly provides brightness adjustment. White Balance mainly addresses illumination and color balance.

Heavily degraded underwater scenes remain challenging for all three methods.

##  Hypothesis

Based on the visual and quantitative comparison, the following hypothesis was recorded:

Classical enhancement methods may work well for mild degradation, but heavily dark and low-contrast underwater images may require a learning-based image-to-image enhancement method to recover details while preserving important edges and structures.

This hypothesis will guide the next stage of the project.

##  Classical Baseline Selection

The current quantitative results show:

- Best PSNR: CLAHE — 10.99
- Best SSIM: Gamma Correction — 0.4821
- Lowest PSNR: White Balance — 10.44

The final classical reference should be selected using:

1. PSNR
2. SSIM
3. Edge similarity/preservation
4. Visual quality
5. Artifact level

The edge-preservation results will be included separately in the Day 13 baseline results.

##  Week-2 Package Structure

```text
Week-2_Package/
│
├── Day13_Classical_Baseline/
│   ├── classical_baseline.ipynb
│   ├── baseline_metrics.csv
│   └── edge_metrics.csv
│
├── Day14_Visual_Comparison/
│   ├── visual_comparison.png
│   └──  difficult_scenes.png
│
└── README.md
```

## 12. File Description

### classical_baseline.ipynb

Contains the implementation and evaluation of the classical enhancement methods.

### baseline_metrics.csv

Contains the PSNR and SSIM results for CLAHE, Gamma Correction, and White Balance.

### edge_metrics.csv

Contains the edge extraction and edge-preservation measurements for the classical enhancement methods.

### visual_comparison.png

Contains a visual comparison of the input, target, CLAHE, Gamma Correction, and White Balance outputs.

### difficult_scenes.png

Contains representative difficult images identified during the image-quality analysis.

### peer_comparison.md

Contains the peer observations, artifact discussion, insights, and hypothesis from the Week-2 comparison.

##  Key Findings

1. Classical methods provide some improvement over degraded input images.
2. CLAHE produced the highest PSNR.
3. Gamma Correction produced the highest SSIM.
4. White Balance produced the lowest PSNR.
5. Very dark and low-contrast scenes remain challenging.
6. CLAHE can improve local visibility but may enhance unwanted texture.
7. Gamma Correction mainly improves brightness and may not recover hidden details.
8. White Balance provides limited improvement for severely degraded images.
9. Visual comparison is important because numerical metrics alone do not fully describe image quality.
10. A stronger image-to-image enhancement approach may be required for difficult underwater scenes.

##  Week-2 Progress

The following activities were completed:

- Classical enhancement baselines implemented.
- CLAHE evaluated.
- Gamma Correction evaluated.
- White Balance evaluated.
- PSNR calculated.
- SSIM calculated.
- Representative outputs visually compared.
- Difficult scenes identified.
- Artifact observations recorded.
- Peer comparison prepared.
- Week-2 package structure prepared.

##  Conclusion

Day 14 completed the Week-2 peer visual comparison of classical underwater image enhancement methods.

The comparison combined quantitative metrics, visual inspection, difficult-scene analysis, artifact discussion, and peer observations.

The results indicate that classical enhancement methods are useful as baseline references but have limitations when dealing with severely degraded underwater images.

The findings and hypothesis from this comparison will be used to guide the next stage of model development.
