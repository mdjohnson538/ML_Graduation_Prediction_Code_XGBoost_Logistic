# High School Graduation Prediction (UNO x Millard Public Schools)

This repository contains the R Markdown code developed as part of the **University of Nebraska–Omaha Applied Machine Learning (ISQA 8720)** course in collaboration with **Millard Public Schools**.  

The goal of the project was to use real student academic, behavioral, and socio-economic data to **predict high school graduation likelihood** and help school staff identify students most at risk of not graduating.

---

## 📊 Project Overview
- **Dataset:** ~1,300 students from Millard Public Schools (2019–2024 cohort)  
- **Features:** GPA, credits earned, Pre-ACT scores, absences, suspensions, counselor visits, free/reduced lunch, and more  
- **Problem:** Strong class imbalance (97% graduated vs. 3% did not graduate) required careful modeling to prioritize recall of at-risk students  
- **Models tested:**
  - Logistic Regression  
  - Random Forest  
  - Neural Network (CNN-LSTM)  
  - XGBoost  
  - Two-stage hybrid (XGBoost + LASSO Logistic Regression)

---

## 🚀 Key Results
- **Best-performing model:** Two-stage approach (XGBoost + LASSO Logistic Regression)  
- **Accuracy:** 99% on test data  
- **Focus:** Maximized recall to minimize false negatives (students at risk incorrectly predicted to graduate)  
- **Interpretability:** Used SHAP values and Partial Dependence Plots to identify key predictors (GPA, GPA change, unexcused absences, Pre-ACT score, counselor visits, etc.)  

---

## 📂 Files
- `ML_Graduation_Prediction_Code_XGBoost_Logistic.Rmd` – Main R Markdown script with preprocessing, feature engineering, modeling, and evaluation  

---

## 🏫 Impact
The Millard Public Schools district intends to integrate this predictive model into a **dashboard for staff**, allowing earlier interventions and more tailored support for students most at risk of not graduating.
