# Multimodal Emotion Recognition using Speech and Text

## Overview

This project implements a Multimodal Emotion Recognition system using Speech and Text modalities with Deep Learning techniques on the TESS dataset.

The project contains three separate pipelines:

1. Speech Emotion Recognition
2. Text Emotion Recognition
3. Multimodal Fusion Emotion Recognition

The system uses:
- MFCC feature extraction
- Conv1D + LSTM architecture
- Text embeddings
- Feature-level fusion
- t-SNE visualization

Raw TESS audio files are excluded from GitHub because of file size limitations.  
However, trained models, plots, confusion matrices, t-SNE visualizations, and output files are included.

Dataset is provided separately through Google Drive.

---

# How to Run

## 1. Clone the Repository

```bash
git clone <repository_link>
cd project
```

## 2. Install Required Libraries

```bash
pip install -r requirements.txt
```

## 3. Download the TESS Dataset

Download and extract the TESS dataset.

Place the dataset folder inside the drive project folder directory :

```bash
project/
│
├── dataset/
```

Update the dataset path inside:
- speechmodel.ipynb
- textmodel.ipynb
- fusion.ipynb

before running the notebooks.

---

# Project Structure

```bash
project/
│
├── models/
│
│   ├── speech_pipeline/
│   │   ├── speechmodel.ipynb
│   │   └── speechmodel.keras
│   │
│   ├── text_pipeline/
│   │   ├── textmodel.ipynb
│   │   └── textmodel.keras
│   │
│   └── fusion_pipeline/
│       ├── fusion.ipynb
│       └── fusion.keras
│
├── outputs/
│   │
│   ├── model_accuracy_comparison.csv
│   │
│   ├── plots/
│   │   ├── accuracy plots
│   │   ├── loss plots
│   │   └── confusion matrices
│   │
│   └── t-SNE clusters/
│       ├── speech tsne
│       ├── text tsne
│       └── fusion tsne
│
├── dataset/
│
├── README.md
└── requirements.txt
