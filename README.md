<img width="1272" height="400" alt="banner" src="https://github.com/user-attachments/assets/a49a1652-1883-4f12-a4ef-2dd96b8bdb89" />

# 🔋 Battery Health Prediction using Machine Learning and Deep Learning  

### Comparative analysis of ML and LSTM models for lithium-ion battery voltage prediction using the NASA dataset  

---

## 🧩 Overview  
This project focuses on predicting **battery voltage and degradation behavior** using both traditional **Machine Learning** methods (Random Forest, XGBoost) and a **Deep Learning** model (LSTM).  
The NASA Accelerated Life Testing (ALT) dataset is used as the main source of data.  

The goal was to understand how different models perform when predicting voltage over time and to compare their performance in terms of accuracy and generalization.  

---

## ☁️ Full Project Access  
All datasets, trained models, and results are available here:  
🔗 [Open full project on Google Drive](https://drive.google.com/file/d/1iaPDphWsycz6nQNrwNkPU6e3jV7D1KfG/view?usp=sharing)

---

## 📦 Dataset  
**Source:** [NASA Accelerated Life Testing (ALT) dataset](https://data.nasa.gov/docs/legacy/battery_alt_dataset.zip)  

The dataset includes several Li-ion batteries tested under different load and temperature conditions.  

**Main features:**  
- Voltage (V)  
- Current (A)  
- Temperature (°C)  
- Time (s)  
- Cycle number  

---

## ⚙️ Folder Structure  
```

battery-health-prediction-ML-DL/
│
├── data/              # NASA battery dataset (raw and processed)
├── notebooks/         # Jupyter notebooks for ML & LSTM models
├── models/            # Trained Random Forest, XGBoost, and LSTM models
├── results/           # Figures and performance plots
├── requirements.txt   # Python dependencies
└── README.md          # Project description

````

---

## 🧠 Models Used  

| Model             | MAE    | RMSE   | R²     |
|-------------------|--------|--------|--------|
| Linear Regression | 0.500  | 0.840  | 0.33   |
| Random Forest     | 0.0146 | 0.093  | 0.9918 |
| XGBoost           | 0.113  | 0.278  | 0.9268 |
| LSTM              | 0.020  | 0.021  | ~0.97  |

The **Random Forest** model achieved the best results overall, followed by the **LSTM** network, which performed very well on time-series predictions.  

---

## 🚀 How to Run  

### Clone the repository  
```bash
git clone https://github.com/Aydafzs/battery-health-prediction-ML-DL.git
cd battery-health-prediction-ML-DL
````

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run the code

```bash
python main.py
```

You can also open the notebooks step by step:

```bash
jupyter notebook notebooks/
```

---

## 📊 Results Summary

* Machine learning models like **Random Forest** and **XGBoost** achieved very strong performance.
* **LSTM** was excellent for capturing the time-series behavior of battery voltage.
* The Random Forest model gave the lowest MAE (0.0146), showing very good accuracy.

---

## 🔍 Visualizations

The project includes several visualizations such as:

* Voltage vs. Cycle plots (predicted vs. actual)
* LSTM training loss curve
* Feature importance (RF and XGBoost)
* Correlation map between features

All figures are available in the `results/` folder.

---

## 💡 Key Points

* **Temperature** and **current** have a big impact on battery health.
* **LSTM** performs better on long time-series predictions.
* **Feature engineering** (like ΔV/Δt and statistical features) helps machine learning models improve.
* Combining **RF and LSTM** could be a great idea for future work.

---

## 👩‍🔬 Author

**Fatemeh Mahmoudi**
M.Sc. student in Nanomaterials Engineering, Sharif University of Technology

Interested in **Battery Materials, Machine Learning, and Sustainable Energy**

📍 Tehran, Iran
📧 [fatemeh.mahmoudi@sharif.edu](mailto:fatemeh.mahmoudi@sharif.edu)
🔗 [LinkedIn](https://www.linkedin.com/in/fatemeh-mahmoudi-a577a0103) | [GitHub](https://github.com/Aydafzs)
