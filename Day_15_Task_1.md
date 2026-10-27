#  Baseline Results and Mentor Feedback

##  Objective

The objective of Day 15 was to present the classical enhancement baseline results, review edge-preservation results, confirm the evaluation methodology, and obtain mentor feedback before moving to the next stage.

---

##  Classical Baseline Methods

The following classical enhancement methods were evaluated:

- CLAHE
- Gamma Correction
- White Balance

---

##  Baseline Results

| Method | PSNR | SSIM | Edge F1 |
|---|---:|---:|---:|
| CLAHE | 10.99 | 0.4346 | 0.0572 |
| Gamma Correction | 10.93 | 0.4821 | 0.0416 |
| White Balance | 10.44 | 0.4611 | 0.0416 |

### Main Observations

- CLAHE achieved the highest PSNR.
- Gamma Correction achieved the highest SSIM.
- CLAHE achieved the highest Edge F1.
- White Balance achieved the lowest PSNR.
- The results show that classical methods have limitations for severely degraded underwater images.

---

##  Edge Preservation

Edge F1 was used to measure the similarity between edges in the enhanced output and the corresponding target image.

### Results

- CLAHE: 0.0572
- Gamma Correction: 0.0416
- White Balance: 0.0416

CLAHE achieved the highest Edge F1 among the tested classical methods.

---

##   Fair Evaluation 

All three methods were evaluated using:

- The same input images
- The same corresponding target images
- The same evaluation procedure
- The same PSNR and SSIM metrics
- The same edge-preservation evaluation

This provides a consistent basis for comparing the classical enhancement methods.

---

##  Current Baseline Decision

Based on the current quantitative results:

**CLAHE is considered the strongest classical reference baseline.**

Reasons:

- Highest PSNR: 10.99
- Highest Edge F1: 0.0572
- Provides noticeable local contrast improvement.

Gamma Correction is also retained as an important comparison because it achieved the highest SSIM of 0.4821.

---

##  Proposed Next Direction

The classical methods provide useful baseline results but have limited ability to recover hidden details in heavily degraded underwater images.

The proposed next direction is:

**Learning-based image-to-image enhancement**

### Hypothesis

A learning-based enhancement method may learn complex underwater degradation patterns and improve brightness, contrast, detail recovery, and edge preservation more effectively than simple classical methods.

---

##  Mentor Review Checklist

Please review the following questions and provide feedback:

### 1. Metric Selection

**Sir, are PSNR, SSIM and Edge F1 suitable for this project?**

Mentor Feedback:

**yes**

---

### 2. Classical Baseline

**Sir, is CLAHE acceptable as the classical reference baseline?**

Mentor Feedback:

**Yes, as it's value is high**

---

### 3. Additional Methods or Metrics

**Should we add any other classical enhancement method or evaluation metric?**

Mentor Feedback:

**Not needed**

---

### 4. Fair Comparison

**Is the current input-target comparison fair and appropriate?**

Mentor Feedback:

**Yes**

---

### 5. Preprocessing and Evaluation

**Are there any preprocessing or evaluation corrections required?**

Mentor Feedback:

**No**

---

### 6. Next Stage

**Can we proceed to the learning-based image enhancement stage?**

Mentor Feedback:

**Yes**

---

##  Corrections Suggested by Mentor

**You can procede further**

---

##  Next Steps

After incorporating mentor feedback:

- Finalize the classical baseline.
- Apply required corrections.
- Finalize evaluation metrics.
- Confirm the learning-based approach.
- Begin the next stage of model development.

---

### Mentor Signature

**Signature:**  gollasudheerbabu

**Date:**  04/09/26
