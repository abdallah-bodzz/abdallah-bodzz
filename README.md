<div align="center">

# Abdallah A Khames

**Data Engineer · ML Engineer · CS @ Alexandria University (FCDS)**

[![Portfolio](https://img.shields.io/badge/Portfolio-abdallah--bodzz.github.io-1A5276?style=flat-square&logo=github&logoColor=white)](https://abdallah-bodzz.github.io/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abdallah-abdelhady-4187802b2)
[![Email](https://img.shields.io/badge/Email-Contact-c14438?style=flat-square&logo=gmail&logoColor=white)](mailto:xabdallahxabdallahx@gmail.com)
[![GitHub followers](https://img.shields.io/github/followers/abdallah-bodzz?label=Follow&style=flat-square)](https://github.com/abdallah-bodzz)
[![TikTok](https://img.shields.io/badge/TikTok-%23000000.svg?style=flat-square&logo=TikTok&logoColor=white)](https://tiktok.com/@data_w_bodzz)
[![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=flat-square&logo=YouTube&logoColor=white)](https://youtube.com/@abdallahabdelhady8713)

</div>

---

I build production-grade data systems and ML pipelines — end to end, from raw source through warehouse to BI layer. The work spans **enterprise data engineering** (medallion lakehouses, SCD2, star schemas), **predictive analytics** (XGBoost, survival analysis, NLP), **quantitative risk** (Monte Carlo VaR, event studies, cross-asset shock transmission), and **computer vision** (real-time fatigue detection). Every project is built for real business impact — not demo aesthetics.

---

## Featured Projects

### Enterprise Data Engineering & ERP Analytics

**[crm-customer-intelligence-module](https://github.com/abdallah-bodzz/crm-customer-intelligence-module)** — *Enterprise CRM Intelligence & Customer 360 Platform*

Production-grade Enterprise CRM platform built on a Medallion Lakehouse (Bronze → Silver → Gold) on SQL Server. Implements **Customer Master Data Management (MDM)** via SCD Type 2, five predictive ML models (XGBoost Churn & CLV, Weibull AFT next-purchase timing, K-means RFM segmentation, LeIA PT-BR sentiment), and an operational **CRM Action Engine** that translates ML predictions into prioritised retention and reactivation tasks — modelled after SAP CRM and Odoo CRM architecture. 96,096 unified customers · R$15.84M GMV · 7-page Power BI report · 29 DAX measures · [Live dashboard →](https://app.powerbi.com/view?r=eyJrIjoiMTBkZDE3YTMtNzZhZS00OWJlLWEyZTItM2U4NjQ4NjI4MzJiIiwidCI6ImVhZjYyNGM4LWEwYzQtNDE5NS04N2QyLTQ0M2U1ZDc1MTZjZCIsImMiOjh9)

`SQL Server` `Python` `XGBoost` `lifelines` `Power BI` `SCD2` `MDM`

---

**[enterprise-retail-analytics-platform](https://github.com/abdallah-bodzz/enterprise-retail-analytics-platform)** — *ERP Analytics Platform*

Institutional-grade ERP analytics platform framed as a real consulting engagement on AdventureWorks 2022. Three-layer medallion lakehouse (7 staging → 8 warehouse → 10 mart tables), SCD Type 2 on products and customers, ABC product classification, RFM + K-means customer segmentation, and 6 Power BI dashboards mapped to executive personas (CEO, Sales Director, Ops, Procurement, Warehouse). 504 SKUs classified · 19,800 customers segmented · sub-second dashboard performance via pre-calculated mart metrics.

`SQL Server` `Python` `Power BI` `ABC Analysis` `K-means` `SCD2`

---

### Machine Learning

**[fraud-detection-api](https://github.com/abdallah-bodzz/fraud-detection-api)** — *Production Credit Card Fraud Detection API*

Production-ready fraud detection API with threshold tuned for dollars protected, not just F1. AUPRC 0.87 on 0.17% fraud rate. **$10,576 protected per run** at threshold 0.4. FastAPI, Docker, rate limiting, structured logging.

`Python` `XGBoost` `FastAPI` `Docker`

---

**[credit-risk-scoring](https://github.com/abdallah-bodzz/credit-risk-scoring)** — *Loan Default Prediction*

End-to-end loan default prediction with EDA, feature engineering, model comparison (LR, RF, XGBoost, LightGBM), probability calibration, and business-optimised threshold. **$3.55M net benefit · 152% ROI per 10k loans.**

`Python` `XGBoost` `LightGBM` `scikit-learn`

---

**[heart-disease-prediction](https://github.com/abdallah-bodzz/heart-disease-prediction)** — *Clinical Screening Classifier*

Binary classifier on UCI Cleveland dataset. Threshold-optimised screening (t=0.40): Recall 0.964, F1 0.900. **164 fewer missed diagnoses → ~$8.1M savings per 10k patients.**

`Python` `scikit-learn`

---

**[driveguard](https://github.com/abdallah-bodzz/driveguard)** — *Real-Time Driver Fatigue Detection*

Real-time fatigue detection via standard webcam. EAR/MAR geometry + CNN hybrid trained on 84k-image MRL dataset. **98.8% accuracy, 3–5ms CPU inference.** Dual-timescale fatigue scoring, head pose via solvePnP, gesture-based alarm dismissal. 25–30 FPS, fully local.

`Python` `OpenCV` `MediaPipe` `TensorFlow`

---

**[sentiment-analysis](https://github.com/abdallah-bodzz/sentiment-analysis)** — *Customer Review Classification Pipeline*

Production-ready NLP pipeline for customer review sentiment classification. TextBlob + custom neutral-word lexicon hybrid. Automated preprocessing (tokenisation, stopword removal, lemmatisation), confusion matrix, structured JSON metric export. **86.7% accuracy · Precision 1.00 on positive class.**

`Python` `NLTK` `TextBlob` `scikit-learn`

---

### Quantitative Risk & Event Studies

**[2026-hormuz-blockade-analysis](https://github.com/abdallah-bodzz/2026-hormuz-blockade-analysis)** — *Cross-Asset Shock Transmission Study · v2*

Hormuz 2026: When Diplomacy Decoupled From Supply — Quantitative event study of the Strait of Hormuz crisis (113 trading days). Update 2 reveals the May Paradox: WTI fell −20% while transit capacity stayed near 2%. Cross-asset shock transmission across 16 assets, 5 event windows. Live interactive dashboard. **[Live Dashboard →](https://abdallah-bodzz.github.io/2026-hormuz-blockade-analysis/)**

`Python` `SciPy` `yfinance` `Plotly`

---

**[monte-carlo-risk-simulator](https://github.com/abdallah-bodzz/monte-carlo-risk-simulator)** — *Correlated Portfolio VaR & Expected Shortfall*

Correlated portfolio Monte Carlo for VaR and Expected Shortfall. Cholesky decomposition, fat tails (Student-t, ν=5), live market data. FastAPI + interactive Chart.js dashboard.

`Python` `NumPy` `SciPy` `FastAPI`

---

### Valuation & Financial Engineering

**[dcf-valuation-engine](https://github.com/abdallah-bodzz/dcf-valuation-engine)** — *DCF with Live Market Data*

DCF tool with live yfinance data, WACC discounting, Gordon Growth terminal value, and a 7×7 sensitivity heatmap. Dark-theme UI.

`Python` `FastAPI` `yfinance`

---

**[financial-Excel-model-generator](https://github.com/abdallah-bodzz/financial-Excel-model-generator)** — *3-Statement Model Generator*

Python generates a complete 3-statement financial model (P&L, Balance Sheet, Cash Flow, DCF, scenario engine, sensitivity matrix) as a native Excel file. All formulas live in Excel — Python only builds the structure. Base/Best/Worst scenarios via INDEX/MATCH dropdown.

`Python` `openpyxl`

---

### Tools & Utilities

**[nb2md](https://github.com/abdallah-bodzz/nb2md)** — *Notebook → AI-Friendly Markdown*

Convert Jupyter notebooks to clean Markdown for LLM context windows. Zero dependencies, pure stdlib. 741 KB `.ipynb` → 71 KB `.md` (90% smaller). Strips base64 images, HTML widgets, cell metadata — keeps code, prose, and text outputs. Available on PyPI.

```
pip install nb2md
```

`Python` `PyPI` `Zero dependencies`

---

**[data-explorer-pro](https://github.com/abdallah-bodzz/data-explorer-pro)** — *Professional Data Analysis Workbench*

Modern, modular data analysis platform built on Streamlit and Plotly. Exploration, data preparation, 20+ chart types, AI Copilot (Gemini, Claude, or local EchoEngine), relationship modelling, and HTML report export. Layered architecture (Core → Services → UI). 34 previous iterations before the current clean architecture.

`Python` `Streamlit` `Plotly` `FastAPI`

---

### Power BI Dashboards

| Project | What it covers |
|---------|----------------|
| [powerbi-wake-county-budget-report](https://github.com/abdallah-bodzz/powerbi-wake-county-budget-report) | Government expenditure analysis — Wake County, NC (FY2017–2019). Star schema from raw CSVs, YTD spend, budget utilisation, drill-through to cost-center level. |
| [mortgage-trading-analysis-powerbi](https://github.com/abdallah-bodzz/mortgage-trading-analysis-powerbi) | Mortgage trading desk simulation — loan pipeline review, counterparty bid evaluation, FICO-based pricing. |
| [financial-analysis-powerbi-dashboard](https://github.com/abdallah-bodzz/financial-analysis-powerbi-dashboard) | 12-page dark dashboard — revenue/profit decomposition, customer segmentation, NPV/IRR, DCF, payback. |
| [supply-chain-analytics-powerbi](https://github.com/abdallah-bodzz/supply-chain-analytics-powerbi) | Make-vs-buy decision tool — supplier quote analysis, volume scenario planning, manufacturing cost comparison. |
| [customer-churn-analysis-powerbi](https://github.com/abdallah-bodzz/customer-churn-analysis-powerbi) | Telecom churn analysis — 6,687 customers, 26.86% churn, breakdown by reason / geography / contract / data plan. |
| [hr-analytics-powerbi](https://github.com/abdallah-bodzz/hr-analytics-powerbi) | Employee attrition — Atlas Labs dataset, automated variance logic surfaced 3 high-attrition clusters on first load. |
| [time-series-analysis-powerbi-dashboard](https://github.com/abdallah-bodzz/time-series-analysis-powerbi-dashboard) | Retail PoS + MSFT financials — rolling windows, YTD/YoY DAX, forecasting visuals. |

---

### Excel Financial Models

| Project | What it covers |
|---------|----------------|
| [financial-modeling-excel](https://github.com/abdallah-bodzz/financial-modeling-excel) | Income statements, cap rates, forecasts, and dynamic models for real estate. |
| [net-revenue-management-excel](https://github.com/abdallah-bodzz/net-revenue-management-excel) | Full NRM business case for an FMCG supplier — market share, portfolio profitability, promotional ROI. |
| [customer-churn-analysis-excel](https://github.com/abdallah-bodzz/customer-churn-analysis-excel) | Churn analysis on 6,687 telecom customers via PivotTables. |

---

## Tech Stack

| Domain | Technologies |
|--------|-------------|
| **Languages** | Python · R · SQL (T-SQL) |
| **Data Engineering** | SQL Server · Medallion Lakehouse · SCD Type 2 · Star Schema · SQLAlchemy · pyodbc |
| **ML & Analytics** | XGBoost · LightGBM · scikit-learn · lifelines (Weibull AFT) · pandas · NumPy · MLflow |
| **NLP** | LeIA (PT-BR VADER) · TextBlob · NLTK · VADER |
| **Computer Vision** | OpenCV · MediaPipe · TensorFlow · CNN |
| **Quantitative Finance** | SciPy (VaR, ES, Cholesky) · Monte Carlo · OLS event study · yfinance |
| **Visualisation & BI** | Power BI (DAX, drill-through, bookmarks, What-If) · Plotly · Matplotlib · Chart.js |
| **Backend & APIs** | FastAPI · Pydantic · Uvicorn · Docker |
| **Databases** | SQL Server · PostgreSQL · MySQL |
| **Tools** | Jupyter · Streamlit · Excel (DCF, 3-statement, NRM) · Git · python-dotenv · rich |

---

## Content — @data_w_bodzz

I document Power BI builds, SQL deep dives, and project breakdowns on TikTok and YouTube.

**200,000+ total views · 1,500+ followers**  
Best video: Power BI normalization & lookup tables — **16k+ views**

---

## Connect

[![Portfolio](https://img.shields.io/badge/Portfolio-abdallah--bodzz.github.io-1A5276?style=flat-square&logo=github)](https://abdallah-bodzz.github.io/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abdallah-abdelhady-4187802b2)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:xabdallahxabdallahx@gmail.com)
[![TikTok](https://img.shields.io/badge/TikTok-%23000000.svg?style=flat-square&logo=TikTok&logoColor=white)](https://tiktok.com/@data_w_bodzz)
[![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=flat-square&logo=YouTube&logoColor=white)](https://youtube.com/@abdallahabdelhady8713)
[![X](https://img.shields.io/badge/X-black.svg?style=flat-square&logo=X&logoColor=white)](https://x.com/hottestboda)
[![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?style=flat-square&logo=Instagram&logoColor=white)](https://instagram.com/abdallah_abdelhadi)
