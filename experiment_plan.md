#  Experiment Plan

## Project
Underwater Image Enhancement

## Baseline Methods

### 1. CLAHE
Used as a classical enhancement baseline.

### 2. Gamma Correction
Used to improve brightness and contrast.

### 3. White Balance
Used to reduce underwater color distortion.

### 4. Histogram Equalization
Used to enhances global contrast by redistributing pixels intensity values across the full available  range.

## Advanced Method

### CNN Image-to-Image Enhancement

A CNN-based model will learn the mapping from a degraded underwater input image to its corresponding target image.

## Project-Specific Experiments

- Compare classical methods with CNN.
- Tune CNN parameters.
- Study model performance under different settings.
- Perform robustness and ablation experiments.
- Compare the final method with the strongest classical baseline.

## Evaluation Criteria

- PSNR
- SSIM
- Edge F1 / Edge Preservation
- Processing Time
- UIQM / UCIQE where applicable
- Visual comparison

## Experimental Rule

The same verified dataset split should be used for fair comparison between methods.

The test set should remain fixed for final evaluation.
