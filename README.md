# Predictive Maintenance & Downtime Risk Analysis

## Project Overview

This project implements a predictive maintenance solution by analyzing the **AI4I 2020 Predictive Maintenance dataset (UCI)** to estimate the risk of machine downtime and proactively schedule maintenance. The goal is to prevent unplanned failures, optimize maintenance schedules, and improve operational efficiency in industrial environments.

---

## Dataset

The dataset consists of sensor readings and operational settings collected from industrial machines.
Key Features:

* Air temperature \[K]
* Process temperature \[K]
* Rotational speed \[rpm]
* Torque \[Nm]
* Tool wear \[min]
* Product ID, UDI
  Target:
* Target → Binary classification: Failure (1) or No Failure (0)

Source: [UCI Machine Learning Repository – AI4I 2020 Predictive Maintenance Dataset](https://archive.ics.uci.edu/ml/datasets/AI4I+2020+Predictive+Maintenance+Dataset)

---

## Objective

* Build a machine learning model to predict machine failure based on sensor data.
* Generate a risk score for downtime to enable predictive maintenance decisions.
* Deploy a simple dashboard for visualization of risk and key metrics.

---

## Features

* Data Preprocessing & Cleaning
* Exploratory Data Analysis (EDA) with visualizations
* Feature Engineering
* Predictive Modeling (Random Forest, XGBoost, etc.)
* Imbalanced Data Handling (SMOTE, class weights)
* Risk Scoring based on predicted probabilities
* Interactive Dashboard built using Streamlit
* PDF Report Export for insights and decisions

---

## Tools & Technologies

* Python (pandas, scikit-learn, XGBoost)
* Visualization (matplotlib, seaborn, Plotly)
* Imbalanced-learn (SMOTE)
* Streamlit (for dashboard)
* Joblib (model serialization)
* Jupyter Notebook (exploration & prototyping)

---

## Usage

### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/predictive-maintenance-risk.git
cd predictive-maintenance-risk
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run Streamlit Dashboard

```bash
streamlit run app.py
```

### 4. Upload New Data (Optional)

Use the dashboard to upload new sensor data and get real-time failure risk predictions.

---

## Model Evaluation

Model performance is evaluated using:

* Precision, Recall, F1-Score
* ROC-AUC
* Confusion Matrix

Sample results:

* ROC-AUC: 0.92
* F1-Score: 0.87

---

## Future Scope

* Real-time integration with IoT data streams
* Automated scheduling of maintenance tasks based on risk thresholds
* Predict remaining useful life (RUL) estimation
* Add anomaly detection for sensor anomalies

---

## License

This project is open-source under the MIT License.

