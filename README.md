# Amazon Sales Analysis & Market Prediction (Classical + Quantum + Forecasting)

## 📌 Project Overview
This project analyzes Amazon sales data, identifies sales trends, compares **classical machine learning (Logistic Regression)** with **Quantum Variational Classifier (VQC)**, and performs **time series forecasting using Prophet**.

---

## 📊 Dataset
- File: `amazon_sales_dataset.xlsx`
- Columns include:
  - `Date`
  - `Sales($)`
- New features engineered:
  - `Sales_Change` → Difference in sales from previous day
  - `Trend` → Label ("Up", "Down", "No Change")

---

## 🔧 Methodology

### 1. Exploratory Data Analysis (EDA)
- Sales difference visualization (bar chart: green=up, red=down).  
- Frequency of Up/Down trends using countplot.  
- Sales trend line plots.  

### 2. Quantum vs Classical Prediction
- Features: Sales patterns + engineered indicators  
- Labels: Trend (Up/Down)  
- Models:
  - **Classical:** Logistic Regression (baseline)  
  - **Quantum:** Variational Quantum Classifier (PennyLane)  
- Evaluation:
  - Accuracy comparison  
  - Confusion matrices  
  - Training curves  

### 3. Sales Forecasting (Prophet)
- Forecast future sales for **90 days ahead**.  
- Outputs:
  - Forecast plot with confidence interval  
  - Trend & seasonality components  

---

## 🛠️ Tech Stack
- **Python 3.9+**
- **Libraries:**
  - `pandas`, `numpy`
  - `matplotlib`, `seaborn`
  - `scikit-learn`
  - `pennylane`, `qiskit`
  - `prophet`

---

## 🚀 How to Run

1. Clone repo:
   ```bash
   git clone https://github.com/your-username/amazon-sales-vqc.git
   cd amazon-sales-vqc
