# Bioreactor Machine Learning

This repository contains code and data used to train machine learning models for predicting the temporal evolution of optical density (OD) in cyanobacterial cultures based on environmental input parameters. These parameters include temperature, light intensity, dissolved oxygen, and pH.

## Repository Structure

### 🧠 Models
Model script filenames reflect the machine learning algorithm used:
- `xgboost.py` — Implements the XGBoost model.
- `regressors.py` — Contains both Random Forest and Linear Regression models.

### 🧼 Data Processing
- `data_collation.py` — Cleans and combines raw experimental data, and visualizes correlations using heatmaps.
- `data_preprocessing.py` — Calculates relevant statistics, including the temporal differential of OD (ΔOD), to prepare the dataset for model training.

## Modeling Strategy

The machine learning models were designed to predict the **temporal change in optical density (ΔOD)** given environmental input parameters. This allows for reconstruction of the full OD time course and offers predictive capabilities without needing to rerun physical experiments.

## Light Regimes

Two separate models were trained to account for different lighting conditions:
- **12-hour light/dark cycle**
- **Continuous light exposure**

Each model is trained on the respective dataset, which is included in the repository.

---

Feel free to explore the code and datasets to understand how environmental conditions affect microbial growth dynamics. Let us know if you use or extend this work!

