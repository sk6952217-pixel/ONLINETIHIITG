# Updated Experiment Plan

## Stage 1 - Dataset Preparation

- Verify input-target pairs.
- Remove incorrect pairs.
- Check duplicates and image quality.
- Prepare the final dataset split.

## Stage 2 - Classical Baselines

Run:

1. CLAHE
2. Gamma Correction
3. White Balance
4. Histogram Equalization

Record:

- PSNR
- SSIM
- Edge F1
- Processing Time
- Visual results

## Stage 3 - CNN Model

Train the CNN using paired input-target images.

Record:

- Training loss
- Validation loss
- PSNR
- SSIM
- Edge F1
- Processing time

## Stage 4 - Model Refinement

Experiment with selected CNN parameters and compare the results.

## Stage 5 - Robustness / Ablation

Study the effect of selected model components or parameters.

## Stage 6 - Final Evaluation

Compare the final CNN with the strongest classical baseline using the same test set.

Metrics:

- PSNR
- SSIM
- Edge F1
- Processing Time
- UIQM/UCIQE where applicable
- Visual comparison

## Stage 7 - Error Analysis

Inspect difficult and failed cases and document recurring failure patterns.

## Fair Comparison Rules

- Use the same test set.
- Use the same evaluation metrics.
- Keep input-target pairs together.
- Do not use test images for training or tuning.
- Record all important parameters and results.
