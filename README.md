# 🧠 Employee Attrition Prediction

This project aims to predict which employees are likely to leave a company using supervised machine learning models. By identifying at-risk employees, organizations can take proactive steps to improve retention, reduce turnover, and minimize the costs of hiring and training.

---

## 📁 Dataset

We use the **IBM HR Analytics Employee Attrition & Performance** dataset, which includes demographic, performance, compensation, and satisfaction information for 1,470 employees.

**Target Variable:**
- `Attrition` — Whether the employee left the company (Yes/No)

**Key Features:**
- Age, Gender, Department, DistanceFromHome  
- JobRole, OverTime, MonthlyIncome, YearsAtCompany  
- Satisfaction metrics (JobSatisfaction, EnvironmentSatisfaction, etc.)

---

## 🔍 Project Steps

1. **Data Preprocessing**
   - Label encoding of the target variable
   - One-hot encoding of categorical features
   - Feature selection and cleaning

2. **Exploratory Data Analysis (EDA)**
   - Visualizations to understand feature distributions and correlations
   - KDE plots to reveal interactions between variables

3. **Handling Class Imbalance**
   - Used **SMOTE (Synthetic Minority Oversampling Technique)** to balance classes in the training data

4. **Model Training**
   - Trained three models:
     - Random Forest Classifier
     - XGBoost Classifier
     - Gradient Boosting Classifier

5. **Model Evaluation**
   - Metrics used:
     - Accuracy
     - Precision, Recall
     - F1 Score
     - ROC-AUC Score

---

## 📊 Key Results

- Class imbalance addressed using SMOTE
- Best model: Random Forest with 85.7% accuracy

---

## 🔧 Tools & Libraries

- Python 3.x
- `pandas`, `numpy`, `matplotlib`, `seaborn`
- `scikit-learn`, `xgboost`, `imbalanced-learn`
- `plotly` (for interactive EDA)
- `SMOTE` for handling imbalance

---

## 🚀 Future Improvements

- Incorporate model explainability (SHAP, LIME)
- Deploy model as an API for HR dashboard integration
- Include time-based features (e.g., trends in satisfaction)
- Test with real-world HR data (with privacy considerations)
