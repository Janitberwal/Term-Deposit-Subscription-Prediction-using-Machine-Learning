# 💼 Term Deposit Subscription Prediction using Machine Learning

This project aims to help banks predict whether a customer is likely to subscribe to a **term deposit** based on historical marketing campaign data. By building machine learning models, we enable smarter targeting and more efficient marketing efforts.

---

## 📌 Problem Statement

**Can we predict whether a customer will subscribe to a term deposit based on their profile and interaction history with the bank?**

Banks often run marketing campaigns to promote term deposits, but reaching out to uninterested customers leads to wasted effort and cost. We aim to build a predictive model that helps the bank identify potential subscribers, increasing the campaign's success rate.

---

## 📊 Dataset Overview

- **Source**: Bank Marketing Dataset
- **Target Variable**: `y` — whether the client subscribed to a term deposit (`yes` or `no`)
- **Size**: ~45,000 rows and multiple features
- **Imbalance**: The dataset was highly imbalanced, with far more "no" outcomes than "yes"

---

## 🔍 EDA & Data Cleaning

- No missing or null values
- Visualizations (bar plots, heatmaps) used for feature understanding
- **Important Features Identified**:
  - `duration` — duration of last contact
  - `campaign` — number of contacts during the campaign
  - `previous` — number of contacts before this campaign

---

## ⚖️ Handling Class Imbalance

- Used **SMOTE (Synthetic Minority Oversampling Technique)** to balance the dataset
- Helped models learn better and avoid bias toward the majority class

---

## 🧠 Machine Learning Models Used

1. **Logistic Regression**
2. **Decision Tree**
3. **Random Forest** ✅ (Best performer)

All models were trained on the balanced dataset.

---

## 📈 Evaluation Metrics

We used the following metrics to evaluate models:

- **Accuracy** — Overall correctness
- **Precision** — How many predicted positives were actual positives
- **Recall** — How many actual positives were captured
- **Confusion Matrix** — Breakdown of predictions

### ✅ Best Model: Random Forest
📌 Business Impact

By using this model:
- Banks can **focus their marketing** on customers likely to subscribe
- **Reduce cost** and effort in contacting uninterested customers
- **Improve overall campaign success rate**

---

## 🧾 Conclusion

We successfully built a classification system to help banks **predict term deposit subscriptions**. After balancing the dataset and testing multiple models, **Random Forest** proved to be the most effective. This solution can significantly **optimize marketing strategies** and improve customer targeting for financial institutions.

---

## 💻 Technologies Used

- Python 🐍
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- SMOTE (from imbalanced-learn)
