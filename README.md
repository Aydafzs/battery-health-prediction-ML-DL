# battery-health-prediction-ML-DL
Comparative analysis of ML and LSTM models for lithium-ion battery voltage prediction using NASA dataset.
#  Battery Health Prediction using Machine Learning and Deep Learning

This repository contains the implementation and results of a research project focused on predicting lithium-ion battery voltage and degradation behavior using both Machine Learning (Random Forest, XGBoost) and Deep Learning (LSTM) models.

---

##  Dataset  
Source: NASA Accelerated Life Testing (ALT) dataset  
Includes voltage, current, temperature, and time features from Li-ion batteries under different load conditions.  
[Download](https://data.nasa.gov/docs/legacy/battery_alt_dataset.zip)

---

##  Models Used  
| Model             | MAE    | RMSE   | R²     |
|-------------------|--------|--------|--------|
| Linear Regression | 0.500  | 0.840  | 0.33   |
| Random Forest     | 0.0146 | 0.093  | 0.9918 |
| XGBoost           | 0.113  | 0.278  | 0.9268 |
| LSTM              | 0.020  | 0.021  | ~0.97  |

---

##  Folder Structure  

