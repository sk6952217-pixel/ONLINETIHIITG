#  Repository / Folder Structure

```text
Underwater_Image_Enhancement/
│
├── README.md
│
├── dataset/
│   ├── train/
│   │   ├── input/
│   │   └── target/
│   ├── val/
│   │   ├── input/
│   │   └── target/
│   └── test/
│       ├── input/
│       └── target/
│
├── notebooks/
│   ├── dataset_preparation.ipynb
│   ├── classical_baseline.ipynb
│   ├── cnn_training.ipynb
│   └── evaluation.ipynb
│
├── model/
│   └── final_model.pth
│
├── outputs/
│   ├── classical/
│   ├── cnn/
│   └── comparisons/
│
├── results/
│   ├── experiment_log.csv
│   ├── metrics.csv
│   └── error_analysis.csv
│
└── report/
    ├── final_report.pdf
    └── final_presentation.pptx
