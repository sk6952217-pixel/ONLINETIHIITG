#  Methodology V1

## Project Title
Underwater Image Enhancement Using Classical and Learning-Based Methods

## 1. Research Question

How effectively can underwater images be enhanced while maintaining image quality, structure, and important visual details?

## 2. Dataset

The project uses paired underwater images.

- Input: degraded underwater image
- Target: corresponding clearer/enhanced image
- Image format: PNG/JPG
- Images are converted to a consistent format and size during preprocessing.

Only verified input-target pairs are used.

## 3. Data Preparation

The following steps will be performed:

1. Check image files and dimensions.
2. Check input-target pairing.
3. Remove incorrect or unusable pairs.
4. Check duplicate images.
5. Preprocess images.
6. Create train, validation and test sets.

## 4. Dataset Split

The dataset will be divided into:

- Training set: used for model training
- Validation set: used for monitoring and parameter tuning
- Test set: used only for final evaluation

Input and target images from the same pair must always remain in the same split.

The test set will remain fixed during final evaluation.

## 5. Preprocessing

- Resize images to a common size.
- Convert images to RGB.
- Normalize pixel values.
- Maintain the same preprocessing for input and target where required.
- Preserve the input-target relationship.

## 6. Baseline Methods

The following classical methods will be used:

### CLAHE
Used for improving local contrast.

### Histogram Equalization
Used to enhances global contrast by redistributing pixels intensity values across the full available range.

### Gamma Correction
Used for brightness and contrast adjustment.

### White Balance
Used for correcting underwater color distortion.

## 7. Learning-Based Method

A CNN-based image-to-image enhancement model will be trained using paired input and target images.

The model will learn:

Input underwater image → Enhanced image

## 8. Evaluation Metrics

The following metrics will be considered:

- PSNR
- SSIM
- Edge F1 / Edge Preservation
- Processing Time
- UIQM/UCIQE where applicable
- Visual comparison

## 9. Experimental Comparison

The project will compare:

1. Classical enhancement methods
2. CNN-based enhancement
3. Tuned CNN model

The same evaluation procedure will be used for fair comparison.

## 10. Error Analysis

The final model will be checked for:

- Very dark images
- Low-contrast scenes
- Color distortion
- Loss of fine details
- Poor edge preservation
- Complex underwater scenes

## 11. Reproducibility

The following will be recorded:

- Dataset version
- Dataset split
- Preprocessing settings
- Model parameters
- Training settings
- Evaluation metrics
- Experiment results

## 12. Expected Output

The final output will be an enhanced underwater image along with quantitative evaluation results and visual comparisons.
