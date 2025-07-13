# 🏥 Machine-Learning-ER-Healthcare

Using **machine learning**—specifically **Random Forest models** with **SHAP (SHapley Additive exPlanations)**—to predict ER wait times and walkouts in healthcare settings.

This project is part of a **Lean Six Sigma (Black Belt-level) initiative** aimed at addressing the persistent issue of long ER wait times and patient walkouts. By integrating the **DMAIC framework**, **Random Forest Machine Learning models**, and **Explainable AI techniques like SHAP**, the project provides data-driven insights for process improvement.

A **realistic synthetic dataset** was generated using **ChatGPT with logic-based simulation**, representing 250 emergency room cases. It enables modeling and analysis while respecting data privacy.

---

## 📂 Quick Access

- 👉 [View Jupyter Notebook](er_ml_analysis.ipynb)  
- 📊 [Download Dataset (CSV)](er_data.csv)

---

## 📁 Files Included

- `er_ml_analysis.ipynb` – Jupyter Notebook with **Random Forest**, SHAP, and visualizations  
- `er_data.csv` – AI-simulated ER dataset (250 records)

---

## 🎯 Project Goals

- Predict **ER Wait Time** (continuous) using **Random Forest Regression**  
- Predict **Patient Walkout** (binary) using **Random Forest Classification**  
- Interpret feature importance using **SHAP (SHapley Additive Explanations)**  
- Recommend improvement strategies based on model insights

> 🔬 SHAP, developed by **Scott Lundberg and Su-In Lee at the University of Washington**, provides a unified, model-agnostic approach to explain the output of machine learning models by quantifying each feature’s contribution to the prediction. SHAP has also been featured in MIT open courseware and AI curricula due to its widespread impact.

---

## 🧠 Techniques Used

- 📊 Statistical Analysis: **Jamovi**  
- 📈 ML Models: **Random Forest Regression** & **Random Forest Classification** (Scikit-learn)  
- 🧠 Model Explainability: **SHAP** (Summary and Interaction plots)  
- 📉 Visualization Tools: **Seaborn**, **Matplotlib**, **Tableau Public**  
- 🛠 Lean Six Sigma Tools: SIPOC, Control Charts, FMEA, Pareto, 5 Whys

---

## ✅ DMAIC Framework Alignment

| Phase     | Description |
|-----------|-------------|
| **Define**   | Identified ER wait time and patient walkouts as CTQ problems |
| **Measure**  | Analyzed simulated data across 250 cases |
| **Analyze**  | Used **Random Forest + SHAP** to identify predictors and root causes |
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

## 🔧 Improvements Proposed

All proposed improvements are **low-cost**, **realistic**, and **scalable**, supported by data insights and accessible technologies:

- Implement **triage optimization protocols** to prioritize high-severity patients  
- **Adjust staffing schedules** based on shift-level wait time patterns  
- Use **digital queue boards or SMS notifications** to reduce walkouts  
- Analyze and monitor process metrics using:
  - 🟢 **Jamovi** for statistical testing and effect sizes  
  - 🐍 **Python + Anaconda + VS Code** for modeling and automation  
  - 📊 **Tableau Public** and **Excel** for dashboards and control charts  
- Train frontline teams with **data-driven decision support tools**  
- Develop a lightweight **real-time prediction dashboard** with existing infrastructure

---

## 📷 Visuals and Plots

This project utilizes multiple visualizations to interpret model results and track ER process improvements:

- **SHAP Summary Plot**  
  Shows the contribution of each feature (e.g., Triage Level, Shift) to predictions of ER wait times made by **Random Forest**.

- **Actual vs. Predicted Wait Time Scatter Plot**  
  Measures **Random Forest** performance—well-aligned points indicate accurate predictions.

- **Control Chart**  
  Monitors ER wait times across shifts using statistical control limits.

- **Pareto Chart**  
  Ranks top causes of delays or walkouts to focus interventions.

- **SHAP Interaction Plot**  
  Explores how variables like Shift and Triage Level interact in **Random Forest predictions**.

All plots are created using **open-source Python libraries** and rendered inside the Jupyter Notebook. Visual outputs can be exported for use in dashboards, reports, or presentations.

---

## 📌 Use Cases

- ER operations and staffing optimization  
- Healthcare analytics and continuous improvement planning  
- Academic case studies for teaching ML and Lean Six Sigma  

---

## 📄 License

This repository is for educational and demonstration purposes only.  
© 2025 fritzbriones. Redistribution requires permission.

---
