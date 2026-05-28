# 💳 Credit Risk Modeling End-to-End Project

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Scikit-Learn](https://img.shields.io/badge/ML-ScikitLearn-orange)
![XGBoost](https://img.shields.io/badge/Model-XGBoost-green)
![MLflow](https://img.shields.io/badge/Tracking-MLflow-blueviolet)
![Streamlit](https://img.shields.io/badge/App-Streamlit-red)
![Status](https://img.shields.io/badge/Project-Production--Ready-success)

---

## 📌 Overview

This project builds a **production-ready Credit Risk Prediction System** to classify loan applicants as **good or bad credit risks**.

It combines **domain-driven feature engineering (WOE & IV)** with machine learning models and deploys the final solution using a **Streamlit web application**.

---

## 🌐 Live Demo

🚀 Try the app:
👉 https://codebasics-ml-project-credit-risk-score.streamlit.app/

💡 Enter applicant details to predict the probability of loan default in real time.

---

## 🎯 Problem Statement

Financial institutions must **minimize default risk** while approving loans.
This project predicts the probability of customer default, enabling **data-driven lending decisions**.

---

## 📊 Dataset

* Customer demographic, financial, and behavioral features
* Target variable:

  * **0 → Non-default (Good)**
  * **1 → Default (Bad)**

---

## ⚙️ Approach

### 🔹 Data Preprocessing

* Missing value handling
* Binning of continuous variables
* Data cleaning and transformation

### 🔹 Feature Engineering (Key Highlight 🚀)

* Applied **Weight of Evidence (WOE)** transformation
* Used **Information Value (IV)** for feature selection
* Ensured model interpretability aligned with credit risk standards

### 🔹 Model Building

* Logistic Regression (interpretable baseline)
* Random Forest (non-linear patterns)
* XGBoost (performance optimization)

### 🔹 Model Evaluation

* ROC-AUC
* Gini Coefficient
* KS Statistic
* Recall

---

## 📊 Model Performance

| Model               | ROC-AUC | Gini  | KS Score | Recall |
| ------------------- |---------|-------|----------|--------|
| Logistic Regression | 0.98    | 0.97 | 85.9%    | 0.94   |
| XGBoost             | 0.99    | 0.97 | 86.4%    | 0.87   |

---

## 🏆 Model Selection

Both models demonstrate strong predictive performance.

* **XGBoost** shows slightly higher ROC-AUC and Gini, indicating better overall discrimination
* **Logistic Regression** provides higher recall and better interpretability

👉 The final choice depends on business objectives:

* Prioritize recall → Logistic Regression
* Maximize overall performance → XGBoost

---

## 📊 Key Insights

* **Loan-to-income ratio** is the strongest predictor of default risk
* **Credit utilization** indicates financial stress and higher risk
* **Past delinquency behavior** strongly predicts future defaults
* **Home ownership** reduces default probability
* **WOE analysis** enables clear risk segmentation across customer groups

---

## 📓 Notebook

The full analysis, feature engineering (WOE/IV), and model development can be found here:

👉 `notebooks/credit_risk_analysis.ipynb`

---
## 🔁 Experiment Tracking

* Used MLflow to:
  * Track experiments
  * Log parameters & metrics
  * Compare multiple model runs
---

## 🚀 Deployment

Built an interactive **Streamlit application** that allows users to:

* Input applicant details
* Receive real-time credit risk predictions

---

## 🧪 How to Run Locally

```bash
git clone https://github.com/your-username/ML-Project-Credit-Risk-Score
cd ML-Project-Credit-Risk-Score

pip install -r requirements.txt

streamlit run main.py
```

---

## 🛠️ Tech Stack

* Python (Pandas, NumPy, Scikit-learn)
* XGBoost
* MLflow
* Streamlit
* Matplotlib / Seaborn

---

## 🔮 Future Improvements

* Threshold tuning for optimized business decisions
* Model monitoring and drift detection
* CI/CD pipeline for automated deployment

---

## ⭐ Key Highlights

✔ End-to-end ML pipeline
✔ Industry-standard credit risk techniques (WOE, IV, KS, Gini)
✔ Strong model performance (AUC ~0.98)
✔ Real-time prediction using Streamlit

---

## 📬 Contact

If you found this project interesting, feel free to connect!
