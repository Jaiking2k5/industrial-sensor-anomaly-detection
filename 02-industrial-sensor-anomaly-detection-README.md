# Industrial Sensor Anomaly Detection

An end-to-end machine-learning project for detecting abnormal behaviour in industrial sensor data.

> **Status:** Planned / Under Development  
> The repository currently defines the project architecture and development plan. Results and metrics will be added after experiments are completed.

## Overview

Industrial equipment produces large volumes of sensor measurements. Detecting abnormal operating behaviour can help identify potential failures or unusual operating conditions.

This project develops a machine-learning pipeline that processes multivariate sensor data and investigates models for anomaly/abnormal-condition detection.

## Objective

Build and evaluate a reproducible ML pipeline covering:

- data inspection
- preprocessing
- exploratory data analysis
- feature engineering
- leakage-aware dataset splitting
- baseline modelling
- model comparison
- imbalance-aware evaluation
- error analysis

## Pipeline

```text
Sensor Dataset
      |
      v
Data Inspection
      |
      v
Data Cleaning
      |
      v
Exploratory Data Analysis
      |
      v
Feature Engineering
      |
      v
Train / Validation / Test
      |
      v
Baseline Model
      |
      v
Model Comparison
      |
      v
Evaluation
      |
      v
Error Analysis
```

## ML Considerations

The project will explicitly investigate:

- missing values
- outliers
- class imbalance
- feature distributions
- data leakage
- train/validation/test separation
- baseline performance
- threshold selection
- false positives
- false negatives

## Planned Models

The initial comparison will use simple, interpretable baselines followed by stronger tree-based models.

Potential models:

1. Baseline classifier
2. Logistic Regression where appropriate
3. Random Forest
4. XGBoost

A neural network will only be considered if the dataset and experimental results justify it.

## Evaluation

Depending on the selected dataset, the project will report:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- PR-AUC
- Confusion Matrix

For imbalanced data, accuracy will not be treated as the sole performance measure.

## Planned Repository Structure

```text
industrial-sensor-anomaly-detection/
├── data/
├── notebooks/
├── src/
│   ├── preprocessing.py
│   ├── features.py
│   ├── train.py
│   └── evaluate.py
├── models/
├── reports/
├── tests/
├── requirements.txt
├── README.md
└── .gitignore
```

## Development Plan

1. Select a suitable open dataset.
2. Inspect features, labels, missing values, and class distribution.
3. Perform exploratory data analysis.
4. Establish a simple baseline.
5. Build a preprocessing pipeline.
6. Engineer useful features.
7. Train Random Forest and XGBoost models.
8. Evaluate using appropriate classification metrics.
9. Perform error analysis.
10. Document failure cases.
11. Make the experiment reproducible.

## Technology Stack

- Python
- Pandas
- NumPy
- scikit-learn
- XGBoost
- Matplotlib
- Jupyter

## Expected Learning Outcomes

- Data preprocessing
- Exploratory data analysis
- Feature engineering
- Supervised machine learning
- Imbalanced classification
- Model selection
- Evaluation methodology
- Error analysis
- Reproducible ML workflows
