# Charalampos Zisis

Data Analyst at Amsterdam UMC and MSc Applied Data Science graduate (Utrecht University, 2026). I prepare and validate complex datasets and build predictive models, most recently on clinical registry data, credit risk and transaction monitoring. Math background (Statistics & Operational Research, University of Patras) → data science, with a focus on risk analytics, financial crime detection and healthcare data.

I like problems where the model has to be trusted by people who aren't data scientists: clinicians, risk officers, auditors. That means interpretability and honest evaluation matter as much as raw accuracy.

---

### Featured project: Transaction Monitoring

**[Understanding False Positives in Transaction Monitoring](https://github.com/Hariszss/aml-transaction-monitoring)**
How simple monitoring rules trade alert volume against detection, using PySpark on IBM's synthetic AML data (about 5 million transactions).

- **PySpark and Spark SQL**: cleaning, currency conversion and account-history features (24-hour and 7-day windows) that use only past transactions, so no future information leaks into an alert.
- **Transparent rules with fair thresholds**: three rules (large amount, amount vs the sender's own history, receiver fan-in), with thresholds set to fixed alert budgets (0.1%, 1%, 5%) on a validation period and evaluated once on a later, held-out test period.
- **The false-positive trade-off, quantified**: at about 1% of transactions flagged, each rule found 2–9% of the labelled transactions, with roughly 200–470 false positives per hit. A plain logistic regression found 21% with 39 false positives per hit.
- **Careful with claims**: the data and labels are simulated, so results describe this dataset, not real-world laundering. Reported numbers are recomputed by an independent script; 23 unit tests cover cleaning, leakage-free windows, metrics and thresholds.

---

### Featured project: Credit Risk Analytics

**[Banking Credit Risk Analytics & Default Prediction](https://github.com/Hariszss/banking-credit-risk-analytics)**
End-to-end credit risk project on 30,000 credit card customers: Python, SQL Server, Power BI (DAX) and scikit-learn.

- **Data warehouse**: validated raw data in Python, then loaded it into a SQL Server star schema (staging → core → analytics) with reconciliation checks and analytics views (window functions, roll rates).
- **Default prediction**: gradient boosting chosen over logistic regression and a rule-based segmentation using decision rules fixed in advance. Gini 0.56 vs 0.45 on a held-out test set, well calibrated (6,625 expected vs 6,636 actual defaults).
- **Fairness**: sex and marital status excluded after showing they add no predictive value, with outcomes checked by group anyway.
- **Power BI**: 4-page report (portfolio KPIs, segment risk, delinquency trends, early-warning watch list), stored as a Power BI Project (TMDL/PBIR) under version control.

---

### Featured project: Solar Financing Risk

**[Solar Revenue and Financing Risk in the Netherlands](https://github.com/Hariszss/solar-financing-risk)**
How solar production and electricity prices affect the revenue and debt coverage of a hypothetical Dutch solar park, using public energy and weather data.

- **Data validation first**: hourly production (PVGIS), weather (KNMI) and day-ahead prices aligned and checked for 2021–2024, including 26 daytime hours where a production model reports zero output that cannot be real.
- **Revenue**: the share of the average market price a solar park actually captures fell from 79% (2021) to 55% (2024); in 2024, 20% of output came in negative-price hours.
- **Financing risk**: first-year debt service coverage ratio ranged from 0.56 to 5.29 when selling at market prices, versus 0.99 to 1.19 under an illustrative fixed-price contract, with stress tests and break-even prices.

---

### Featured project: MSc Thesis

**[Staged ML Prediction of Postoperative Complications After Esophagectomy](https://github.com/Hariszss/esophagectomy-thesis)**
A staged machine learning pipeline (LASSO, Random Forest, XGBoost) predicting surgical complications from the Dutch nationwide DUCA registry (N=1,181 patients, Amsterdam UMC).

- **Staged design**: predictors added cumulatively across 4 clinical decision points, quantifying *when* in the patient pathway risk becomes predictable.
- **Leakage-safe evaluation**: 5-fold stratified CV with imputation fit per fold; hyperparameter sensitivity checked across a full grid.
- **Interpretability**: SHAP to sanity-check the drivers behind model output, including catching a confounded predictor before over-claiming a causal story.
- **Model vs. human judgment**: AUC 0.629 (model) vs. 0.536 (physiotherapist qualitative classification) on the same patients.

---

### Other projects

- **[Hospital Readmission Prediction](https://github.com/Hariszss/hospital-readmission)**: 30-day readmission risk in diabetic patients, gradient boosting + subgroup analysis
- **[Gender Bias in Multilingual mBERT](https://github.com/Hariszss/gender-bias-multilingual-mBERT)**: template-based probing and corpus analysis of bias across five languages

---

### Technical skills

**Languages:** Python, R, SQL
**Big data:** PySpark, Spark SQL (window functions, local-mode pipelines)
**ML:** scikit-learn, XGBoost, SHAP, PyTorch, HuggingFace
**Data & BI:** SQL Server (T-SQL, window functions, star schemas), Power BI (DAX, Power Query), pandas
**Methods:** Imbalanced-data evaluation (precision-recall, alert budgets, false positives per hit), probability-of-default modelling and calibration, staged prediction, model interpretability, cross-validation design, statistical testing
**Domains:** Financial crime detection, credit and financing risk, healthcare analytics & clinical registry data, NLP, stakeholder-facing reporting

---

### Background

- Data Analyst, Amsterdam UMC (Sep 2026–present); Data Science Intern (Apr–Aug 2026)
- MSc Applied Data Science, Utrecht University (2025–2026)
- BSc Mathematics (Statistics & Operational Research), University of Patras, Greece (2025)
- Erasmus+ exchange, University of Extremadura, Spain

---

### Reach me

[LinkedIn](https://www.linkedin.com/in/charalampos-zisis-8a3b40275/) · haris.zhshs@gmail.com
