# Customer-Churn-Prediction

This project uses machine learning to predict whether a customer will leave a telecom company (churn) based on usage and demographic data.

---

## 🎯 Objective
Build a classification model to identify customers at risk of churn, enabling targeted retention strategies.

---

## 📂 Dataset
- Source: [Telco Customer Churn Dataset on Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- Rows: ~7,000
- Target variable: `Churn` (Yes/No → 1/0)

---

## 🔍 EDA Highlights
- Class imbalance: ~26% customers churned
- `Contract`, `MonthlyCharges`, `tenure`, and `InternetService` showed strong patterns with churn

---

## 🧹 Preprocessing
- Dropped `customerID`
- Converted `TotalCharges` to numeric and handled missing values
- Label encoded all categorical columns
- Train-test split: 80% training, 20% testing (stratified)

---

## 🤖 Models Used
| Model               | Accuracy | AUC Score |
|--------------------|----------|-----------|
| Logistic Regression | ~80%     | ~0.84     |
| Random Forest       | ~81%     | ~0.85     |

---

## 📊 Evaluation Metrics
- Accuracy, Precision, Recall, F1-score
- Confusion Matrix
- ROC Curve & AUC
- Feature Importance (from Random Forest)

---

## 📌 Top Important Features
- `tenure`
- `Contract`
- `MonthlyCharges`
- `OnlineSecurity`
- `TechSupport`

---

## 📁 Project Structure
customer-churn-prediction/
│
├── WA_Fn-UseC_-Telco-Customer-Churn.csv
├── churn_prediction.ipynb
├── README.md
└── requirements.txt

## 💡 Skills Demonstrated
- EDA & Data Cleaning
- Encoding & Train-Test Split
- Handling Class Imbalance
- Binary Classification Models
- Evaluation using ROC-AUC & Feature Importance
