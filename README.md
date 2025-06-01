# 🕵️‍♀️ Credit Card Fraud Detection with XGBoost

This project is a machine learning pipeline designed to detect fraudulent credit card transactions using Python, Spark, and XGBoost. It focuses on handling class imbalance and improving model recall to help minimize undetected fraud.

## 📂 Dataset

Sourced from [Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud), the dataset contains:

- 284,807 transactions
- 492 frauds (0.17%)
- Anonymized, PCA-transformed features + `Time` and `Amount`

## ⚙️ Workflow

The project includes the following stages:

### 🔹 Load Dataset
- Loaded with Spark for scalability

### 🔍 Exploratory Data Analysis (EDA)
- Checked for null values
- Visualized fraud distribution
- Explored `Amount` and `Time` patterns

### 🧹 Preprocessing & Feature Engineering
- Log transformation of `Amount`
- Applied **SMOTE** to handle class imbalance
- Feature scaling and cleanup

### 🧠 Model Training
- Used **XGBoostClassifier**
- Tuned hyperparameters for performance
- Trained on balanced data

### 📊 Evaluation & Results
- Focused on **Recall**
- Used confusion matrix, ROC AUC, and classification report
- Visualized feature importance

## ✅ Key Results

- **High Recall** achieved on test set
- Strong performance in imbalanced conditions
- Clean, scalable pipeline for future integration

## 🚀 How to Use

1. Clone this repo
2. Run the notebook step-by-step (Databricks or Jupyter compatible)
3. Install missing libraries using `pip` as needed

## 🔮 Future Plans

- Deploy as a simple web app for real-time fraud checks
- Integrate into a streaming pipeline (Spark Structured Streaming)
- Test other anomaly detection models
