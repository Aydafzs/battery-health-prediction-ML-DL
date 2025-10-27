<img width="1024" height="1024" alt="banner" src="https://github.com/user-attachments/assets/48677f00-5ee4-411a-9c3b-8e89b5330658" />
# battery-health-prediction-ML-DL
Comparative analysis of ML and LSTM models for lithium-ion battery voltage prediction using NASA dataset.
#  Battery Health Prediction using Machine Learning and Deep Learning

This repository contains the implementation and results of a research project focused on predicting lithium-ion battery voltage and degradation behavior using both Machine Learning (Random Forest, XGBoost) and Deep Learning (LSTM) models.
## ☁️ Full Project Access
All datasets, trained models and complete results are available in Google Drive:  
🔗 [Open the full project via Google Drive](https://drive.google.com/file/d/1iaPDphWsycz6nQNrwNkPU6e3jV7D1KfG/view?usp=sharing)

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
battery-health-prediction-ML-DL/
│
├── data/ # NASA battery dataset (raw and processed)
├── notebooks/ # Jupyter notebooks for ML & LSTM models
├── models/ # Trained Random Forest, XGBoost, and LSTM models
├── results/ # Performance plots and visualizations
├── requirements.txt # Python dependencies
└── README.md # Project documentation

How to Run

Clone the repository

git clone https://github.com/username/battery-health-prediction-ML-DL.git
cd battery-health-prediction-ML-DL


Install dependencies

pip install -r requirements.txt


Run the models

python main.py

📊 Results Summary

Machine Learning models (RF, XGBoost) provided excellent accuracy on test data, with Random Forest achieving the lowest MAE (0.0146).

Deep Learning (LSTM) captured temporal voltage trends effectively, with near-perfect correlation between predicted and actual battery voltage curves.

Results confirm that ensemble ML models are efficient for quick inference, while LSTM is superior for long-term cycle prediction.

🔍 Visualization Samples

Voltage vs. Cycle plots for Random Forest and LSTM predictions

LSTM loss curve during training

Feature importance visualization for RF and XGBoost

🧠 Key Insights

Temperature and discharge current significantly affect battery degradation.

Time-series models (LSTM) outperform static ML models for sequence prediction.

Feature engineering (voltage statistics, ΔV/Δt) improves accuracy of ML methods.

🧾 Citation

If you use this project, please cite as:

Mahmoudi, F. (2025). Battery Health Prediction using Machine Learning and Deep Learning (NASA Dataset). GitHub Repository.
