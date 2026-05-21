# ehr-clinical-prediction-ml-pipeline
Automated machine learning pipeline and Streamlit dashboard for clinical prediction under temporal shift in EHR data using Decision Trees, SVMs, Neural Networks, and continual learning.
# EHR Clinical Prediction ML Pipeline

BITS F464 Machine Learning – Assignment 2

## Overview

This project implements an automated machine learning pipeline and interactive Streamlit dashboard for clinical prediction under temporal shift using Electronic Health Record (EHR) data.

The project focuses on:
- Multi-table EHR data integration
- Feature engineering and aggregation
- Exploratory Data Analysis (EDA)
- Temporal dataset splitting
- Classification modeling
- Continual learning
- Temporal drift analysis
- Interactive dashboard visualization

The pipeline evaluates model generalization across historical and current healthcare datasets and studies the impact of temporal data drift in clinical prediction systems.

---

# Models Implemented

## Classification Models
- Decision Tree Classifier
- Support Vector Machine (SVM)
- Neural Network (MLPClassifier)

## Continual Learning Approaches
- Fine-tuned Neural Network
- Incremental SVM using SGDClassifier
- Retrained Decision Tree on combined datasets

---

# Dataset Information

The dataset is a synthetic Electronic Health Record (EHR) dataset designed for clinical prediction and temporal shift analysis.

## Dataset Source

Full Dataset Drive Link:

https://drive.google.com/drive/folders/1d7QielEDfhua8YfU77U0EmPF048LEcLv

---

# Dataset Files Used

The project uses multiple relational healthcare tables:

| File Name | Description |
|---|---|
| allergies.csv | Patient allergy records |
| careplans.csv | Treatment and care plans |
| claims.csv | Insurance claims |
| claims_transactions.csv | Financial claim transactions |
| conditions.csv | Diagnosed medical conditions |
| devices.csv | Medical device usage |
| encounters.csv | Patient encounters and visits |
| imaging_studies.csv | Imaging study records |
| immunizations.csv | Vaccination records |
| medications.csv | Prescribed medications |
| observations.csv | Clinical observations and vitals |
| organizations.csv | Healthcare organizations |
| patients.csv | Patient demographic information |
| payer_transitions.csv | Insurance payer transitions |
| procedures.csv | Medical procedures |
| providers.csv | Healthcare providers |
| supplies.csv | Medical supplies data |

---

# Key Features Implemented

## Data Engineering
- Multi-table relational joins
- Patient-level feature aggregation
- Missing value handling
- Numerical scaling and encoding
- Temporal filtering

## Exploratory Data Analysis
- Feature distributions
- Correlation heatmaps
- Demographic analysis
- Drift analysis between datasets
- Class distribution analysis

## Temporal Dataset Splitting
- Dataset 1 (Historical)
- Dataset 2 (Current)

based on encounter timestamps.

## Model Evaluation
Models are evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Confusion Matrix

## Continual Learning
The project simulates real-world ML deployment where models trained on historical healthcare data are continuously adapted to new patient distributions.

---

# Dashboard Features

The Streamlit dashboard includes:
- Raw dataset previews
- Interactive EDA
- Feature engineering visualization
- Model training metrics
- ROC curves
- Confusion matrices
- Temporal shift analysis
- Continual learning comparison
- Final results summary

---

# Technologies Used

- Python
- Streamlit
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib

---

# Project Structure

```text
ehr-clinical-prediction-ml-pipeline/
│
├── data/
│   ├── allergies.csv
│   ├── careplans.csv
│   ├── claims.csv
│   ├── claims_transactions.csv
│   ├── conditions.csv
│   ├── devices.csv
│   ├── encounters.csv
│   ├── imaging_studies.csv
│   ├── immunizations.csv
│   ├── medications.csv
│   ├── observations.csv
│   ├── organizations.csv
│   ├── patients.csv
│   ├── payer_transitions.csv
│   ├── procedures.csv
│   ├── providers.csv
│   └── supplies.csv
│
├── Dashboard.py
├── Description.pdf
├── README.md
├── requirements.txt
└── .gitignore
```

---

# Installation

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# Running the Dashboard

Run the Streamlit application:

```bash
streamlit run Dashboard.py
```

---

# Team Members

- Aayush Shah
- Sakshi Bharadwaj
- Harsh Sharma
- Gaurvi Khurana

BITS Pilani Hyderabad Campus

---

# Assignment Objective

This project was developed as part of:

BITS F464 Machine Learning — Assignment 2:
“Automated Machine Learning Pipeline and Dashboard for Clinical Prediction under Temporal Shift in EHR Data”

The objective is to study:
- predictive healthcare modeling
- temporal distribution drift
- model generalization
- continual learning in healthcare systems

using structured Electronic Health Record datasets.

---

# Notes
- The dataset is large and may not be fully hosted directly on GitHub.
- If required, use the provided Google Drive link to access the complete dataset.
- Ensure all CSV files are placed inside the `data/` directory before running the dashboard.
- The dataset is large and may not be fully hosted directly on GitHub.
- If required, use the provided Google Drive link to access the complete dataset.
- Ensure all CSV files are placed inside the `data/` directory before running the dashboard.
