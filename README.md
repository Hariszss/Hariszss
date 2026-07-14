# Charalampos Zisis

MSc Applied Data Science student (Utrecht University) currently interning as a Data Scientist at Amsterdam UMC, where I build and validate machine learning models on real clinical registry data. Math background (Statistics & Operational Research, University of Patras) → data science, with a focus on the intersection of machine learning, NLP, and healthcare data.

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

### Other projects

- **[Hospital Readmission Prediction](https://github.com/Hariszss/hospital-readmission)**: 30-day readmission risk in diabetic patients, gradient boosting + subgroup analysis
- **[Diabetes Prediction ML](https://github.com/Hariszss/diabetes-prediction-ml)**: classification benchmark (logistic regression, SVM, random forest) with full evaluation metrics
- **[Gender Bias in Multilingual mBERT](https://github.com/Hariszss/gender-bias-multilingual-mBERT)**: template-based probing and corpus analysis of bias across five languages

---

### Technical skills

**Languages:** Python, R, SQL
**ML:** scikit-learn, XGBoost, SHAP, PyTorch, HuggingFace
**Methods:** Risk modeling & staged prediction, model interpretability, cross-validation design, statistical testing (Wilcoxon, Mann-Whitney, chi-square)
**Domains:** Healthcare analytics & epidemiology, clinical/registry data, NLP, stakeholder-facing reporting

---

### Background

- MSc Applied Data Science, Utrecht University (2025–present)
- BSc Mathematics (Statistics & Operational Research), University of Patras, Greece (2025)
- Erasmus+ exchange, University of Extremadura, Spain

---

### Reach me

[LinkedIn](https://www.linkedin.com/in/charalampos-zisis-8a3b40275/) · haris.zhshs@gmail.com
