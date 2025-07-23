# 🚨 Fraud Detection Project

---

## 📖 Project Overview

This project aims to **proactively detect fraudulent financial transactions** using advanced machine learning techniques. By analyzing millions of transaction records, it helps financial institutions minimize losses by identifying suspicious activities accurately and efficiently.

---

## 📊 Dataset Highlights

- Over **6 million** transaction records  
- Features include transaction types, amounts, account balances, and fraud indicators  
- Highly **imbalanced dataset** — fraudulent transactions constitute roughly **0.13%** of total transactions  

---

## 🛠 Approach & Methodology

1. **Data Cleaning & Preprocessing**  
   - Removed duplicates  
   - Handled missing values (none found)  
   - Analyzed and addressed multicollinearity among features  
   - Scaled numerical features for better model performance  

2. **Feature Selection**  
   - Dropped irrelevant categorical columns like `type`, `nameOrig`, and `nameDest`  
   - Selected features based on correlation and multicollinearity analysis  

3. **Modeling**  
   - Trained **Random Forest** and **XGBoost** classifiers  
   - Applied class weighting to address data imbalance  

4. **Evaluation**  
   - Performance metrics: Precision, Recall, F1-score, Confusion Matrix, ROC-AUC  
   - Random Forest achieved a ROC-AUC of **0.99**, showing excellent predictive power  

---

## 📈 Results Summary

| Metric          | Random Forest | XGBoost      |
|-----------------|---------------|--------------|
| Precision (Fraud)| ~97%          | ~77%         |
| Recall (Fraud)   | ~70%          | ~67%         |
| F1-Score (Fraud) | ~81%          | ~71%         |
| ROC-AUC         | 0.9911        | (High)       |

---

## 🚀 Usage Instructions

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/fraud-detection-project.git
   cd fraud-detection-project
````

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```
3. Open and run the Jupyter Notebook:

   ```bash
   jupyter notebook Fraud_Detection.ipynb
   ```
4. Load your dataset and execute all cells step-by-step.

---

## 🔍 Key Insights & Recommendations

* Deploy the trained model for **real-time fraud monitoring**.
* Monitor model performance regularly to detect data drift or degradation.
* Retrain the model periodically with new data to maintain accuracy.
* Investigate top features impacting fraud predictions to improve business rules and alerts.

---

## 🧰 Tech Stack

* **Languages:** Python
* **Libraries:** Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn, Statsmodels
* **Tools:** Jupyter Notebook
