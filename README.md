# Credit Risk Prediction Using Machine Learning

## 📌 Project Overview
This project focuses on predicting **loan default risk** using machine learning techniques.  
The objective is to help financial institutions **reduce loan default rates** by making informed, data-driven lending decisions.

The model classifies applicants as **low, medium, or high credit risk** based on financial, demographic, and loan-related features.

---

## 🎯 Objectives
- Analyze customer and loan characteristics using EDA
- Identify key factors influencing loan default
- Build a machine learning model for credit risk prediction
- Evaluate model performance using appropriate metrics
- Provide business insights to support risk-based decision making

---

## 🗂 Dataset Description
The dataset includes:
- Demographic features (Age, Education, Marital Status)
- Financial features (Income, Credit Score, DTI Ratio)
- Employment details (Employment Type, Months Employed)
- Loan information (Loan Amount, Interest Rate, Loan Term)
- Target variable:  
  - `0` → Non-Defaulter  
  - `1` → Defaulter

---

## 🔍 Exploratory Data Analysis (EDA)
Key insights from EDA:
- The dataset is **highly imbalanced**
- Defaulters are generally:
  - Younger
  - Lower income
  - Higher interest rates
  - Higher debt-to-income ratios
  - Shorter employment history
- No single feature explains default risk alone

Visualizations used:
- Distribution plots
- Boxplots
- KDE plots
- Correlation heatmap
- Feature importance
- Confusion matrix
- ROC curve

---

## ⚙️ Data Preprocessing
- Missing value handling
- One-hot encoding using `pd.get_dummies()`
- Train-test split with stratification
- Feature scaling using `StandardScaler` (where required)

---

## 🤖 Model Used
### Random Forest Classifier
Chosen because it:
- Handles non-linear relationships
- Works well with imbalanced data
- Does not require feature scaling
- Provides feature importance for explainability

---

## 📊 Model Evaluation
Evaluation metrics:
- Confusion Matrix
- ROC Curve
- AUC Score: **0.74**

Key observation:
- Model predicts non-defaulters very well
- Recall for defaulters is low due to class imbalance
- Threshold tuning is required for real-world deployment

---

## 📈 Feature Importance
Top influencing features:
1. Income
2. Interest Rate
3. Loan Amount
4. Age
5. Credit Score
6. Months Employed
7. DTI Ratio

This confirms that **financial stability is the strongest driver of credit risk**.

---

## 🧠 Business Impact
- Enables **risk-based loan approval**
- Helps reduce financial losses
- Supports proactive monitoring of high-risk applicants
- Improves decision consistency and transparency

---

## 🚀 Future Improvements
- Handle class imbalance using SMOTE or cost-sensitive learning
- Threshold optimization for better defaulter recall
- Use advanced models like XGBoost or LightGBM
- Deploy model as an API or dashboard

---

## 🛠 Tech Stack
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📄 License
This project is for educational and research purposes.
