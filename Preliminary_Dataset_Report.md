# Dataset Receipt & Initial Inspection

## 1. Dataset Received

The project uses an underwater image dataset containing:

- Input images
- Target images
- Generated images
- Multiple dataset/epoch folders

The original dataset was received and preserved without modification.

## 2. Raw Dataset Preservation

The raw dataset is kept separately from the processed dataset.

No images were deleted, renamed, overwritten, or modified during the initial inspection stage.

All later cleaning and preprocessing are performed on separate copies.

## 3. Dataset Organization

The raw data is organized into multiple folders/epochs.

Each folder may contain different versions of underwater images such as:

- `input`
- `target`
- `generated`

The filename/image ID is used as an initial reference for identifying related images.

## 4. Initial Observations

The initial inspection showed:

- Input images are generally darker than target images.
- Some input images have low contrast.
- Target images generally contain improved visual information.
- Generated images are available for comparison.
- Image dimensions are generally suitable for image-to-image enhancement.
- The dataset contains multiple image groups that require careful pairing.

## 5. Data Quality Concerns

The following risks were identified for further checking:

### Incorrect Pairing
An input and target with the same image ID may not always represent the same scene.

### Duplicate Files
Some duplicate or copied files may exist.

### Missing Pairs
Some input images may not have a valid target image.

### Low-Quality Images
Very dark and low-contrast images may be difficult for enhancement.

### Data Leakage
Duplicate or highly similar images should not be present across different dataset splits.

## 6. Important Finding

Filename-based pairing alone cannot guarantee that an input image and target image are semantically correct.

Therefore, visual verification of important input-target pairs is required before creating the final dataset.

## 7. Raw Data Policy

The raw dataset remains unchanged.

The following stages are performed separately:

Raw Dataset
→ Inspection
→ Pair Verification
→ Cleaning
→ Dataset V1
→ Model Training

## 8. Initial Conclusion

The dataset contains sufficient material for further underwater image enhancement experiments, but data quality and input-target pairing must be verified before final model training.

The inspection stage provides the basis for creating a clean and reliable Dataset V1.
