# ⚡ Wind Turbine SCADA – Power Forecasting Using XGBoost

This project demonstrates a machine learning approach to **predicting wind turbine power output** using real-world SCADA data. It leverages **XGBoost Regression** to model the relationship between wind parameters and active power generation.

## 📁 Dataset

* **Source**: [Kaggle - Wind Turbine SCADA Dataset](https://www.kaggle.com/datasets/berkerisen/wind-turbine-scada-dataset)
* **File Used**: `T1.csv`
* **Records**: 50,530
* **Features**:

  * `Date/Time`
  * `LV ActivePower (kW)`
  * `Wind Speed (m/s)`
  * `Theoretical_Power_Curve (KWh)`
  * `Wind Direction (°)`

---

## 🧠 Objective

Predict the **LV ActivePower (kW)** using features like:

* Wind Speed
* Theoretical Power Curve
* Wind Direction

---

## 🔍 Exploratory Data Analysis

* Visualized the relationship between wind speed and power output
* Checked for null values and converted `Date/Time` to datetime format
* Plotted scatter graphs to understand feature distributions

---

## 🛠️ Tech Stack

* Python (Pandas, NumPy, Matplotlib, Seaborn)
* Scikit-learn for preprocessing and metrics
* XGBoost for regression modeling
* KaggleHub for dataset integration

---

## 🧪 Model Training

* Features scaled using **StandardScaler**
* Split into training and test sets (80/20)
* Trained using **XGBRegressor**

### ✅ Results:

* **RMSE**: 397.47
* **R² Score**: 0.907

---

## 📊 Visualization

Plots showing:

* Wind Speed vs Active Power Output
* Comparison of Actual vs Predicted values over 100 samples

---

## 🚀 Getting Started

### Requirements:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost kagglehub
```

### Run the notebook or script:

```bash
python wind_forecasting.py
```

Make sure your Kaggle API is properly set up if using `kagglehub`.

---

## 📎 License

This project is open-sourced under the **MIT License**.
