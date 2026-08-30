# Car Resell Price Prediction

A Machine Learning project using Python, Pandas, and Scikit-Learn to preprocess automotive datasets and train a Random Forest Regressor to predict car resale values.

## Overview

This repository contains a Jupyter Notebook (`car_resell.ipynb`) designed to predict the resell price of used cars. The workflow includes loading dataset splits from Google Drive, handling data types and missing values, and building a prediction pipeline with random forests.

## Features & Methods

* **Data Ingestion**: Automated Google Drive mounting and multi-file CSV ingestion (`train.csv`, `test.csv`, `test_labels.csv`).
* **Data Preprocessing**:
  * Numeric type enforcement on the `mileage` feature.
  * Median imputation for missing mileage entries.
* **Model Pipeline**:
  * Implements `RandomForestRegressor` for price estimation.
  * Uses `OneHotEncoder` for categorical feature transformations.
  * Evaluated using `MAE`, `MSE`, and `R²` metrics.
  * Model serialization via `joblib`.

## File Structure

```text
.
├── car_resell.ipynb   # Main Jupyter Notebook
└── README.md          # Project documentation
