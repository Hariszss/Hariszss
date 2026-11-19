# Charalampos Zisis

Data Analyst at Amsterdam UMC and MSc Applied Data Science graduate (Utrecht University, 2026). I prepare and validate complex datasets and build predictive models, most recently on clinical registry data, credit risk and transaction monitoring. Math background (Statistics & Operational Research, University of Patras) → data science, with a focus on risk analytics, financial crime detection and healthcare data.

I like problems where the model has to be trusted by people who aren't data scientists: clinicians, risk officers, auditors. That means interpretability and honest evaluation matter as much as raw accuracy.

---

### Featured project: Transaction Monitoring

**[Understanding False Positives in Transaction Monitoring](https://github.com/Hariszss/aml-transaction-monitoring)**
How simple monitoring rules trade alert volume against detection, using PySpark on IBM's synthetic AML data (about 5 million transactions).

- **PySpark pipeline with leakage-free features**: account-history windows that use only past transactions; rule thresholds set on fixed alert budgets and evaluated once on a held-out test period.
- **False positives quantified**: at about 1% of transactions flagged, the rules found 2–9% of labelled cases with 200–470 false positives per hit; a logistic regression found 21% with 39.

---

### Featured project: Credit Risk Analytics

**[Banking Credit Risk Analytics & Default Prediction](https://github.com/Hariszss/banking-credit-risk-analytics)**
End-to-end credit risk project on 30,000 credit card customers: Python, SQL Server, Power BI and scikit-learn.

- **SQL Server warehouse and Power BI report**: star schema with reconciliation checks, and a 4-page dashboard including an early-warning watch list.
- **Default prediction**: gradient boosting beat logistic regression and a rule-based segmentation (Gini 0.56 vs 0.45 on held-out data) and was well calibrated.

---

### Featured project: Solar Financing Risk

**[Solar Revenue and Financing Risk in the Netherlands](https://github.com/Hariszss/solar-financing-risk)**
How solar production and electricity prices affect the revenue and debt coverage of a hypothetical Dutch solar park, using public data.

- **Revenue**: the share of the market price a solar park actually captures fell from 79% (2021) to 55% (2024).
- **Financing risk**: first-year debt service coverage ranged from 0.56 to 5.29 at market prices, versus 0.99 to 1.19 under an illustrative fixed-price contract.

---

### Featured project: MSc Thesis

**[Staged ML Prediction of Postoperative Complications After Esophagectomy](https://github.com/Hariszss/esophagectomy-thesis)**
Predicting surgical complications from the Dutch DUCA registry (N=1,181 patients, Amsterdam UMC) with LASSO, Random Forest and XGBoost.

- **Staged design**: predictors added across 4 clinical decision points to show *when* in the patient pathway risk becomes predictable, with leakage-safe cross-validation and SHAP.
- **Model vs. human judgment**: AUC 0.629 for the model vs. 0.536 for physiotherapists' qualitative risk classification on the same patients.

---

### Other projects

- **[Hospital Readmission Prediction](https://github.com/Hariszss/hospital-readmission)**: 30-day readmission risk in diabetic patients, gradient boosting + subgroup analysis
- **[Gender Bias in Multilingual mBERT](https://github.com/Hariszss/gender-bias-multilingual-mBERT)**: template-based probing and corpus analysis of bias across five languages

---

### Technical skills

| | |
|---|---|
| **Languages** | Python, R, SQL |
| **Big data** | PySpark, Spark SQL |
| **Machine learning** | scikit-learn, XGBoost, SHAP, PyTorch, Hugging Face |
| **Data & BI** | pandas, SQL Server (T-SQL, star schemas), Power BI (DAX, Power Query) |
| **Methods** | Imbalanced-data evaluation, PD modelling and calibration, model interpretability, cross-validation design, statistical testing |
| **Domains** | Financial crime detection, credit and financing risk, healthcare and clinical registry data, NLP |

---

### Background

- Data Analyst, Amsterdam UMC (Sep 2026–present); Data Science Intern (Apr–Sep 2026)
- MSc Applied Data Science, Utrecht University (2025–2026)
- BSc Mathematics (Statistics & Operational Research), University of Patras, Greece (2025)
- Erasmus+ exchange, University of Extremadura, Spain

---

### Reach me

[LinkedIn](https://www.linkedin.com/in/charalampos-zisis-8a3b40275/) · haris.zhshs@gmail.com
