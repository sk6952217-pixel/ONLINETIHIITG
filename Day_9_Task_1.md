# Approved Data Plan

## Project

Underwater Image Enhancement

## 1. Dataset

The dataset contains **3235 images** stored mainly in PNG format.

The identified image categories are:

- Input images: **1078**
- Target images: **1078**
- Generated images: **1078**

The images are organized into different epoch folders.

## 2. Data Quality Check

The dataset will be checked for:

- Duplicate images
- Missing images
- Invalid or corrupted images
- Incorrect file names
- Unmatched input-target pairs
- Incorrect image dimensions

During the initial inspection, one duplicate was identified:

`epoch_0110/img 74_input - Copy.png`

It was verified as an exact duplicate of the original input image.

The duplicate will not be treated as a separate data sample.

## 3. Pairing Strategy

Input, target, and generated images will be matched using their common image number.

Example:

- img 74_input.png
- img 74_target.png
- img 74_gen.png

## 4. Data Preparation Workflow

The data preparation process will follow these steps:

Raw Dataset  
  ↓  
Quality Check  
   ↓  
Duplicate Check  
    ↓  
Input–Target Pairing  
     ↓  
Preprocessing  
      ↓  
Train / Validation / Test Split  
      ↓  
Model Training

   ↓  
  Evaluation 

## 5. Data Storage

The original dataset will be kept unchanged.

Any cleaned or preprocessed data will be stored separately to preserve the original dataset.

## 6. Plan Status

The data-preparation plan is.

- Quality check
- Duplicate removal/exclusion
- Input-target pairing
- Preprocessing
- Dataset splitting
- Model training
- Evaluation
