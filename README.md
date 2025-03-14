# Credit Risk Estimation Using Machine Learning

This repository contains a Jupyter Notebook that demonstrates a complete workflow for estimating credit risk parameters—**Probability of Default (PD), Loss Given Default (LGD), and Exposure at Default (EAD)**—using simulated financial statement data and machine learning.  

The notebook starts with financial statement outputs from a **Financial Statement Analyzer for ABC Corp**, derives key financial ratios, trains regression models on synthetic data, and finally predicts risk parameters to compute the **Expected Loss (EL)**.

---

## 🔹 Overview

The workflow is divided into the following steps:

### 1️⃣ Data Simulation
- Simulate a dataset with financial ratios, such as:
  - **Liquidity Ratios**: Current ratio, quick ratio  
  - **Profitability Ratios**: Net profit margin, ROA, ROE  
  - **Leverage Ratios**: Debt-to-equity  
  - **Efficiency Ratios**: Asset turnover  
- Generate synthetic target variables (**PD, LGD, and EAD**) for training.

### 2️⃣ Model Training
- Split the simulated dataset into **training** and **testing** sets.  
- Train **Random Forest models** for each risk parameter (**PD, LGD, and EAD**).

### 3️⃣ ABC Corp Analysis
- Create a **feature vector** for ABC Corp using the **derived financial ratios** from its financial statements.

### 4️⃣ Risk Prediction & Expected Loss Calculation
- Predict **PD, LGD, and EAD** using the trained models.
- Compute the **Expected Loss (EL)** using the formula:

Expected Loss (EL) = PD × LGD × EAD

### 5️⃣ Visualization
- Plot **actual vs. predicted values** for the test set to evaluate model performance.

---

## 🔹 Installation & Usage

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/credit-risk-estimation.git
   cd credit-risk-estimation
