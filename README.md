# 🧠 Financial Risk Prediction Using Ensemble Learning

This project aims to predict an individual's financial risk using demographic and financial attributes. It leverages **Exploratory Data Analysis (EDA)** and an **ensemble machine learning model (Random Forest Classifier)** to classify individuals as **risky** or **safe**.

---

## 📁 Dataset

- Source: `risk_behavior_features.csv`
- Contains 73 records with attributes like Age, Gender, Education Level, Income, Credit Score, Debt-to-Income Ratio, and more.
- A binary target column `Financial_Risk` is created from `Defaults Records`:
  - `1`: Risky (has defaulted before)
  - `0`: Safe (no defaults)

---

## 🔍 Features Used

- **Numerical:** Age, Number of Dependents, Income, Credit Score, Debt-to-Income Ratio, Assets Value, Defaults Records, Years in Current Job  
- **Categorical:** Gender, Education Level, Marital Status, Employment Status

---

## 🧪 Process Overview

### 📊 Data Preprocessing
- Scaled numeric features using `MinMaxScaler`
- Encoded categorical features using `OneHotEncoder`

### 🔎 Exploratory Data Analysis (EDA)
- Visualized risk distribution
- Analyzed feature correlations to identify risk indicators

### 🧠 Model Training
- Trained `RandomForestClassifier` to classify financial risk
- Evaluated using:
  - Accuracy
  - Confusion matrix
  - Classification report (precision, recall, F1-score)

### 📈 Feature Importance
- Identified key drivers of financial risk such as:
  - Credit Score
  - Debt-to-Income Ratio
  - Defaults Records

### 🔮 Prediction on New Data
- Used preprocessing pipeline to predict financial risk for new, unseen data

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/financial-risk-prediction.git
   cd financial-risk-prediction
