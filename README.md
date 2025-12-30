# kaggle-diabetes-prediction
# 🩺 The Digital Physician: Ensemble Intelligence for Diabetes Prediction

![Python](https://img.shields.io/badge/python-3.11+-blue.svg)
![Kaggle](https://img.shields.io/badge/Kaggle-Competition-lightblue.svg)
![Machine Learning](https://img.shields.io/badge/ML-Ensemble-orange.svg)

## 📋 Project Overview
This project focuses on predicting the probability of a diabetes diagnosis using a massive dataset of **1,000,000 patients** (700,000 training records and 300,000 test records). 

Using a clinical perspective, I built a high-performance diagnostic tool by blending **lifestyle indicators** (diet, exercise, sleep) with **clinical vitals** (BMI, Blood Pressure, Cholesterol). The final solution utilizes an **Ensemble Consensus** of XGBoost and CatBoost to reach state-of-the-art predictive accuracy.

## 🧬 Key Clinical Insights
*   **The Genetic Anchor:** Feature importance analysis revealed that `family_history_diabetes` is the strongest predictor, accounting for nearly **78% of the model's decision-making power**.
*   **Behavioral Synergy:** Created a custom feature, `lifestyle_balance` (Diet Score + Physical Activity), which consistently outperformed individual clinical vitals.
*   **Universal Risk:** Diagnostic risk was found to be statistically uniform across demographic groups (Gender, Ethnicity), highlighting the universal predictive power of metabolic vitals.

## 🛠️ Tech Stack & Methods
*   **Languages:** Python
*   **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn
*   **Models:** 
    *   **XGBoost:** Leveraged manual label encoding and standard scaling.
    *   **CatBoost:** Utilized native categorical feature handling for high-fidelity pattern recognition.
*   **Ensemble Strategy:** 50/50 Probability Blending (Mean Ensemble).
*   **Metric:** ROC-AUC (Area Under the Receiver Operating Characteristic Curve).

## 🚀 The Pipeline
1.  **Patient Intake (EDA):** Visualizing target distribution and identifying imbalanced classes.
2.  **Vital Signs Check (Correlation):** Mapping the statistical links between BMI, Age, and Diabetes.
3.  **Pre-Op Room (Preprocessing):** `StandardScaler` for numeric normalization and `LabelEncoder` for categorical alignment.
4.  **The Diagnostic Brain (Modeling):**
    *   Initial XGBoost Baseline: **0.7237 AUC**
    *   CatBoost Specialist: **0.7248 AUC**
    *   **Final Ensemble Consensus: 0.7249 AUC**
5.  **Alignment Fix:** Solved a critical "Feature Alignment" issue to ensure XGBoost and CatBoost received data in their preferred formats.

## 📈 Results
The final model produces a nuanced **Risk Spectrum**, moving beyond simple "Yes/No" classifications to provide a detailed probability of diagnosis—essential for early medical intervention.

