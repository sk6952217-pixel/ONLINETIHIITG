# Shortlisted Candidates

## Objective

The objective was to compare all implemented enhancement methods and shortlist the strongest candidates for deeper experiments.

## Methods Compared

- Histogram Equalization
- CLAHE
- Gamma Correction
- White Balance
- Refined CLAHE-3
- CNN

## Comparison Summary

| Method | PSNR | SSIM | Edge F1 |
|---|---:|---:|---:|
| Histogram Equalization | 8.0800 | 0.2225 | 0.0573 |
| CLAHE | 10.9900 | 0.4346 | 0.0572 |
| Gamma Correction | 10.9300 | 0.4821 | 0.0416 |
| White Balance | 10.4400 | 0.4611 | 0.0416 |
| Refined CLAHE-3 | 11.4000 | 0.3995 | 0.0688 |
| CNN | 14.4692 | 0.5619 | 0.0259 |

UIQM/UCIQE values were not available in the current comparison results.

## Shortlisted Candidate 1: CNN

CNN achieved:

- PSNR = 14.4692
- SSIM = 0.5619
- Edge F1 = 0.0259

CNN achieved the highest PSNR and SSIM among the compared methods.

Therefore, CNN is shortlisted as the primary learning-based candidate for deeper experiments.

## Shortlisted Candidate 2: Refined CLAHE-3

Refined CLAHE-3 achieved:

- PSNR = 11.4000
- SSIM = 0.3995
- Edge F1 = 0.0688
- Clip Limit = 3.0
- Tile Grid Size = 8×8

It achieved the highest Edge F1 among the compared methods and provides a strong classical reference.

## Limitations

- Dataset V1 contains 312 valid paired images.
- The dataset may not represent all underwater scene conditions.
- Different metrics provide different rankings.
- CNN has higher computational complexity than classical methods.
- Edge F1 for CNN is lower than the classical candidates.

## Final Shortlist

1. CNN – Primary learning-based candidate
2. Refined CLAHE-3 – Classical reference candidate

## Conclusion

CNN and Refined CLAHE-3 are shortlisted for deeper experiments. CNN provides the strongest PSNR and SSIM results, while Refined CLAHE-3 provides the strongest edge-preservation result.
