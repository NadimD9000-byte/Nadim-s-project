# MSD Risk Prediction Using Machine Learning

## Overview

This project focuses on predicting Musculoskeletal Disorder (MSD) risk levels using machine learning techniques.

The objective is to develop and evaluate supervised machine learning models for classifying MSD risk levels based on the available dataset features.

## Machine Learning Models

The following models are implemented and compared:

- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- XGBoost

XGBoost is used as the primary machine learning model.

## Data Preprocessing

The workflow includes:

1. Loading the dataset
2. Encoding the target variable
3. One-hot encoding of categorical variables
4. Train-test splitting
5. Feature scaling

An 80:20 stratified train-test split is used.

## XGBoost Model

The XGBoost classifier is configured with:

- Number of estimators: 200
- Maximum depth: 4
- Learning rate: 0.1
- Subsample: 0.8
- Column sampling: 0.8
- Minimum child weight: 3
- L1 regularization: 0.01
- L2 regularization: 2
- Random state: 42

## Evaluation Metrics

The models are evaluated using:

- Accuracy
- Weighted F1-score
- Macro F1-score
- 5-fold cross-validation
- Weighted ROC-AUC
- Confusion matrix
- Feature importance

## Explainable AI

SHAP (SHapley Additive exPlanations) is used to investigate feature contributions to the XGBoost predictions.

## Project Files

- `msd_prediction.ipynb` — Complete machine learning implementation
- `requirements.txt` — Required Python packages
- `data/README.md` — Dataset information

## Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- SHAP
- Matplotlib
- Seaborn
- Google Colab

## How to Run

Install the required packages using:

```bash
pip install -r requirements.txt
