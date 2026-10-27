#  Research Framing & Mentor Review

## Project Title
Underwater Image Enhancement Using Classical and Learning-Based Methods

## Research Question
How effectively can underwater images be enhanced while maintaining image quality, structure, and important visual details?

## Objectives
- Improve underwater image quality.
- Compare classical and learning-based enhancement methods.
- Preserve important edges and details.
- Evaluate enhancement using measurable metrics.
- Study limitations and failure cases.

## Target Definition
Input: Low-quality/degraded underwater image.
Target: Corresponding clearer/enhanced underwater image.
Output: Enhanced image produced by the model.

## Methods
Classical Methods:
- CLAHE
- Gamma Correction
- White Balance

Learning-Based Method:
- CNN image-to-image enhancement

## Evaluation Metrics
- PSNR
- SSIM
- Edge F1 / Edge Preservation
- Processing Time
- Visual Comparison

## Initial Findings
- Underwater images generally have low brightness and contrast.
- Classical methods provide useful baseline results.
- The CNN approach provides improved image similarity compared with the initial classical methods.
- Edge preservation is important for evaluating enhancement quality.
- Visual comparison is also necessary along with numerical metrics.

## Blockers
- Some input-target pairs were found to be incorrectly matched.
- Very dark and low-contrast images are difficult to enhance.
- Dataset quality can affect model performance.
- Complex underwater scenes may produce weaker results.

## Next Plan
- Finalize the verified dataset.
- Continue CNN training and refinement.
- Compare the CNN with classical methods.
- Evaluate PSNR, SSIM and Edge F1.
- Analyze difficult and failed images.
- Perform final validation.
- Prepare the final report and presentation.

## Project Pipeline
Raw Dataset
→ Quality Check
→ Input-Target Pairing
→ Preprocessing
→ Train/Validation/Test Split
→ Model Training
→ Evaluation
→ Error Analysis
→ Final Validation
