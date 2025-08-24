# 📊 Customer Churn Prediction with Machine Learning

Customer churn is one of the biggest challenges for subscription-based businesses.
This project develops an **end-to-end machine learning pipeline** to predict churn and simulate the **ROI of targeted retention campaigns**.

---

## 🌟 Key Features

* **Data Cleaning & Preprocessing**

  * Removal of duplicates and irrelevant IDs
  * Conversion of categorical features (e.g., area, marital status)
  * Feature scaling for continuous variables
  * Handling missing values with appropriate strategies

* **Exploratory Data Analysis (EDA)**

  * Distribution plots of churn vs non-churn groups
  * Correlation heatmaps of key features (e.g., usage, billing, support calls)
  * Feature importance ranking from tree-based models

* **Machine Learning Models**

  * Compared multiple classifiers:
    Logistic Regression, Random Forest, Gradient Boosting, XGBoost, LightGBM
  * Applied **probability calibration** to improve threshold-based decisions

* **Class Imbalance Handling**

  * SMOTE oversampling
  * Class weighting strategies for imbalance

* **Hyperparameter Optimization**

  * RandomizedSearchCV
  * BayesSearchCV for advanced tuning

* **Model Evaluation**

  * Confusion Matrix & Classification Report
  * ROC-AUC & PR-AUC for imbalanced classification
  * Calibration curves & Brier score

* **Business ROI Simulation**

  * Modeled retention campaign targeting top churn-risk customers
  * Calculated **saved revenue vs campaign cost**
  * Demonstrated ROI improvement compared to random targeting

---

## 📊 Results

* **HistGradientBoosting** achieved the highest ROC-AUC (≈0.87)
* Oversampling + calibration improved recall on minority class (churners)
* ROI Simulation:

  * Targeting top 20% high-risk customers → **ROI ≈ 2.0x**
  * Retention campaigns are **profitable when precision > 0.5**

---

## 🛠️ Tech Stack

* **Python**: pandas, numpy, matplotlib, seaborn
* **ML**: scikit-learn, xgboost, lightgbm, imbalanced-learn
* **Optimization**: scikit-optimize (BayesSearchCV)
* **Explainability**: shap

---

## 🚀 Future Improvements

* Deploy model as an API for live churn scoring
* Uplift modeling for causal campaign impact
* Fairness checks to avoid demographic bias
* Automated monitoring of churn model performance

---

## 📢 About

This project is designed as a **portfolio-ready case study**, demonstrating senior-level skills:

* **End-to-end ML workflow** (data → models → business impact)
* **Handling real-world dataset challenges** (imbalance, calibration, feature engineering)
* **Business framing** with ROI simulation, not just accuracy
