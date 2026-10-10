# AI/ML-Based Prediction of Kerf Width in Wire EDM (WEDM)

## Project Overview
This repository contains the dataset and code for an academic research project focused on **Non-Traditional Machining**. The goal of this project is to develop and compare different Artificial Intelligence and Machine Learning regression models to predict the Kerf Width in Wire Electrical Discharge Machining (WEDM).

## Objective
To accurately predict Kerf Width using the following machining parameters:
*   Wire Feed Rate (mm/s)
*   Voltage (V)
*   Pulse ON Time (µs)
*   Pulse OFF Time (µs)
*   Peak Current (A)

## Machine Learning Models
The project evaluates and compares four machine learning algorithms to determine the best-performing model for this specific manufacturing problem:
1.  **Random Forest Regressor**
2.  **XGBoost Regressor**
3.  **Artificial Neural Network (ANN)**
4.  **Support Vector Regression (SVR)**

## Dataset
The repository includes a combined dataset (`WEDM_Real_and_Synthetic_Combined.csv`) consisting of:
*   **27 Real Observations:** Data obtained directly from physical WEDM experiments.
*   **18 Synthetic Observations:** Mathematically interpolated data points derived from the real observations to assist in training.

*(Note: Synthetic data is rigorously excluded from validation metrics to preserve scientific integrity).*

## Repository Contents
*   `WEDM_Real_and_Synthetic_Combined.csv`: The primary dataset used for training and evaluating the models.
*   `WEDM_Real_27_Experiments.csv`: The raw experimental data.

## Getting Started
The project was originally developed and executed in Google Colab. To replicate the results:
1. Upload the dataset and the associated `.ipynb` notebook to Google Colab.
2. Run the notebook from top to bottom.
3. The models will be trained, evaluated (R², RMSE, MAE), and compared automatically.
