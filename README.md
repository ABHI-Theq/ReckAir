# ✈️ ReckAir - Predictive Maintenance of Renewable Energy

ReckAir is a machine learning-based project aimed at predictive maintenance within the renewable energy sector. It uses historical sensor data to forecast potential equipment failures and assess component health. The project includes data preprocessing, exploratory data analysis (EDA), feature engineering, and the creation of a predictive model. A production-ready `.pkl` model is included for deployment.

---

## 📁 Project Structure

```
ReckAir/
├── ReckAir.ipynb             # Jupyter notebook with data preprocessing, EDA, modeling
├── ReckAir.pkl               # Trained model saved as a pickle file
├── ReckAir_Train_Data.xlsx   # Excel file containing the training dataset
└── ReckAir_Test_Data.xlsx    # Excel file containing the test dataset
```

---

## 🎓 Project Objective

To perform predictive maintenance for renewable energy components (e.g., turbines) using sensor data by:

* Identifying failure patterns
* Engineering health-related features
* Predicting breakdowns before they occur

---

## 📊 Dataset Overview

### A. Data Sources

* Historical operational data from renewable energy equipment (e.g., pressure, vibration, temperature).

### B. Data Structure

* Time series and event-based data containing sensor readings and component health status.

---

## 🔄 Data Preprocessing

### a. Data Cleaning

* Removed missing, duplicate, or anomalous records.

### b. Data Transformation

* Scaled sensor readings
* Converted timestamps
* Merged component-specific datasets

### c. Feature Engineering

* Rate of change in vibration or pressure
* Cumulative operational time before failure
* Deviation from baseline behavior
* Fault frequency aggregation (e.g., failure count per turbine)

---

## 📊 Exploratory Data Analysis (EDA)

### a. Univariate Analysis

* Distribution of individual sensor values

### b. Bivariate Analysis

* Correlation between sensor readings and failures

### c. Temporal Patterns

* Time-series visualization of operational metrics

### d. Component Health Analysis

* Lifecycle visualization of turbines

### e. Failure Analysis

* Distribution and root cause exploration of failures

---

## 📊 Key Insights

* High correlation between vibration spikes and imminent failures
* Certain turbines show consistent early failure patterns
* Operational time is a strong predictor for component fatigue

---

## 🚀 Modeling Pipeline

1. **Model Training**

   * Trained various regression/classification models
   * Tuned hyperparameters for best results

2. **Model Evaluation**

   * Used R² score, F1-score, Precision, Recall, etc.

3. **Model Exporting**

   * Final model exported as `ReckAir.pkl`

---

## 🚀 How to Use

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/ReckAir.git
   cd ReckAir
   ```

2. Launch the notebook:

   ```bash
   jupyter notebook ReckAir.ipynb
   ```

3. Follow the notebook steps to load, process, analyze, and model data.

4. Use the `ReckAir.pkl` file in deployment apps (Flask, Streamlit, etc.) for predictive maintenance insights.

---

## 📌 To Do

* [ ] Integrate real-time sensor data
* [ ] Build dashboard for monitoring component health
* [ ] Automate retraining pipeline for dynamic environments

---

## 📜 License

This project is open-source under the [MIT License](LICENSE).
