# Amazon-Prime-TV-Shows-and-Movies-Exploratory-Data-Analysis
An end-to-end Python EDA on 9.8k+ Amazon Prime titles analyzing catalog structure, genre trends, global production hubs, and IMDb/TMDB rating metrics to optimize content acquisition and reduce subscriber churn.
# 🎬 Amazon Prime Video Catalog Analysis & EDA

A comprehensive Exploratory Data Analysis (EDA) of Amazon Prime Video's US catalog analyzing **9,800+ titles** and **124,000+ credit records** using Python.

---

## 📌 Business Objective
Analyze catalog structure, regional footprints, genre hierarchies, and audience rating dynamics to guide content acquisition strategies and reduce subscriber churn.

---

## 🛠️ Tech Stack
* **Language:** Python
* **Environment:** Google Colab / Jupyter Notebook
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
* **Utilities:** `ast.literal_eval` (List parsing)

---

## 🧹 Data Hygiene & Wrangling
* **Cleaned Strings:** Parsed array-like strings in `genres` and `production_countries` into native Python lists.
* **Exploded Data:** Created unnested long-format DataFrames for precise, non-redundant genre and country counts.
* **Handling Nulls & Duplicates:** Imputed missing age ratings as `'Unrated'`, removed duplicate rows, and merged `titles.csv` with `credits.csv`.
* **UBM Framework:** Structured visual analysis following Univariate $\rightarrow$ Bivariate $\rightarrow$ Multivariate steps.

---

## 📊 Key Findings

| Finding | Insight | Business Impact |
| :--- | :--- | :--- |
| **Catalog Asymmetry** | Movies make up **86.2%** of titles, but TV Shows score higher (mean IMDb **7.12** vs **5.80** for Movies). | Shift acquisition budgets toward multi-season TV series for higher viewer retention. |
| **Global Hubs** | US leads production volume; **India** is the top international hub with over 1,000 titles. | Double down on local original productions in rapid-growth markets like India. |
| **Genre ROI** | Drama and Comedy dominate volume; **Documentaries** achieve highest quality ratings (~7.2 IMDb). | Leverage documentaries for high cost-to-rating efficiency and prestige branding. |
| **Runtime Fatigue** | Slight negative correlation ($r = -0.10$) between runtime and IMDb ratings. | Keep feature runtimes optimized to prevent viewer drop-offs. |
| **Series Churn Risk** | Strong negative correlation ($r = -0.41$) between release year and season count (>60% single-season shows). | Avoid premature show cancellations to maintain viewer trust and prevent churn. |

---
