#  Software Performance / Final Validation

## Objective

- Measure CNN inference time and model size.
- Perform final validation on the frozen test set.
- Compare the final CNN with the strongest simple baseline, Refined CLAHE-3.
- Record quality versus computational complexity.

## Frozen Validation Setup

- Dataset: Dataset V1
- Test images: 47
- Image size: 256 × 256
- Final model: CNN
- Classical baseline: Refined CLAHE-3
- Metrics: PSNR, SSIM and Edge F1

The test set was kept separate from training and parameter selection.

## Conclusion

The final CNN was evaluated on the held-out test set using the frozen Dataset V1 pipeline. PSNR, SSIM and Edge F1 were calculated to measure reconstruction quality and edge preservation. CNN inference time and model size were also measured to evaluate computational complexity.

The final CNN was compared with Refined CLAHE-3, the strongest simple classical reference. The comparison shows that the CNN provides stronger overall reconstruction quality, while Refined CLAHE-3 has better edge preservation and lower computational complexity.

Therefore, the final results show a quality-versus-complexity trade-off between the learning-based CNN and the classical enhancement method.
