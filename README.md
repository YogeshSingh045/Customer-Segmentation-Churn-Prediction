# Customer-Segmentation-Churn-Prediction

This project explores customer churn behavior and performs segmentation using machine learning techniques. The goal is to identify factors that influence customer churn and uncover customer segments for strategic retention efforts.

---

## 🧾 Table of Contents
- [Problem Statement](#problem-statement)
- [Dataset](#dataset)
- [Tools & Libraries Used](#tools--libraries-used)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Churn Prediction](#churn-prediction)
- [Customer Segmentation (KMeans)](#customer-segmentation-kmeans)
- [Model Evaluation](#model-evaluation)
- [Key Insights](#key-insights)
- [Dashboard & Deployment (Optional)](#dashboard--deployment-optional)
- [Conclusion](#conclusion)

---

## 📌 Problem Statement

The objective is to:
- Predict whether a customer is likely to churn or not.
- Understand which features most influence churn.
- Group customers into behavioral segments to assist in targeted marketing.

---

## 📂 Dataset

- **Rows:** 1000 customers  
- **Columns:** Age, Gender, Tenure, Monthly/Total Charges, Contract Type, Internet Service, Tech Support, and Churn
- **Source:** Synthetic or real-world inspired telecom data

---

## 🔧 Tools & Libraries Used

- Python, Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- Jupyter Notebook / Colab
- (Optional) Power BI / Tableau for dashboard

---

## 🧹 Data Preprocessing

- Handled missing values (`InternetService`)
- Dropped irrelevant fields (`CustomerID`)
- LabelEncoded categorical columns (`Gender`, `ContractType`, etc.)
- Feature-target split
- Train/test split (80/20)

---

## 📊 Exploratory Data Analysis (EDA)

- Churn rates visualized by:
  - Gender
  - Contract Type
  - Internet Service
  - Tech Support
- Swarmplots and boxplots of `TotalCharges` and `MonthlyCharges`
- Distribution of `Age` and `Tenure`

---

## 🤖 Churn Prediction

Tested multiple models:
- Logistic Regression ✅
- Random Forest ✅
- Decision Tree ✅
- Naive Bayes ✅
- KNN ✅
- SVM ✅
- Linear Regression (as baseline) ✅

### 📈 Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1 Score
- ROC AUC

### ✅ Feature Importance
```python
RandomForestClassifier().feature_importances_
