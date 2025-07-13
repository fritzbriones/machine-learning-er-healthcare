# 🏥 Machine-Learning-ER-Healthcare

Using machine learning and SHAP to predict ER wait times and walkouts in healthcare settings

This project is part of a **Lean Six Sigma (Black Belt-level) initiative** aimed at addressing the persistent issue of long ER wait times and patient walkouts. By integrating the **DMAIC framework**, **Machine Learning**, and **Explainable AI (SHAP)**, the project provides data-driven insights for process improvement.

A **realistic synthetic dataset** was generated using **ChatGPT with logic-based simulation**, representing 250 emergency room cases. It enables modeling and analysis while respecting data privacy.

---

## 📁 Files Included

- `er_ml_analysis.ipynb` – Jupyter Notebook with machine learning, SHAP, and visualizations  
- `er_data.csv` – AI-simulated ER dataset (250 records)

---

## 🎯 Project Goals

- Predict **ER Wait Time** (continuous) using Random Forest Regression  
- Predict **Patient Walkout** (binary) using Random Forest Classification  
- Interpret feature importance using **SHAP values**  
- Recommend improvement strategies based on model insights

---

## 🧠 Techniques Used

- 📊 Descriptive Statistics & Visualization (Seaborn, Matplotlib)
- 📈 ML Models: Random Forest Regression & Classification (Scikit-learn)
- 🧠 Model Explainability using SHAP (Summary & Interaction plots)
- 🛠 Lean Six Sigma Tools: SIPOC, Control Charts, FMEA, Pareto, 5 Whys

---

## ✅ DMAIC Framework Alignment

| Phase     | Description |
|-----------|-------------|
| **Define**   | Identified ER wait time and patient walkouts as CTQ problems |
| **Measure**  | Analyzed simulated data across 250 cases |
| **Analyze**  | Used ML + SHAP to identify predictors and root causes |
| **Improve**  | Proposed actions: triage optimization, shift-based staffing |
| **Control**  | Metrics tracked via visual charts and modeling feedback |

---

## 📊 Key Insights

| **Indicator**                    | **Baseline** | **Proposed Outcome** | **% Change**        |
|----------------------------------|--------------|-----------------------|---------------------|
| Average Wait Time               | 169 mins     | 128 mins (target)     | ↓ 24.3%             |
| % Patients Waiting >150 mins    | 40%          | 18%                   | ↓ 55%               |
| Walkout Rate                    | 35%          | 14%                   | ↓ 60%               |
| Sigma Level                     | 1.85         | 2.55                  | ↑ Improved Capability |
| Estimated Annual Savings        | —            | ₱520,000 (projected)  | Cost Avoidance      |

> 📌 *Figures represent expected improvements based on model findings, not actual post-intervention data.*

---

## 🧠 SHAP Highlights

- **Triage Level**: Strongest driver—higher severity linked to shorter waits
- **Shift**: Night shifts associated with higher predicted wait times
- **SHAP Interaction**: Long waits during night shifts have magnified effects

---

## 📌 Use Cases

- ER operations and staffing optimization  
- Healthcare analytics and improvement planning  
- Academic case studies in ML and Lean Six Sigma

---

## 📄 License

This repository is for educational and demonstration purposes only.  
© 2025 fritzbriones. Redistribution requires permission.

---
