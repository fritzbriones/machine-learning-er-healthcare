# 🏥 Machine-Learning-ER-Healthcare

Using **machine learning**—specifically **Random Forest models** coupled with **SHAP (SHapley Additive exPlanations)**—to predict ER wait times and patient walkouts in healthcare settings.

This project is part of a **Lean Six Sigma Black Belt-level initiative** aimed at addressing the persistent issue of long ER wait times and patient walkouts. By integrating the **DMAIC framework**, **Random Forest machine learning models**, and explainable AI techniques like **SHAP**, the project delivers actionable, data-driven insights to optimize ER processes and enhance patient outcomes.

A **realistic synthetic dataset** was generated using **ChatGPT with logic-based simulation**, representing 250 emergency room cases. This approach allows for robust modeling and analysis while fully preserving patient privacy.

---

## 📊 Data Generation & Simulation

Both the **baseline** and **post-intervention datasets** are synthetically generated through ChatGPT-powered logic-based simulation:

- The **baseline dataset** models typical ER patient flows, wait times, and walkouts prior to any interventions.  
- The **post-intervention dataset** is simulated by applying modeled Lean Six Sigma interventions—such as triage optimization, shift-based staffing adjustments, and digital queue management—to the baseline data, reflecting expected operational improvements.

This method ensures realistic, privacy-compliant data for predictive modeling and comparative evaluation of process improvements.

---

## 📂 Quick Access

- 👉 [Explore Jupyter Notebook](er_ml_analysis.ipynb)  
- 📊 [Download Baseline Dataset (CSV)](er_data.csv)  
- 📊 [Download Post-Intervention Dataset (CSV)](post_intervention_er_data.csv)

---

## 📁 Files Included

| Filename                     | Description                                                        |
|------------------------------|--------------------------------------------------------------------|
| `er_ml_analysis.ipynb`       | Jupyter Notebook with **Random Forest**, SHAP explainability, and visualizations |
| `er_data.csv`                | Synthetic baseline ER dataset (250 simulated patient records)      |
| `post_intervention_er_data.csv` | Synthetic post-intervention dataset modeling Lean Six Sigma improvements |

---

## 🎯 Project Goals

- Predict **ER Wait Time** (continuous) using **Random Forest Regression**  
- Predict **Patient Walkout** (binary) using **Random Forest Classification**  
- Interpret feature importance with **SHAP (SHapley Additive exPlanations)**—a model-agnostic explainability method based on **Shapley values** from cooperative game theory  
- Recommend scalable, low-cost process improvements based on model insights

> 🔬 **SHAP**, developed by Scott Lundberg and Su-In Lee (University of Washington), provides a unified framework to explain individual and global model predictions by quantifying each feature’s contribution, enhancing transparency and trustworthiness in AI-driven healthcare solutions.

---

## 🧠 Techniques Used

- **Statistical Analysis:** Jamovi  
- **Machine Learning Models:** Random Forest Regression and Classification (Scikit-learn)  
- **Explainability:** SHAP (summary and interaction plots)  
- **Visualization:** Seaborn, Matplotlib, Tableau Public  
- **Lean Six Sigma Tools:** SIPOC, Control Charts, FMEA, Pareto Analysis, 5 Whys

---

## ✅ DMAIC Framework Alignment

| Phase     | Description                                                                        |
|-----------|------------------------------------------------------------------------------------|
| **Define**   | Identified ER wait times and patient walkouts as critical-to-quality (CTQ) issues |
| **Measure**  | Analyzed 250 simulated ER patient cases for baseline performance                 |
| **Analyze**  | Employed **Random Forest + SHAP** to identify predictors and root causes         |
| **Improve**  | Proposed triage optimization, shift-based staffing, and digital queue management |
| **Control**  | Established monitoring via control charts and ongoing data-driven feedback       |

---

## 📊 Key Insights & Results

| Indicator                      | Baseline       | Post-Intervention             | % Change           | Impact Summary                                                                                   |
|-------------------------------|----------------|------------------------------|--------------------|------------------------------------------------------------------------------------------------|
| **Average Wait Time (minutes)**| 169.06         | 127.92                       | ↓ 24.3%            | Approximately 41-minute reduction per patient following triage restructuring and digitization  |
| **% Patients Waiting >150 mins**| 75.2%          | 14.8%                        | ↓ 80.3%            | Significant drop in excessive wait times identified as defects in both datasets                 |
| **Walkout Rate**               | 35.2%          | 18.4%                        | ↓ 47.7%            | Verified via Chi-square test; reflects improved patient retention and satisfaction               |
| **Sigma Level**                | 1.85 σ         | 2.55 σ                       | ↑ Enhanced Capability | Calculated using NORMSINV(1 - defect rate) + 1.5; defect rate dropped from ~31% to 14.8%       |
| **Estimated Annual Savings**   | —              | ₱420,000 (~$7,500 USD)       | Cost Avoidance     | Projected savings from 16.8% fewer walkouts, capturing retained revenue and increased throughput |

---

## 🧠 SHAP Highlights

- **Triage Level:** Strongest predictor; higher severity (lower triage scores) correlates with shorter waits  
- **Shift:** Night shifts are associated with increased predicted wait times  
- **Feature Interaction:** Combination of night shift and triage level magnifies wait time effects

---

## 🔧 Proposed Improvements

All recommended interventions are **low-cost, scalable, and data-backed**:

- Implement **triage optimization protocols** prioritizing high-acuity patients  
- Adjust **staffing schedules based on shift-level wait time patterns**  
- Deploy **digital queue boards and SMS notifications** to reduce walkouts  
- Monitor KPIs using:  
  - 🟢 **Jamovi** for statistical validation  
  - 🐍 **Python (Anaconda + VS Code)** for model development and automation  
  - 📊 **Tableau Public** and **Excel** for dashboards and control charts  
- Train frontline staff on **data-driven decision support** tools  
- Develop **real-time predictive dashboards** integrated into existing hospital systems

---

## 📷 Visualizations

Visual tools included:

- **SHAP Summary Plot:** Feature importance and impact on wait time predictions  
- **Actual vs. Predicted Scatter Plot:** Model accuracy assessment  
- **Control Chart:** Monitoring wait times and detecting variations  
- **Pareto Chart:** Ranking top causes of delays and walkouts  
- **SHAP Interaction Plot:** Exploring feature interactions affecting predictions

All plots are generated using open-source Python libraries within the Jupyter Notebook and can be exported for reports and presentations.

---

## 📌 Use Cases

- ER operations optimization and staffing planning  
- Healthcare analytics for quality improvement  
- Academic and professional case studies on ML + Lean Six Sigma integration

---

## 📄 License

This repository is intended for **educational and demonstration purposes only**.  
© 2025 fritzbriones. Redistribution or commercial use requires prior permission.

---
