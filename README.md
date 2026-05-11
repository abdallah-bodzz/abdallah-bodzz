# Abdallah Abdelhady
**Data Analyst · ML Engineer · CS @ Alexandria University (FCDS)**

[![Portfolio](https://img.shields.io/badge/Portfolio-abdallah--bodzz.github.io-1A5276?style=flat-square&logo=github&logoColor=white)](https://abdallah-bodzz.github.io/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abdallah-abdelhady-4187802b2)
[![Email](https://img.shields.io/badge/Email-Contact-c14438?style=flat-square&logo=gmail&logoColor=white)](mailto:xabdallahxabdallahx@gmail.com)
[![GitHub followers](https://img.shields.io/github/followers/abdallah-bodzz?label=Follow&style=flat-square)](https://github.com/abdallah-bodzz)

I build data-driven tools at the intersection of **machine learning, quantitative risk, and finance** — credit risk pipelines, Monte Carlo VaR simulations, DCF valuation engines, computer vision systems, and geopolitical event studies. Every project is driven by **real business impact**: ROI, cost savings, risk reduction, or a finding that changes how you read the market.

---

## 🛠️ Tech Stack

| Category | Technologies |
|----------|--------------| 
| **Languages** | Python · R · SQL |
| **ML & Data Science** | scikit-learn · XGBoost · LightGBM · pandas · NumPy · MLflow · category_encoders · joblib |
| **Computer Vision** | OpenCV · MediaPipe · TensorFlow · CNN (EAR/MAR geometry · solvePnP) |
| **Quantitative Finance** | SciPy (VaR, ES, Cholesky) · Monte Carlo simulation · OLS event study · Student‑t · yfinance |
| **Visualization & BI** | Power BI (DAX, drill-through, bookmarks, Key Influencers, forecasting) · Plotly · Matplotlib · Chart.js |
| **Backend & APIs** | FastAPI · Pydantic · Uvicorn · Docker |
| **Databases** | PostgreSQL · MySQL · MS SQL Server |
| **Tools** | Excel (PivotTables, DCF, NRM, 3‑statement modeling) · Jupyter · Git · YAML · openpyxl |

---

## 🚀 Projects

### 🤖 Machine Learning

| Project | Description | Stack |
|---------|-------------|-------|
| [**fraud-detection-api**](https://github.com/abdallah-bodzz/fraud-detection-api) | Production-ready credit card fraud detection API. Threshold tuned for dollars saved — not F1. **AUPRC 0.87** on 0.17% fraud rate. **$10,576 protected per run** at threshold 0.4. FastAPI, Docker, rate limiting, structured logging. | Python · XGBoost · FastAPI · Docker |
| [**credit-risk-scoring**](https://github.com/abdallah-bodzz/credit-risk-scoring) | End-to-end loan default prediction: EDA, feature engineering, model comparison (LR, RF, XGBoost, LightGBM), probability calibration, business-optimised threshold. **$3.55M net benefit / 152% ROI per 10k loans.** | Python · XGBoost · LightGBM · scikit-learn |
| [**heart-disease-prediction**](https://github.com/abdallah-bodzz/heart-disease-prediction) | Binary classifier on UCI Cleveland dataset. Threshold-optimised screening (t=0.40): recall **0.964**, F1 **0.900**. **164 fewer missed diagnoses → ~$8.1M savings per 10k patients.** | Python · scikit-learn · pandas |
| [**driveguard**](https://github.com/abdallah-bodzz/driveguard) | Real-time driver fatigue detection via standard webcam. EAR/MAR geometry + CNN hybrid (84k-image MRL dataset, **98.8% accuracy**, 3–5ms CPU inference). Dual-timescale fatigue scoring, head pose via solvePnP, gesture-based alarm dismissal. 25–30 FPS, fully local. | Python · OpenCV · MediaPipe · TensorFlow |

### 📉 Quantitative Risk & Event Studies

| Project | Description | Stack |
|---------|-------------|-------|
| [**2026-hormuz-blockade-analysis**](https://github.com/abdallah-bodzz/2026-hormuz-blockade-analysis) | Quantitative event study of the 47-day Strait of Hormuz blockade (Feb–Apr 2026). Key finding: **WTI +32.9% during closure while XOM fell −1.5%** — energy equities are not oil proxies in supply shocks. Beta flipped from +0.15 to −0.42. Gold dropped −9.6% (safe-haven failure under margin pressure). OLS abnormal returns, Cholesky correlation, DXY decomposition, counterfactual baseline across 10 assets. | Python · SciPy · yfinance · Plotly |
| [**monte-carlo-risk-simulator**](https://github.com/abdallah-bodzz/monte-carlo-risk-simulator) | Correlated portfolio Monte Carlo for VaR & Expected Shortfall. Cholesky decomposition, fat tails (Student‑t, ν=5), live market data. FastAPI + interactive Chart.js dashboard. Answers: *"How bad can this portfolio actually get?"* | Python · NumPy · SciPy · FastAPI |

### 💰 Valuation & Financial Engineering

| Project | Description | Stack |
|---------|-------------|-------|
| [**dcf-valuation-engine**](https://github.com/abdallah-bodzz/dcf-valuation-engine) | DCF tool with live yfinance data, WACC discounting, Gordon Growth terminal value, and a 7×7 sensitivity heatmap. Dark-theme UI. | Python · FastAPI · yfinance · Chart.js |
| [**financial-Excel-model-generator**](https://github.com/abdallah-bodzz/financial-Excel-model-generator) | Python generates a complete 3-statement financial model (P&L, Balance Sheet, Cash Flow, DCF, scenario engine, sensitivity matrix) as a native Excel file. All formulas live in Excel — Python only builds the structure. Base/Best/Worst scenarios via INDEX/MATCH dropdown. | Python · openpyxl |

### 📈 Power BI Dashboards

| Project | Description |
|---------|-------------|
| [**powerbi-wake-county-budget-report**](https://github.com/abdallah-bodzz/powerbi-wake-county-budget-report) | Government expenditure analysis on Wake County, NC open data (FY2017–2019). Star-schema model from raw CSVs; DAX measures for YTD spend, budget utilization, variance flags; drill-through to cost-center level. Replicates a real public-sector BI workflow end-to-end. |
| [**mortgage-trading-analysis-powerbi**](https://github.com/abdallah-bodzz/mortgage-trading-analysis-powerbi) | Mortgage trading desk simulation: loan pipeline review, counterparty bid evaluation, benchmark testing, FICO‑based pricing recommendations. DataCamp capstone. |
| [**financial-analysis-powerbi-dashboard**](https://github.com/abdallah-bodzz/financial-analysis-powerbi-dashboard) | 12-page dark dashboard: revenue/profit decomposition, customer segmentation, scenario modeling, capital budgeting (NPV/IRR, DCF, payback). |
| [**supply-chain-analytics-powerbi**](https://github.com/abdallah-bodzz/supply-chain-analytics-powerbi) | Make‑vs‑buy decision tool with supplier quote analysis, dynamic volume scenario planning, internal manufacturing cost comparison. |
| [**customer-churn-analysis-powerbi**](https://github.com/abdallah-bodzz/customer-churn-analysis-powerbi) | Telecom churn analysis (Databel, 6,687 customers, 26.86% churn): breakdown by reason, geography, age, contract type, data plan, international plan mismatch. |
| [**hr-analytics-powerbi**](https://github.com/abdallah-bodzz/hr-analytics-powerbi) | Employee attrition analysis (Atlas Labs): demographics, attrition by department/role/tenure/travel, individual performance tracking. Automated variance logic surfaced 3 high-attrition clusters on first load. |
| [**time-series-analysis-powerbi-dashboard**](https://github.com/abdallah-bodzz/time-series-analysis-powerbi-dashboard) | Retail PoS (Superstore) + MSFT financial data: rolling windows, YTD/YoY DAX measures, and forecasting visuals. |

### 📊 Excel Financial Models

| Project | Description |
|---------|-------------|
| [**financial-modeling-excel**](https://github.com/abdallah-bodzz/financial-modeling-excel) | Income statements, cap rates, forecasts, and dynamic models for real estate investments. |
| [**net-revenue-management-excel**](https://github.com/abdallah-bodzz/net-revenue-management-excel) | Full NRM business case for an FMCG supplier (HealthMax): market share, portfolio profitability, subcategory opportunity sizing, promotional ROI. |
| [**customer-churn-analysis-excel**](https://github.com/abdallah-bodzz/customer-churn-analysis-excel) | Churn analysis on 6,687 telecom customers (Databel). PivotTables, calculated columns, complete dashboard. |

---

## 📌 What You'll Find Here

- **Business-first ML** — models optimised for real cost structures (false negatives costlier than false positives)
- **Production-ready APIs** — fraud detection with Docker, rate limiting, structured logging
- **Quantitative risk & event studies** — proper correlation (Cholesky), fat tails, VaR/ES, OLS abnormal returns
- **Computer vision** — real-time fatigue detection with CNN hybrid, gesture control, session recording
- **Valuation tools** — DCF with sensitivity, real data integration, 3-statement Excel generators
- **Geopolitical data analysis** — cross-asset shock transmission, counterfactual baselines, regime detection
- **Interactive dashboards** — Power BI & Excel for government, finance, ops, HR, and supply chain
- **Clean, modular code** — `src/` packages, YAML configs, reproducible notebooks

---

## 📱 Content — @data_w_bodzz

I document Power BI builds, SQL deep dives, and project breakdowns on **TikTok & YouTube**.

→ **200,000+ total views · 1,500+ followers**  
→ Best video: Power BI normalization & lookup tables — **16k+ views**  
→ Content: real-time build series, mortgage trading insights, honest project breakdowns

---

## 🌐 Connect

[![Portfolio](https://img.shields.io/badge/Portfolio-abdallah--bodzz.github.io-1A5276?style=flat-square&logo=github)](https://abdallah-bodzz.github.io/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abdallah-abdelhady-4187802b2)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:xabdallahxabdallahx@gmail.com)
[![TikTok](https://img.shields.io/badge/TikTok-%23000000.svg?style=flat-square&logo=TikTok&logoColor=white)](https://tiktok.com/@data_w_bodzz)
[![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=flat-square&logo=YouTube&logoColor=white)](https://youtube.com/@abdallahabdelhady8713)
[![X](https://img.shields.io/badge/X-black.svg?style=flat-square&logo=X&logoColor=white)](https://x.com/hottestboda)
[![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?style=flat-square&logo=Instagram&logoColor=white)](https://instagram.com/abdallah_abdelhadi)
