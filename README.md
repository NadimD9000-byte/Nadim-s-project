# Sales Forecasting Using Machine Learning

## Overview
This project predicts product sales using Machine Learning techniques.

## Dataset
- Total rows: 150,150
- Features include:
  - store_id
  - sku_id
  - week
  - units_sold

## Data Preprocessing
- Split week column into day/month/week
- Removed unnecessary columns
- Removed outliers
- One-hot encoding applied on categorical features

## Machine Learning Model
- Random Forest Regressor

## Hyperparameter Tuning
Used GridSearchCV with:
- n_estimators
- min_samples_split

## Model Performance
- Initial R² Score: 0.776
- Improved R² Score: 0.811
- RMSE: 18.51

## Libraries Used
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Author
Nadim
