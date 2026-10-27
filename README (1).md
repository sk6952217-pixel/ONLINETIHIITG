# Day 10 – Visual EDA

## 1. Objective

The objective of Day 10 was to perform Exploratory Data Analysis (EDA) on the underwater image dataset.

The analysis focused on:

- Image quality
- Image distribution
- Image dimensions
- Brightness
- Contrast
- Representative image grids
- Difficult image conditions
- Degradation patterns

## 2. Dataset Statistics

The dataset contains three types of images:

- Input images: **1078**
- Target images: **1078**
- Generated images: **1078**

### Image Dimensions

- Width: **256 pixels**
- Height: **256 pixels**
- Image format: **PNG**

## 3. Image Quality Analysis

The input images were analyzed for brightness and contrast.

### Brightness Statistics

| Statistic | Value |
|---|---:|
| Number of input images | 1078 |
| Average brightness | 70.16 |
| Minimum brightness | 1.03 |
| Maximum brightness | 246.69 |

The brightness values show that the dataset contains images ranging from very dark to very bright conditions.

### Contrast Statistics

| Statistic | Value |
|---|---:|
| Average contrast | 26.68 |
| Minimum contrast | 2.19 |
| Maximum contrast | 73.32 |

The results show that some images have very low contrast, which may make image details difficult to distinguish.

## 4. Representative Raw-Data Grid

A visual grid was created to compare:

- Input images
- Target images
- Generated images

The grid helps visually inspect the differences between degraded input images and their corresponding target and generated images.

## 5. Difficult Samples

The darkest and lowest-contrast input images were identified using brightness and contrast statistics.

### 5.1 Five Darkest Input Images

| Brightness | Image |
|---:|---|
| 1.03 | `epoch_0110/img 58_input.png` |
| 2.69 | `epoch_0110/img 140_input.png` |
| 3.65 | `epoch_0110/img 57_input.png` |
| 4.07 | `epoch_0110/img 141_input.png` |
| 4.21 | `epoch_0110/img 59_input.png` |

### 5.2 Five Lowest-Contrast Input Images

| Contrast | Image |
|---:|---|
| 2.19 | `epoch_0096/img_22_input.png` |
| 2.19 | `epoch_0096/img_25_input.png` |
| 2.25 | `epoch_0096/img_23_input.png` |
| 2.47 | `epoch_0096/img_24_input.png` |
| 3.06 | `epoch_0096/img_14_input.png` |

## 6. Degradation Patterns

The EDA indicates the following degradation patterns:

### Darkness

Some input images have extremely low brightness values.

This indicates that low illumination is an important degradation condition in the dataset.

### Low Contrast

Some images have very low contrast values.

Low contrast can make objects and fine details difficult to distinguish from the background.

### Variable Illumination

The brightness range is large, from **1.03 to 246.69**.

Therefore, the enhancement method needs to handle different illumination conditions.

### Variable Contrast

The contrast range is from **2.19 to 73.32**.

This indicates that images have different levels of contrast and may require different levels of enhancement.

## 7. Observations

The visual inspection showed:

- Target images appeared clearer than input images.
- Generated images appeared closer to the target images.
- No major color difference was observed in the inspected samples.
- No noticeable blur or noise was observed.
- Important image details appeared to be preserved.
- Some input images were very dark.
- Some input images had very low contrast.

## 8. Difficult Condition Hypotheses

Based on the statistical and visual analysis, the following hypotheses were recorded:

1. Very dark images may be difficult to enhance because important details are less visible.

2. Low-contrast images may require stronger contrast enhancement.

3. The wide brightness range indicates that the model should handle different illumination conditions.

4. The wide contrast range indicates that enhancement performance may vary across different image conditions.

5. The enhancement method should improve visibility while preserving important image details.

## 9. EDA Workflow

```text
Dataset
   ↓
Image Statistics
   ↓
Brightness Analysis
   ↓
Contrast Analysis
   ↓
Representative Image Grid
   ↓
Difficult Sample Identification
   ↓
Degradation Pattern Analysis
   ↓
Hypothesis Formation
