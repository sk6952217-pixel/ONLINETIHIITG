# Day 21 - Best Candidate Review

## Objective
Review the baseline and tuned results, compare the best candidates, and identify successes, failures, and remaining weaknesses.

## Final Comparison

| Method | PSNR | SSIM | Edge F1 |
|---|---:|---:|---:|
| CLAHE Baseline | 10.99 | 0.4346 | 0.0572 |
| Refined CLAHE-3 | 11.40 | 0.3995 | 0.0688 |
| CNN | 14.4692 | 0.5619 | 0.0259 |

## Key Findings

- CNN achieved the highest PSNR and SSIM.
- Refined CLAHE-3 achieved the highest Edge F1 among the tested methods.
- CNN improved PSNR and SSIM compared with the classical methods.
- Refined CLAHE-3 provided better edge preservation than CNN.
- CLAHE parameter tuning improved PSNR and Edge F1 but reduced SSIM.

## Success and Failure Analysis

Representative validation images were reviewed using:
- Input image
- CNN enhanced output
- Target image

The success cases show improved brightness and overall image reconstruction.

The difficult cases show that the CNN can still have problems with structural details and edge preservation.

## Remaining Weaknesses

- CNN has lower edge preservation than the classical reference.
- The prepared Dataset V1 contains only 312 valid input-target pairs.
- The learning-based model may be affected by the limited dataset size.
- CLAHE tuning shows a trade-off between PSNR, SSIM, and edge preservation.
- Evaluation is mainly based on PSNR, SSIM, and Edge F1.

## Best Candidate

### Primary Candidate: CNN
Reason:
- Highest PSNR: 14.4692
- Highest SSIM: 0.5619
- Better overall reconstruction quality.

### Classical Reference: Refined CLAHE-3
Reason:
- Best classical PSNR: 11.40
- Highest Edge F1: 0.0688
- Strong edge preservation.

## Week-4 Final Direction

The CNN will be considered the primary final candidate for underwater image enhancement.

Refined CLAHE-3 will be retained as the classical reference method.

Final evaluation will focus on:
- PSNR
- SSIM
- Edge F1
- Visual quality
- Success and failure cases

## Mentor Approval Required

Please confirm the final Week-4 direction:  Approved

**CNN as the primary final candidate and Refined CLAHE-3 as the classical reference.**
