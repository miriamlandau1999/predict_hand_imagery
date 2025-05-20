# Neural Decoding: Left vs Right Hand Imagery Classification

## Overview
This project focuses on decoding neural activity from EEG signals to classify left vs right hand imagery movements. Using machine learning techniques, we aim to predict whether a subject is imagining moving their left hand (0) or right hand (1) based on EEG recordings.

This is a practice project designed to prepare for technical interviews, focusing on machine learning and signal processing. 

## Problem Statement
- **Task**: Binary Classification
- **Input**: EEG signals
- **Output**: Hand imagery prediction (0 = Left, 1 = Right)
- **Approach**: Classical Machine Learning with tabular features

## Dataset
The project uses the [EEG Motor Movement/Imagery Dataset](https://physionet.org/content/eegmmidb/1.0.0/) from PhysioNet.

### Feature Extraction
Each trial is processed to extract statistical features:
- 64 EEG channels
- 4 statistical measures per channel:
  - Standard deviation
  - Mean
  - Minimum
  - Maximum
- Total: 256 features per trial

## Technical Stack
- **MNE-Python**: EEG signal processing and analysis
- **Pandas**:
- **NumPy**: 
- **Scikit-learn**: 

## Project Structure
```
├── data/
│   ├── raw/          # Original EEG recordings
│   └── processed/    # feature-extracted data in csv
├── notebooks/        # Jupyter notebooks
└── requirements.txt  # Project dependencies
```

## Getting Started
1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run the notebooks in order:
   - `01_data_loading_and_overview.ipynb`
   - `02_exploratory_data_analysis.ipynb`
   - [Additional notebooks to be added]

## Interview Preparation Focus
This project demonstrates:
- Data preprocessing and feature engineering skills
- Classical machine learning implementation
- Understanding of EEG signal processing and real-world biomedical data
- Implementation of machine learning pipelines
- Documentation and code organization