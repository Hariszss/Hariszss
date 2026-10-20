# Charalampos Zisis

Data Analyst at Amsterdam UMC and MSc Applied Data Science graduate (Utrecht University, 2026). I prepare and validate complex datasets and build predictive models, most recently on clinical registry data and on credit risk. Math background (Statistics & Operational Research, University of Patras) → data science, with a focus on predictive modelling, risk analytics and healthcare data.

I like problems where the model has to be trusted by people who aren't data scientists: clinicians, risk officers, auditors. That means interpretability and honest evaluation matter as much as raw accuracy.

---

### Featured project: MSc Thesis

**[Staged ML Prediction of Postoperative Complications After Esophagectomy](https://github.com/Hariszss/esophagectomy-thesis)**
A staged machine learning pipeline (LASSO, Random Forest, XGBoost) predicting surgical complications from the Dutch nationwide DUCA registry (N=1,181 patients, Amsterdam UMC).

- **Staged design**: predictors added cumulatively across 4 clinical decision points (demographics → comorbidity → tumour/treatment → surgical factors), quantifying *when* in the patient pathway risk becomes predictable, not just whether it is.
- **Leakage-safe evaluation**: 5-fold stratified CV with imputation fit per-fold; hyperparameter sensitivity checked across a full grid (AUC spread of 0.006, confirming the result isn't a tuning artifact).
- **Interpretability**: SHAP (TreeExplainer) to identify and sanity-check the drivers behind model output, including catching a confounded predictor (anastomosis location acting as a proxy for surgical approach) before over-claiming a causal story.
- **Model vs. human judgment**: benchmarked the data-driven model against real clinical risk assessments: AUC 0.629 (model) vs. 0.536 (physiotherapist qualitative classification) on the same patients.
- **NLP-derived features**: incorporated functioning scores extracted from unstructured clinical notes (ICF framework) as a supplementary signal.

---

### Featured project: Credit Risk Analytics

**[Banking Credit Risk Analytics & Default Prediction](https://github.com/Hariszss/banking-credit-risk-analytics)**
End-to-end credit risk project on 30,000 credit card customers: Python, SQL Server, Power BI (DAX) and scikit-learn.

- **Data warehouse**: validated raw data in Python, then loaded it into a SQL Server star schema (staging → core → analytics) with reconciliation checks and analytics views (window functions, roll rates).
- **Default prediction**: gradient boosting chosen over logistic regression and a rule-based segmentation using decision rules fixed in advance. Gini 0.56 vs 0.45 on a held-out test set, well calibrated (6,625 expected vs 6,636 actual defaults).
- **Fairness**: sex and marital status excluded after showing they add no predictive value, with outcomes checked by group anyway.
- **Power BI**: 4-page report (portfolio KPIs, segment risk, delinquency trends, early-warning watch list), stored as a Power BI Project (TMDL/PBIR) under version control.
- **Data issues reported, not hidden**: a repayment-status coding break that would have produced a false delinquency spike, so trends use a definition that stays comparable over time.

---

### Other projects

- **[Hospital Readmission Prediction](https://github.com/Hariszss/hospital-readmission)**: 30-day readmission risk in diabetic patients, gradient boosting + subgroup analysis
- **[Diabetes Prediction ML](https://github.com/Hariszss/diabetes-prediction-ml)**: classification benchmark (logistic regression, SVM, random forest) with full evaluation metrics
- **[Gender Bias in Multilingual mBERT](https://github.com/Hariszss/gender-bias-multilingual-mBERT)**: template-based probing and corpus analysis of bias across five languages

---

### Technical skills

**Languages:** Python, R, SQL
**ML:** scikit-learn, XGBoost, SHAP, PyTorch, HuggingFace
**Data & BI:** SQL Server (T-SQL, window functions, star schemas), Power BI (DAX, Power Query), pandas
**Methods:** Risk modeling & staged prediction, probability-of-default modelling and calibration, model interpretability, cross-validation design, statistical testing (Wilcoxon, Mann-Whitney, chi-square)
**Domains:** Healthcare analytics & epidemiology, clinical/registry data, credit risk, NLP, stakeholder-facing reporting

---

### Background

- Data Analyst, Amsterdam UMC (Sep 2026–present); Data Science Intern (Apr–Aug 2026)
- MSc Applied Data Science, Utrecht University (2025–2026)
- BSc Mathematics (Statistics & Operational Research), University of Patras, Greece (2025)
- Erasmus+ exchange, University of Extremadura, Spain

---

### Reach me

[LinkedIn](https://www.linkedin.com/in/charalampos-zisis-8a3b40275/) · haris.zhshs@gmail.com
