# Controlled Hyperparameter Experiments

## Objective

Tune the shortlisted CNN and Refined CLAHE candidates using controlled parameter experiments.

## CNN Experiments

Learning rate was varied while keeping the remaining training settings fixed.

Experiments:
- 0.0001
- 0.001
- 0.01

Selection criterion:
Lowest validation loss.

## CLAHE Experiments

Clip limit was varied while keeping grid size fixed at 8×8.

Experiments:
- 2.0
- 3.0
- 4.0

Selection criterion:
Highest validation PSNR.

## Data Usage

Training data was used for CNN training.

Validation data was used for parameter selection.

The test set was kept completely untouched.

## Deliverables

- CNN experiment log
- CLAHE experiment log
- Best validated CNN configuration
- Best validated CLAHE configuration

## Conclusion

The best validated configurations were selected from the controlled experiments and saved for final evaluation.
