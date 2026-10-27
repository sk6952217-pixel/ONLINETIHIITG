# Final Technical Review

## Objective

The objective of Day 24 was to present the final project method, validation results and complete input-to-output workflow to the mentor. The purpose was also to confirm the remaining error-analysis and reporting requirements and record the mentor's corrections.

## Final Method

- Final learning-based method: CNN
- Classical reference: Refined CLAHE-3
- Dataset: Dataset V1
- Total paired images: 312
- Train: 218
- Validation: 47
- Test: 47
- Image size: 256 × 256 RGB
- Evaluation metrics: PSNR, SSIM and Edge F1

## Final Results

| Method | PSNR | SSIM | Edge F1 |
|---|---:|---:|---:|
| Refined CLAHE-3 | 10.8626 | 0.4217 | 0.0656 |
| CNN | 14.2688 | 0.5517 | 0.0377 |

## Final Workflow

Raw Underwater Images
→ Quality Check
→ Duplicate Check
→ Input-Target Pairing
→ Dataset V1
→ Frozen Train/Validation/Test Split
→ Preprocessing
→ CNN Training
→ CNN Inference
→ Enhanced Output
→ PSNR + SSIM + Edge F1
→ Final Comparison

## Main Findings

- CNN achieved higher PSNR and SSIM than Refined CLAHE-3.
- Refined CLAHE-3 achieved higher Edge F1.
- CNN provides better overall reconstruction quality.
- CLAHE-3 provides stronger edge preservation.
- The results show a trade-off between image quality and structural preservation.
- The final pipeline and dataset split were kept fixed for reproducibility.
