# Enological Market Intelligence: Chemical-Sensory Positioning & Margin Optimization

[![Language](https://img.shields.io/badge/Language-R%20Markdown%20%7C%20Supabase-276DC3?style=flat&logo=r)](https://www.r-project.org/)
[![Domain](https://img.shields.io/badge/Domain-Enological%20BI%20%26%20Pricing-purple)](#)
[![Report](https://img.shields.io/badge/Report-Executive%20BI%20Summary-red?logo=adobeacrobatreader)](businessgame_full.pdf)

> End-to-end Business Intelligence pipeline: transforming 11 enological chemical parameters and 2,000 unstructured customer reviews into strategic pricing and product segmentation.

---

## 📌 Executive Summary

Wineries frequently set pricing and market positioning based on historical dogma or subjective tasting panels. They fail to identify the direct empirical bridge connecting enological chemistry to actual consumer willingness-to-pay.

Engineered as a commercial business intelligence prototype, this project delivers an end-to-end analytical pipeline:
- Ingests a catalog of **20 wines with 11 chemical indicators** alongside **2,000 consumer reviews** with demographic profiles.
- Executes four sequential analytical phases: **Preprocessing → Chemical EDA → NLP & Clustering → Executive Export**.
- Delivers clean, enriched datasets ready for real-time visualization in Power BI and Tableau to maximize product margins.

Full technical details and strategic recommendations are compiled in [`businessgame_full.pdf`](businessgame_full.pdf) and [`report_executive_summary.md`](report_executive_summary.md).

---

## 🔍 Four-Phase BI Pipeline

### 1. Robust Preprocessing & Outlier Hygiene
- **1st–99th Percentile Winsorization:** Mitigates extreme recording anomalies across volatile chemical indicators (`residual.sugar`, `chlorides`, `sulphates`) while preserving genuine biological terroir variation.
- **Median Imputation Safeguards:** Embeds procedural safeguards ensuring future unreleased catalog additions with missing metrics do not break upstream ETL pipelines.

### 2. Enological Chemistry EDA
- Identifies critical covariance structures: strong collinearity between free and total sulfur dioxide ($r = 0.58$), and inverse density-alcohol correlations ($r = -0.68$).
- Establishes quality baselines: isolating how volatile acidity thresholds directly depress consumer rating ceilings.

### 3. Customer Sentiment NLP & Unsupervised Clustering
- **K-Means & Hierarchical Clustering:** Segments the product portfolio into distinct sensory clusters (e.g., High-Alcohol Bold Reds vs Acidic Crisp Whites).
- **Sentiment & Demographic Cross-Referencing:** Maps customer age and spending preferences against specific flavor profiles, identifying premiumization opportunities.

### 4. Enterprise Reporting & BI Export
- Unified relational schemas exported directly to CSV and Supabase cloud tables.
- Pre-configured data models for Power BI (`.pbix`) and Tableau (`.twb`) dashboards with KPI drill-downs for winery leadership.

---

**Authors:** Francesco Colombini & Mattia Lombardo  
[GitHub Profile](https://github.com/FRA-0023) · [LinkedIn](https://www.linkedin.com/in/francescocolombini/)