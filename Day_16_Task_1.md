# Day 16 – Improved Model

## Objective
Implement a simple supervised CNN for underwater image enhancement using paired input-target images.

## Model
A simple CNN was used to learn the mapping:

Input Image → CNN → Enhanced Image

## Training
- Dataset: Prepared Dataset V1
- Train images: 218
- Validation images: 47
- Batch size: 8
- Epochs: 10
- Loss: MSE Loss
- Optimizer: Adam
- Learning rate: 0.001

## Hypothesis
A simple supervised CNN can learn enhancement patterns from paired underwater input-target images and improve image quality.

## Output
- Trained CNN model
- Training/validation loss plot
- Sample validation outputs
