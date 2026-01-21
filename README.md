# Proactive Fraud Detection in Financial Transactions

## Project Overview
This project focuses on building a machine learning–based system to proactively detect fraudulent financial transactions. Using a large-scale transactional dataset containing over 6 million records, the objective is to identify fraud patterns, evaluate model performance under class imbalance, and propose actionable business interventions.

---

## Business Problem
Financial institutions face significant losses due to fraudulent activities. Traditional rule-based systems often fail to detect sophisticated fraud patterns. This project aims to:
- Predict fraudulent transactions accurately
- Minimize missed fraud cases (false negatives)
- Provide interpretable insights for decision-making

---

## 📂 Dataset
- **Rows:** ~6.3 million
- **Features:** Transaction type, amount, account balances, timestamps
- **Target:** `isFraud`

---

## 🔍 Approach
1. **Data Cleaning**
   - Handled structural missing values
   - Retained outliers due to their importance in fraud detection
   - Addressed multicollinearity using derived balance features

2. **Feature Engineering**
   - Balance difference features
   - Log-transformed transaction amounts
   - Transaction risk indicators

3. **Modeling**
   - Logistic Regression (baseline)
   - Random Forest (primary model)

4. **Evaluation**
   - Precision, Recall, F1-score
   - ROC-AUC
   - Confusion Matrix
   - Precision–Recall Curve

---

##  Key Insights
- Fraud is highly concentrated in **TRANSFER** and **CASH_OUT** transactions
- Large transaction amounts and balance inconsistencies are strong fraud indicators
- ML models significantly outperform rule-based fraud flags

---

## Business Recommendations
- Implement hybrid ML + rule-based fraud detection
- Apply risk-based authentication for high-value transfers
- Monitor behavioral deviations in real time

---

## How to Measure Success
- Reduction in fraud losses
- Improved fraud recall over time
- Controlled A/B testing of prevention strategies

---

##  Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

---

## Future Improvements
- XGBoost / LightGBM
- SHAP-based model interpretability
- Cost-sensitive learning

---

“Dataset not included due to size constraints.”

##  Author
Aditya Prakash
