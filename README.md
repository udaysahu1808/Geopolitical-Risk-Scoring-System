# 🌍 Geopolitical Risk Scoring System

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-Database-4479A1?logo=mysql&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi&logoColor=black)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn%20%7C%20XGBoost-F7931E?logo=scikitlearn&logoColor=white)
![EDA](https://img.shields.io/badge/EDA-Exploratory%20Data%20Analysis-6A1B9A)
![Data Visualization](https://img.shields.io/badge/Data%20Visualization-Matplotlib-11557C)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0)
![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white)
![Classification](https://img.shields.io/badge/Task-Classification-success)
![Clustering](https://img.shields.io/badge/Task-Clustering-success)
![Anomaly Detection](https://img.shields.io/badge/Task-Anomaly%20Detection-success)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

A comprehensive end to end data analytics and machine learning project that transforms historical conflict data (WW1 & WW2) and simulated modern day escalation scenarios (WW3) into a quantified **Geopolitical Risk Index (0–100)** paired with SQL based analytics, predictive risk-tier classification, anomaly detection, conflict archetype clustering and an interactive Power BI dashboard.

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Objectives](#objectives)
- [Dataset](#dataset)
- [Project Structure](#project-structure)
- [Analysis Phases](#analysis-phases)
- [Key Insights](#key-insights)
- [Strategic Recommendations](#strategic-recommendations)
- [Tools & Technologies](#tools--technologies)
- [How to Run](#how-to-run)
- [Summary Table](#summary-table)
- [License](#license)
- [Author](#author)

---

## Project Introduction

Global geopolitical events armed conflicts, political instability, economic sanctions, terrorism, cyber warfare and diplomatic disputes create significant uncertainty for governments, multinational organizations, financial institutions and businesses. Although large volumes of geopolitical data are publicly available, converting this raw information into a meaningful, quantified risk assessment remains a major challenge.

This project follows a complete analytics pipeline: data collection and storage in **MySQL**, SQL-based business analytics, exploratory data analysis (EDA), feature engineering, a custom-built **Geopolitical Risk Index**, machine learning model development (classification, clustering, and anomaly detection) and an interactive **Power BI** dashboard.

By integrating Python, SQL, Machine Learning, and Business Intelligence into a unified workflow, the system enables analysts to identify geopolitical risk patterns, benchmark historical conflicts and predict the severity of emerging risk scenarios for informed strategic decision-making.

---

## 📖 Problem Statement

Large volumes of geopolitical and historical conflict data are publicly available, but the absence of an integrated analytical framework makes it difficult to efficiently store, analyze, visualize and predict geopolitical risk. A common challenge faced by analysts, governments and businesses is determining:

- Which factors (escalation, nuclear capability, cyber threat, economic impact, probability) contribute most to overall geopolitical risk.
- How historical conflict patterns (WW1, WW2) compare with modern escalation scenarios (WW3).
- Which regions and conflict issues carry the highest and most persistent risk.
- Whether unusual/anomalous scenarios exist that deviate from expected risk patterns.
- How to classify and predict the severity tier of a geopolitical scenario using machine learning.

Therefore, there is a need for a comprehensive, data-driven system that combines relational database management, statistical analysis, machine learning and business intelligence to generate accurate, actionable geopolitical risk insights.

---

## 🎯 Objectives of the Study

**Primary Objective:**
To develop an end-to-end Geopolitical Risk Scoring System by integrating MySQL, SQL Analytics, Exploratory Data Analysis (EDA), Machine Learning and Power BI for effective geopolitical risk assessment and decision support.

**Specific Objectives:**
- To collect, clean, and preprocess historical conflict and WW3 escalation scenario data for accurate analysis and modeling.
- To design and manage a relational database (MySQL) for efficient storage and retrieval of geopolitical data.
- To perform SQL-based analysis for extracting meaningful insights, trends and patterns from the dataset.
- To conduct Exploratory Data Analysis (EDA) using Python libraries to understand the distribution, relationships and characteristics of geopolitical events.
- To identify major factors influencing geopolitical risk: Region, Escalation Level, Nuclear Risk, Cyber Domain, Economic Impact and Conflict Probability.
- To engineer a composite **Geopolitical Risk Index (0–100)** from weighted risk components.
- To build and evaluate Machine Learning models (Logistic Regression, Random Forest, XGBoost) for predicting geopolitical risk tiers.
- To detect anomalous conflict scenarios using Isolation Forest.
- To segment conflicts into behavioral archetypes using K-Means clustering.
- To develop an interactive Power BI dashboard visualizing geopolitical trends, risk scores, and analytical insights.
- To provide data-driven recommendations supporting governments, businesses, researchers and policymakers in strategic decision-making.

---

## 📚 Scope of the Study

The scope of this project covers the complete lifecycle of a modern data analytics solution:

- **Data Cleaning & Preprocessing** — standardizing WW1/WW2 schemas, merging into a unified historical dataset, handling missing values in WW3 scenarios.
- **MySQL Database Design & Management** — storage of raw, cleaned, scored and ML-enriched tables.
- **SQL Queries & Business Analytics** — casualty analysis, theater/country rankings, escalation and nuclear-risk cross-tabs.
- **Exploratory Data Analysis (EDA)** — distributions, correlations, heatmaps, radar charts and year-wise trends.
- **Feature Engineering** — total casualties, casualty rate % and a five-component weighted risk score.
- **Machine Learning** — multi-class risk-tier classification, Isolation Forest anomaly detection, K-Means conflict archetype clustering.
- **Model Evaluation** — accuracy, confusion matrix, classification report, feature importance.
- **Interactive Power BI Dashboard Development** — executive summary, historical conflicts, regional ranking, WW3 scenarios and ML insights.

The study is limited to the available historical and simulated datasets and focuses on predictive analytics rather than real-time monitoring or live event forecasting.

---

## 📚 Significance of the Study

This project demonstrates how an integrated analytics pipeline can convert raw historical and scenario-based geopolitical data into valuable business intelligence and predictive insight. It is beneficial for:

- **Governments** — monitoring geopolitical stability and prioritizing diplomatic engagement.
- **Businesses & financial institutions** — evaluating operational, investment and market risk.
- **Researchers & analysts** — studying historical conflict patterns and modern escalation dynamics.
- **Students** — gaining practical, industry-standard experience with SQL, ML and BI tooling.
- **Organizations** — improving strategic, data-driven decision-making.

Additionally, the project serves as a portfolio piece demonstrating real-world application of Data Analytics, SQL, Machine Learning and Business Intelligence in a single workflow.

---

## 📊 Dataset

**Files:** `world_war_1_details.csv`, `world_war_2_details.csv`, `world_war_3_scenarios.csv`

### Historical Conflicts (WW1 & WW2 — merged into `historical_conflicts`)

| Column | Description |
|---|---|
| `conflict` | WW1 or WW2 |
| `start_year` / `end_year` | Conflict duration |
| `theater` | Theater of operations (e.g. Eastern Front, Pacific, Balkans) |
| `operation_or_battle` | Named battle or operation |
| `country` | Country involved |
| `alliance` | Allied Powers / Central Powers (WW1), Allies / Axis (WW2) |
| `role` | Air, Naval, Support, Belligerent, Expeditionary |
| `casualties_mil_k` | Military casualties (thousands) |
| `casualties_civ_k` | Civilian casualties (thousands) |
| `military_personnel_k` | Personnel deployed (thousands) |
| `front` | Front designation |
| `outcome` | Result of the battle/operation |
| `treaty` | Related treaty or conference |
| `key_leader` | Key military/political leader |
| `equipment_focus` | Primary equipment category |
| `notes` | Free-text notes |
| `total_casualties_k` *(engineered)* | Military + civilian casualties |
| `casualty_rate_pct` *(engineered)* | Military casualties as % of personnel deployed |

### WW3 Escalation Scenarios (`ww3_scenarios`)

| Column | Description |
|---|---|
| `issue_label` | Named geopolitical issue (e.g. Russia–Ukraine Conflict) |
| `year` | Scenario year |
| `region` | Geographic region |
| `primary_parties` / `allies` / `adversaries` | Parties involved |
| `trigger_event` | Precipitating event |
| `escalation_level` | Low / Moderate / High / Severe |
| `probability_estimate` | Estimated conflict probability (0–1) |
| `confidence` | Analyst confidence level |
| `humanitarian_impact` | Humanitarian consequence category |
| `economic_impact` | Economic consequence category |
| `cyber_domain` | Cyber threat severity |
| `nuclear_risk` | None / Low / Moderate / High |
| `narrative` / `data_origin` / `notes` | Supporting context |
| `probability_pct` *(engineered)* | Probability estimate as a percentage |

> **Dataset Size:** WW1 — 10,000 rows × 17 columns · WW2 — 10,000 rows × 17 columns · WW3 — 10,000 rows × 17 columns · **Total: 30,000 records** (Historical merged: 20,000 rows × 19 columns; WW3 cleaned: 10,000 rows × 18 columns)

---

## 📁 Project Structure

```
├── Dataset/
│   ├── world_war_1_details.csv
│   ├── world_war_2_details.csv
│   └── world_war_3_scenarios.csv
├── Notebook/
│   └── Geopolitical Risk Scoring System.ipynb
├── Power BI Dashboard/
│   ├── Dashboard Visuals/
│   │   ├── Executive Summary.png
│   │   ├── Historical Conflicts.png
│   │   ├── ML Insights.png
│   │   ├── Regional Risk Ranking.png
│   │   └── WW3 Risk Scenarios.png
│   └── Dashboard/
│       └── Geopolitical Risk Scoring System Dashboard.pbix
├── Visuals/
│   ├── Avg Conflict Probability - Nuclear Risk vs Cyber Domain.png
│   ├── Casualty Distribution WW1 vs WW2.png
│   ├── Distribution of Geopolitical Risk Index.png
│   ├── Risk Index Distribution by Nuclear Risk Level.png
│   ├── Scenario Count by Risk Tier.png
│   ├── Top 10 Most Anomalous Scenarios.png
│   ├── WW3 Risk Distribution.png
│   └── WW3 Scenarios per year & Average Risk Index.png
├── License
├── Requriments.txt
└── README.md
```

---

## 🔍 Analysis Phases

## Phase 1: Data Collection & Understanding

**Libraries used:** pandas, numpy, matplotlib, seaborn, mysql-connector-python, pymysql, sqlalchemy, scikit-learn (LabelEncoder, StandardScaler, MinMaxScaler, train_test_split, RandomForestClassifier, IsolationForest, LogisticRegression, KMeans, silhouette_score), xgboost.

**Database:** MySQL 8.0.45 — `geopolitical_risk_db` created and connected via SQLAlchemy.

**Datasets loaded:**

| Dataset | Rows | Columns |
|---|---|---|
| WW1 | 10,000 | 17 |
| WW2 | 10,000 | 17 |
| WW3 | 10,000 | 17 |
| **Total** | **30,000** | — |

---

## Phase 2: Missing Value Analysis

| Dataset | Missing Values |
|---|---|
| WW1 | None |
| WW2 | None |
| WW3 | `nuclear_risk` — 2,523 missing |

**Insight:** WW1 and WW2 datasets are fully complete. The only gap is in WW3's `nuclear_risk` field, resolved by assigning the category `"None"` ensuring no data loss while preserving analytical consistency.

---

## Phase 3: Data Cleaning, Feature Engineering & Push to MySQL

- WW1/WW2 columns standardized (`battle_name`/`operation_name` → `operation_or_battle`, `conflict_name` → `conflict`) and merged into a single `historical_conflicts` table.
- Engineered features: `total_casualties_k` (military + civilian), `casualty_rate_pct` (military casualties ÷ personnel deployed).
- WW3 `nuclear_risk` missing values filled with `"None"`; `probability_pct` engineered from `probability_estimate`.

| Table | Shape |
|---|---|
| `historical_conflicts` (WW1+WW2 merged) | 20,000 rows × 19 columns |
| `ww3_scenarios` (cleaned) | 10,000 rows × 18 columns |

Both tables pushed to MySQL and row-count validated (20,000 and 10,000 rows respectively).

---

## Phase 4: Core Business SQL Queries

**4.1 — Total Casualties by War & Alliance**

| Conflict | Alliance | Mil. Casualties (k) | Civ. Casualties (k) | Total (k) | Records |
|---|---|---|---|---|---|
| WW1 | Allied Powers | 3,120,595.82 | 2,112,214.81 | 5,232,810.63 | 6,970 |
| WW1 | Central Powers | 1,354,136.65 | 925,699.05 | 2,279,835.70 | 3,030 |
| WW2 | Allies | 5,305,058.77 | 4,220,670.86 | 9,525,729.63 | 7,010 |
| WW2 | Axis | 2,252,795.24 | 1,822,090.80 | 4,074,886.04 | 2,990 |

**4.2 — Top Deadliest Theaters (sample):** WW2 theaters (Asia, Eastern Front, Pacific, Atlantic, European, North Africa) dominate the top of the ranking with total casualties above 2.24M(k) each, ahead of the highest WW1 theaters (Air, Eastern Front, Naval, Balkans — ~925K–990K(k)).

**4.3 — Casualty Rate % by Role:** Casualty rates cluster tightly between ~28–30% across roles and conflicts, with Air roles in WW1 (30.25%) and Expeditionary roles in WW2 (30.21%) at the top.

**4.4 — Top Countries by Total Casualties:** United Kingdom (2.19M k total), Italy (2.14M k), France (2.15M k), United States (2.12M k) and Germany (2.07M k) lead the ranking.

**Insight:** WW2 alliances recorded substantially higher absolute casualties than WW1 due to greater scale of mobilization; casualty rates by role remain remarkably consistent across both wars, suggesting comparable combat-intensity ratios despite different technologies and eras.

---

## Phase 5: WW3 Scenario SQL Analysis

- **Risk distribution:** Combinations of Moderate/High escalation with High nuclear risk show the highest average conflict probabilities (~44–47%).
- **High-risk scenarios by region:** Latin America (Severe: 44.69% avg. probability, 485 scenarios), Middle East (High: 44.16%), Eastern Europe (High: 43.30%) rank among the most volatile.
- **Nuclear risk × cyber domain cross-tab:** Moderate nuclear risk paired with Moderate cyber domain yields the highest average probability (44.93%); combinations involving High cyber severity consistently rank in the upper range.
- **Economic impact frequency:** "Regional recession" paired with "Mass displacement" is the most frequent high-probability combination (662 scenarios, 44.93% avg. probability).

**Insight:** Escalation level and nuclear risk jointly serve as the strongest short-term predictors of conflict probability; regions such as Latin America, the Middle East and Eastern Europe consistently surface in high-escalation cross-tabs.

---

## Phase 6: SQL-Based Risk Scoring (Geopolitical Risk Index 0–100)

A weighted composite score built entirely in SQL from five components:

| Component | Range | Basis |
|---|---|---|
| Escalation score | 0–25 | Low → Severe |
| Nuclear score | 0–30 | None → High |
| Cyber score | 0–20 | Low → Severe |
| Probability score | 0–15 | `probability_estimate × 15` |
| Economic score | 0–10 | Localized shock → Global market impact |

The raw sum is min–max normalized to a **0–100 Risk Index** and tiered:

| Tier | Range |
|---|---|
| 🔴 Critical | ≥ 75 |
| 🟠 High | 50–74.9 |
| 🟡 Moderate | 25–49.9 |
| 🟢 Low | < 25 |

**Top-ranked scenarios include:** Russia–Ukraine Conflict (Latin America, 100.0), Venezuela–US Tensions 2026 (Latin America, 99.8), Russia–Ukraine Conflict (East Asia, 99.6), Korean Peninsula Risk (Middle East, 98.4), Taiwan Strait Stability (Middle East, 98.3) all classified 🔴 Critical.

The scored table (`risk_scored_scenarios`) was pushed back to MySQL for downstream analysis.

---

## Phase 7: Regional Risk Aggregation & Rankings

**6.1 — Regional Average Risk Index**

| Region | Avg. Risk Index | Max Risk Index | Scenarios | Critical Count |
|---|---|---|---|---|
| South Asia | 50.02 | 95.5 | 1,997 | 180 |
| Middle East | 49.86 | 98.4 | 1,931 | 178 |
| Eastern Europe | 49.79 | 95.5 | 2,065 | 189 |
| Latin America | 49.68 | 100.0 | 1,981 | 173 |
| East Asia | 49.52 | 99.6 | 2,026 | 187 |

**6.2 — Top Conflict Issues by Risk Index (Critical tier):** Israel–Arab Tensions (82.25), Venezuela–US Tensions 2026 (82.19), Taiwan Strait Stability (82.15), India–Pakistan Escalation 2025 (81.89), Russia–Ukraine Conflict (81.74), Korean Peninsula Risk (81.39).

**Insight:** Regional average risk is remarkably narrow (49.5–50.0) across all five regions, indicating a globally distributed risk landscape rather than concentration in a single hotspot though max risk and critical-scenario counts still differentiate regional volatility.

---

## Phase 8: Distribution, Correlation & Advanced EDA

- **Casualty distribution (WW1 vs WW2):** right-skewed in both wars; WW2 shows a heavier tail of high-casualty events.
- **WW3 probability distribution by escalation level:** Severe scenarios shift the probability density clearly rightward relative to Low/Moderate.
- **Risk Index by nuclear risk tier:** progressively higher density mass at elevated Risk Index values as nuclear risk increases from None → High.
- **Box plot (Risk Index by escalation level):** median Risk Index rises consistently from Low → Severe, with Severe showing the widest spread and most high-end outliers.
- **Correlation heatmaps:** `casualties_mil_k` correlates strongly with `total_casualties_k`; all five risk-score components (escalation, nuclear, cyber, probability, economic) correlate positively with the final `risk_index`, with escalation and nuclear risk showing the strongest relationships.
- **Scatter (personnel vs. casualties):** positive regression trend in both WW1 and WW2, confirming deployment scale as a key casualty driver.
- **Pair plot:** risk-tier classes (Low/Moderate/High/Critical) form visibly separable clusters across escalation, nuclear, and cyber scores.
- **Heatmaps (theater × alliance, region × escalation):** specific theater–alliance and region–escalation combinations consistently register the highest average risk/casualties.
- **Radar chart:** Severe-escalation scenarios score highest across all five risk dimensions simultaneously.
- **Year-wise trend:** scenario count and average Risk Index tracked together across years to detect emerging instability trends.

**Insight:** The Geopolitical Risk Index framework is internally consistent — every underlying component contributes positively and non-redundantly to the composite score and the classification structure (Low/Moderate/High/Critical) is visibly well-separated in feature space.

---

## Phase 9: EDA Summary Table

| Metric | Value |
|---|---|
| Total historical records | 20,000 |
| Total WW3 scenarios | 10,000 |
| Avg. military casualties WW1 (k) | 447.5 |
| Avg. military casualties WW2 (k) | 755.8 |
| Avg. WW3 probability estimate | ~43–45% |
| Highest risk region | South Asia |
| Most critical escalation level | Severe |
| Avg. Risk Index (all scenarios) | 49.8 |
| Critical risk scenarios | 9.1% |

**Insight:** WW2 recorded significantly higher average military casualties than WW1, reflecting its greater destructive scale. The overall Risk Index average of 49.8, with 9.1% of scenarios rated Critical, suggests a moderate-to-high global risk environment warranting continuous monitoring.

---

## Phase 10: Anomaly Detection (Isolation Forest)

- **Model:** `IsolationForest(contamination=0.05, random_state=42)` on standardized risk-score features.
- **Result:** 500 anomalous scenarios detected out of 10,000 (9,500 normal).
- **Top anomalies** recur around: Russia–Ukraine Conflict, Venezuela–US Tensions 2026, Korean Peninsula Risk, India–Pakistan Escalation 2025 and Taiwan Strait Stability — spanning both very low and very high Risk Index extremes.

**Insight:** Anomalies occur at both ends of the risk spectrum, showing that unusual geopolitical conditions aren't limited to high-risk cases, some low-escalation scenarios also deviate meaningfully from typical patterns, making them worth deeper investigation.

---

## Phase 11: Risk Tier Classifier (Multi-Class Classification)

Three models were trained on an 80/20 stratified split (8,000 train / 2,000 test) to predict risk tier (Low / Moderate / High / Critical):

| Model | Accuracy |
|---|---|
| Logistic Regression | 98.10% |
| Random Forest | 98.30% |
| **XGBoost (best)** | **99.20%** |

**Classification Report (XGBoost, test set):**

| Tier | Precision | Recall | F1-score | Support |
|---|---|---|---|---|
| Low | 1.00 | 0.98 | 0.99 | 198 |
| Moderate | 0.99 | 0.99 | 0.99 | 809 |
| High | 0.99 | 0.99 | 0.99 | 812 |
| Critical | 0.99 | 0.99 | 0.99 | 181 |
| **Accuracy** | | | **0.99** | 2,000 |

**Full-dataset prediction accuracy: 99.84%.**

**Insight:** Escalation level and nuclear risk emerged as the most influential features driving predictions. Misclassifications occur almost exclusively between adjacent tiers (e.g. High↔Critical), confirming the model reliably distinguishes major risk categories.

---

## Phase 12: K-Means Clustering — Conflict Archetypes

Optimal cluster count selected via elbow method + silhouette score → **K = 4**.

| Archetype | Count | Avg. Risk Index | Avg. Prob. % | Top Region | Top Escalation |
|---|---|---|---|---|---|
| Proxy War | 2,454 | 64.78 | 43.45 | East Asia | High |
| Nuclear Standoff | 2,464 | 52.80 | 42.69 | Eastern Europe | High |
| Cyber-Dominant | 2,607 | 45.33 | 64.04 | Latin America | Low |
| Direct Confrontation | 2,475 | 36.56 | 21.64 | Eastern Europe | Low |

**Insight:** Proxy War scenarios carry the highest average Risk Index (64.78) despite moderate probability, while Cyber-Dominant scenarios show the highest average conflict probability (64.04%), highlighting cyber threats as a high-likelihood but comparatively lower-severity risk category. Each archetype occupies a distinct region of the risk-probability space, supporting targeted, archetype-specific strategic planning.

---

## Phase 13: Power BI Export & Final Deliverables

Seven analysis-ready CSV exports generated for Power BI:

1. `01_master_risk_scored.csv` — master risk-scored dataset with all ML outputs
2. `02_historical_casualties_summary.csv` — historical casualties summary
3. `03_regional_risk_index.csv` — regional risk index rollup
4. `04_conflict_archetypes.csv` — conflict archetypes with cluster info
5. `05_anomalous_scenarios.csv` — anomalous scenarios
6. `06_equipment_analysis.csv` — equipment focus, WW1 vs WW2
7. `07_yearly_risk_trend.csv`— yearwise trend
   export

The final ML-enriched table (`final_risk_ml_output`) : containing risk scores, predicted tiers, anomaly flags, and archetypes was pushed back to MySQL: **10,000 rows** verified.

**Insight:** Organizing outputs into subject-specific datasets improves dashboard performance and simplifies Power BI data modeling, while the consolidated MySQL table supports scalable downstream querying.

---

## Phase 14: Business Insights

1. **Escalation Level is the Strongest Driver of Geopolitical Risk** — risk rises sharply as conflicts move from Low to Severe escalation.
2. **Nuclear Risk Significantly Amplifies Conflict Probability** — severe escalation combined with high nuclear capability produces the most critical scenarios.
3. **Certain Regions Consistently Exhibit Higher Risk Levels** — South Asia, the Middle East, and Eastern Europe lead in average and maximum risk.
4. **Historical Conflict Data Reveals Concentrated Casualty Patterns** — a small number of theaters (mainly WW2) account for the majority of casualties.
5. **Cyber Threats Increase Overall Geopolitical Instability** — higher cyber-domain severity tracks with higher composite risk.
6. **Economic and Humanitarian Impacts are Strongly Connected** — major economic disruption scenarios frequently coincide with severe humanitarian consequences.
7. **Machine Learning Successfully Identifies High-Risk Scenarios** — XGBoost achieves 99.2% test accuracy in classifying risk tiers.
8. **Conflict Archetypes Reveal Distinct Risk Profiles** — Proxy War, Nuclear Standoff, Cyber-Dominant, and Direct Confrontation each require different monitoring strategies.
9. **Anomaly Detection Surfaces Emerging Threats** — recurring anomalies (Russia–Ukraine, Venezuela–US, Korean Peninsula) merit continuous, dedicated tracking.
10. **Data-Driven Risk Scoring Enables Consistent Cross-Regional Comparison** — the 0–100 index allows apples-to-apples benchmarking across disparate conflict types.

---

## Phase 15: Strategic Recommendations

1. **Establish a Real-Time Geopolitical Risk Monitoring System** — integrate live data feeds for early conflict detection.
2. **Prioritize High-Risk Regions for Continuous Surveillance** — focus diplomatic, military, and economic attention on persistently high-scoring regions.
3. **Strengthen Nuclear Risk Assessment Frameworks** — regularly evaluate nuclear developments and arms trajectories.
4. **Integrate Cyber Threat Intelligence into Risk Assessment** — incorporate cyber posture into national and organizational security strategy.
5. **Enhance Economic Risk Preparedness** — build contingency plans for sanctions-, conflict-, or supply-chain-driven disruption.
6. **Leverage Machine Learning for Early Warning Systems** — deploy the trained classifier to flag high-risk scenarios before escalation.
7. **Improve Data Quality and Continuous Data Integration** — maintain accurate, up-to-date historical and scenario datasets.
8. **Support Data-Driven Policy Formulation** — use dashboards and predictive insight to guide foreign policy and defense planning.
9. **Promote International Collaboration** — encourage cross-border data and intelligence sharing to improve model coverage and accuracy.

---

## Phase 16: Executive Summary, Future Scope & Conclusion

### Executive Summary
This project presents an end-to-end Geopolitical Risk Scoring System that evaluates and predicts geopolitical instability using historical conflict data, modern escalation indicators, and machine learning. The framework integrates SQL, Python, ML, and Power BI to automate data processing, EDA, predictive modeling, anomaly detection, clustering, and interactive visualization. EDA revealed strong relationships between escalation, nuclear capability, conflict probability, and overall risk; the XGBoost classifier achieved 99.2% test accuracy in predicting risk tiers, while Isolation Forest and K-Means clustering surfaced anomalous scenarios and four distinct conflict archetypes. The resulting dashboard equips decision-makers with real-time visibility into regional instability, high-risk issues, and emerging threats.

### 💡 Future Scope
1. **Integrate real-time geopolitical news feeds and global intelligence APIs.**
2. **Incorporate satellite imagery and geospatial analytics** for enhanced regional monitoring.
3. **Develop deep learning models** for improved conflict prediction accuracy.
4. **Implement NLP** to analyze global news sentiment and diplomatic communications.
5. **Deploy cloud-based dashboards** for real-time monitoring and collaborative decision-making.
6. **Expand the framework** to include trade relations, sanctions, energy security, and migration patterns.
7. **Develop automated early warning systems** capable of generating proactive geopolitical alerts.
8. **Integrate reinforcement learning** to simulate conflict scenarios and policy outcomes.
9. **Enhance explainable AI (XAI)** capabilities (SHAP/LIME) for transparency in risk predictions.
10. **Build a fully automated enterprise-grade Geopolitical Intelligence Platform** for governments, corporations, and defense organizations.

### 📌 Conclusion
The Geopolitical Risk Scoring System successfully demonstrates how modern data analytics and machine learning can transform historical conflict data and simulated escalation scenarios into actionable geopolitical intelligence. Escalation level, nuclear risk, cyber threats, and conflict probability are confirmed as the strongest contributors to overall risk; predictive models classify risk levels with 99%+ accuracy, while anomaly detection and clustering reveal outlier scenarios and behavioral conflict archetypes. Overall, the project highlights the value of integrating Data Analytics, Machine Learning, and Business Intelligence for proactive geopolitical risk assessment, enabling governments, businesses, and policymakers to make informed strategic decisions in an increasingly uncertain global environment.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Python | Programming |
| Pandas / NumPy | Data analysis & numerical computing |
| Matplotlib / Seaborn | EDA visualization |
| MySQL / SQLAlchemy / PyMySQL | Relational database & SQL analytics |
| Scikit-learn | Machine learning (classification, clustering, anomaly detection, scaling) |
| XGBoost | Gradient-boosted risk-tier classification |
| Power BI | Interactive dashboard & business intelligence |
| Jupyter Notebook | Development environment |

---

## ▶️ How to Run

```bash
pip install mysql-connector-python pymysql sqlalchemy pandas numpy matplotlib seaborn xgboost scikit-learn openpyxl shap
jupyter notebook
```

1. Install MySQL and update `DB_HOST`, `DB_PORT`, `DB_USER`, `DB_PASSWORD` in the notebook to match your local setup.
2. Update the CSV file paths to point to your local `Dataset/` folder.
3. Run the notebook cells sequentially (Phases 1–16 as documented above).
4. Open the exported CSVs (or the `final_risk_ml_output` MySQL table) in Power BI to reproduce or refresh the dashboard.

---

## Summary Table

| Model | Accuracy |
|---|---|
| Logistic Regression | 98.10% |
| Random Forest | 98.30% |
| **XGBoost (best)** | **99.20%** |

| Metric | Value |
|---|---|
| Total records analyzed | 30,000 (20,000 historical + 10,000 WW3 scenarios) |
| Anomalies detected | 500 / 10,000 (5%) |
| Conflict archetypes identified | 4 (K-Means, K=4) |
| Avg. Risk Index (all scenarios) | 49.8 |
| Critical risk scenarios | 9.1% |
| Full-dataset classification accuracy | 99.84% |

---

## 📄 License

Copyright © 2026 Uday Sahu

All Rights Reserved.

This project and all associated files, including but not limited to source code, notebooks, reports, dashboards, visualizations, documentation, and datasets, are the exclusive intellectual property of Uday Sahu.

No part of this project may be copied, reproduced, modified, distributed, published, sublicensed, displayed, transmitted, or sold in any form or by any means without the prior written permission of the copyright holder.

Permission is granted only to view this project for personal, educational, or portfolio evaluation purposes. Commercial use, redistribution, and creation of derivative works are strictly prohibited.

Unauthorized use, reproduction, or distribution of this project may result in legal action under applicable copyright laws.

For permissions or licensing inquiries, please contact the copyright holder directly.

---

## 🙋 Author

**Uday Sahu**

**Data Analyst | Python | SQL | Power BI | Data Visualization | Business Analytics**

Passionate about transforming raw data into meaningful business insights through analytics, visualization, and automation.

---

⭐ **If you found this project helpful, consider giving it a Star!**
