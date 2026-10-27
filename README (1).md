# Final Model / Pipeline Freeze

## Final Model

The CNN was selected as the final model based on validation results, robustness analysis and overall reconstruction quality.

The Refined CLAHE-3 method is retained as the classical reference.

## Final Results

| Method | PSNR | SSIM | Edge F1 |
|---|---:|---:|---:|
| Refined CLAHE-3 | 11.40 | 0.3995 | 0.0688 |
| CNN | 14.4692 | 0.5619 | 0.0259 |

## Selection Rationale

CNN was selected because it achieved the highest PSNR and SSIM among the tested methods.

Refined CLAHE-3 achieved better edge preservation, so it is retained as the classical reference for comparison.

The final selection therefore considers overall reconstruction quality while keeping the classical method as a reference for structural preservation.

## Frozen Pipeline

Dataset: Dataset V1

Total valid pairs: 312

Train: 218

Validation: 47

Test: 47

Image size: 256 × 256

Channels: 3

Evaluation metrics:
- PSNR
- SSIM
- Edge F1

The train, validation and test split is frozen and will not be changed during final evaluation.

## Saved Artefacts

- `final_CNN_model.pth` - final trained CNN model
- `final_pipeline_config.json` - frozen pipeline configuration
- Final CNN outputs
- Final comparison results

## Reproducibility

The same Dataset V1, preprocessing, frozen split and evaluation metrics will be used for the final evaluation.

No changes will be made to the test set before final reporting.

## Final Decision

**Final Model: CNN**

**Classical Reference: Refined CLAHE-3**

The pipeline is now frozen for the final evaluation and reporting stage.
