##  Research Insight

The robustness and ablation analysis compared classical enhancement with the learning-based CNN and examined the effect of CLAHE parameter refinement.

The CNN achieved the highest PSNR (14.4692) and SSIM (0.5619), showing better overall similarity to the target images than the classical methods.

However, Refined CLAHE-3 achieved a higher Edge F1 score (0.0688) than the CNN (0.0259). This indicates that better PSNR and SSIM do not necessarily mean better edge preservation.

The CLAHE ablation showed that parameter refinement improved PSNR from 10.99 to 11.40 and Edge F1 from 0.0572 to 0.0688, while SSIM decreased from 0.4346 to 0.3995.

Therefore, the experiments suggest that learning-based enhancement provides better overall image reconstruction quality, while classical CLAHE can preserve structural edges better. This shows a trade-off between overall image similarity and edge preservation.
