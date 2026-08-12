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

I build data systems and ML pipelines end to end: raw source, warehouse, BI layer. That covers enterprise data engineering (medallion lakehouses, SCD2, star schemas), predictive analytics (XGBoost, survival analysis, NLP), quantitative risk (Monte Carlo VaR, event studies, cross-asset shock transmission), and computer vision (real-time fatigue detection). I'd rather ship something that runs than polish a notebook nobody deploys.

---

## Featured Projects

### Enterprise Data Engineering & ERP Analytics

**[crm-customer-intelligence-module](https://github.com/abdallah-bodzz/crm-customer-intelligence-module)** — *Enterprise CRM Intelligence & Customer 360 Platform*

A CRM platform on a Medallion Lakehouse (Bronze → Silver → Gold), SQL Server. Customer Master Data Management via SCD Type 2, five predictive ML models (XGBoost churn and CLV, Weibull AFT next-purchase timing, K-means RFM segmentation, LeIA PT-BR sentiment), and a CRM Action Engine that turns predictions into prioritised retention tasks, built along the lines of SAP CRM and Odoo CRM. 96,096 unified customers, R$15.84M GMV, 7-page Power BI report, 29 DAX measures. [Live dashboard →](https://app.powerbi.com/view?r=eyJrIjoiMTBkZDE3YTMtNzZhZS00OWJlLWEyZTItM2U4NjQ4NjI4MzJiIiwidCI6ImVhZjYyNGM4LWEwYzQtNDE5NS04N2QyLTQ0M2U1ZDc1MTZjZCIsImMiOjh9)

`SQL Server` `Python` `XGBoost` `lifelines` `Power BI` `SCD2` `MDM`

---

**[enterprise-retail-analytics-platform](https://github.com/abdallah-bodzz/enterprise-retail-analytics-platform)** — *ERP Analytics Platform*

Built as if it were a real consulting engagement on AdventureWorks 2022. Three-layer medallion lakehouse (7 staging, 8 warehouse, 10 mart tables), SCD Type 2 on products and customers, ABC product classification, RFM plus K-means segmentation, and 6 Power BI dashboards mapped to executive personas (CEO, Sales Director, Ops, Procurement, Warehouse). 504 SKUs classified, 19,800 customers segmented, sub-second dashboards from pre-calculated mart metrics.

`SQL Server` `Python` `Power BI` `ABC Analysis` `K-means` `SCD2`

---

### Machine Learning

**[network-fraud-scoring](https://github.com/abdallah-bodzz/network-fraud-scoring)** — *Graph-Aware AML Fraud Detection*

Network-aware fraud scoring on 3.7M AMLSim transactions. Fused tabular XGBoost features with graph structure (degree, PageRank, community, GraphSAGE embeddings) and benchmarked the fusion against a tabular-only baseline at fixed review capacity, not AUPRC alone. The fusion model won, AUPRC 0.0438 vs. 0.0415; GraphSAGE underperformed and that result is reported, not buried. Rule-based typology matching flags fan-out, cycle, and stack patterns, and each flagged cluster gets an LLM explanation validated against source data before a reviewer sees it, 100% grounding on the held-out set. FastAPI service, operator dashboard, Docker, 31 tests.

`Python` `PyTorch Geometric` `GraphSAGE` `XGBoost` `FastAPI` `Docker`

---

**[fraud-detection-api](https://github.com/abdallah-bodzz/fraud-detection-api)** — *Production Credit Card Fraud Detection API*

I treated this as a cost problem, not a classification benchmark, so the decision threshold is picked by net dollar value instead of F1. AUPRC 0.877 on a 0.173% fraud rate, $10,484 net value protected on the held-out test set. Ships as a FastAPI service with Pydantic validation, rate limiting, structured logging, a branded operator dashboard, Docker with a healthcheck, CI/CD, and 32 tests against a real fixture model, not mocked predictions. Transaction-level precursor to network-fraud-scoring above.

`Python` `XGBoost` `FastAPI` `Docker` `CI/CD`

---

**[credit-risk-scoring](https://github.com/abdallah-bodzz/credit-risk-scoring)** — *Loan Default Prediction*

End-to-end loan default prediction: EDA, feature engineering, model comparison (LR, RF, XGBoost, LightGBM), probability calibration, business-optimised threshold. $3.55M net benefit, 152% ROI per 10k loans.

`Python` `XGBoost` `LightGBM` `scikit-learn`

---

**[heart-disease-prediction](https://github.com/abdallah-bodzz/heart-disease-prediction)** — *Clinical Screening Classifier*

Binary classifier on the UCI Cleveland dataset. Threshold-optimised screening at t=0.40: Recall 0.964, F1 0.900. 164 fewer missed diagnoses works out to roughly $8.1M saved per 10k patients.

`Python` `scikit-learn`

---

**[driveguard](https://github.com/abdallah-bodzz/driveguard)** — *Real-Time Driver Fatigue Detection*

Fatigue detection off a normal webcam. EAR/MAR geometry plus a CNN hybrid, trained on the 84k-image MRL dataset. 98.8% accuracy, 3 to 5ms CPU inference. Dual-timescale fatigue scoring, head pose via solvePnP, gesture-based alarm dismissal, 25 to 30 FPS, fully local.

`Python` `OpenCV` `MediaPipe` `TensorFlow`

---

**[sentiment-analysis](https://github.com/abdallah-bodzz/sentiment-analysis)** — *Customer Review Classification Pipeline*

NLP pipeline for review sentiment. TextBlob plus a custom neutral-word lexicon. Automated preprocessing (tokenisation, stopword removal, lemmatisation), confusion matrix, structured JSON metric export. 86.7% accuracy, precision 1.00 on the positive class.

`Python` `NLTK` `TextBlob` `scikit-learn`

---

### Quantitative Risk & Event Studies

**[2026-hormuz-blockade-analysis](https://github.com/abdallah-bodzz/2026-hormuz-blockade-analysis)** — *Cross-Asset Shock Transmission Study, v2*

Hormuz 2026: When Diplomacy Decoupled From Supply. Event study of the Strait of Hormuz crisis across 113 trading days. Update 2 turned up what I've been calling the May Paradox: WTI fell 20% while transit capacity stayed near 2%. Cross-asset shock transmission across 16 assets, 5 event windows, live interactive dashboard. [Live dashboard →](https://abdallah-bodzz.github.io/2026-hormuz-blockade-analysis/)

`Python` `SciPy` `yfinance` `Plotly`

---

**[monte-carlo-risk-simulator](https://github.com/abdallah-bodzz/monte-carlo-risk-simulator)** — *Correlated Portfolio VaR & Expected Shortfall*

Correlated portfolio Monte Carlo for VaR and Expected Shortfall. Cholesky decomposition, fat tails (Student-t, ν=5), live market data. FastAPI backend, interactive Chart.js dashboard.

`Python` `NumPy` `SciPy` `FastAPI`

---

### Valuation & Financial Engineering

**[dcf-valuation-engine](https://github.com/abdallah-bodzz/dcf-valuation-engine)** — *DCF with Live Market Data*

DCF tool pulling live yfinance data, WACC discounting, Gordon Growth terminal value, and a 7x7 sensitivity heatmap. Dark-theme UI.

`Python` `FastAPI` `yfinance`

---

**[financial-Excel-model-generator](https://github.com/abdallah-bodzz/financial-Excel-model-generator)** — *3-Statement Model Generator*

Python builds a complete 3-statement financial model (P&L, Balance Sheet, Cash Flow, DCF, scenario engine, sensitivity matrix) as a native Excel file. All formulas stay in Excel; Python only builds the structure. Base/Best/Worst scenarios via an INDEX/MATCH dropdown.

`Python` `openpyxl`

---

### Tools & Utilities

**[nb2md](https://github.com/abdallah-bodzz/nb2md)** — *Notebook to AI-Friendly Markdown*

Converts Jupyter notebooks to clean Markdown for LLM context windows. Zero dependencies, pure stdlib. Takes a 741 KB `.ipynb` down to 71 KB of `.md` (about 90% smaller). Strips base64 images, HTML widgets, and cell metadata, keeps code, prose, and text outputs. On PyPI.

```
pip install nb2md
```

`Python` `PyPI` `Zero dependencies`

---

**[data-explorer-pro](https://github.com/abdallah-bodzz/data-explorer-pro)** — *Professional Data Analysis Workbench*

A data analysis platform on Streamlit and Plotly: exploration, data prep, 20+ chart types, an AI Copilot (Gemini, Claude, or a local EchoEngine), relationship modelling, HTML report export. Layered architecture (Core, Services, UI). Took 34 earlier iterations to land on this one.

`Python` `Streamlit` `Plotly` `FastAPI`

---

### Power BI Dashboards

**[procurement-spend-analysis-dashboard](https://github.com/abdallah-bodzz/procurement-spend-analysis-dashboard)** — *Enterprise Procurement Spend Analysis & Control*

Rebuild of the Microsoft Procurement Analysis sample with a custom "Dark Ruby" theme, published on the [Fabric Community Themes Gallery](https://community.fabric.microsoft.com/t5/Themes-Gallery/Dark-Ruby-Premium-Dark-Theme-for-Executive-amp-Procurement/m-p/5287105). Star-schema model, spend visibility, savings realisation, supplier performance, 3-page report. [Live dashboard →](https://app.powerbi.com/view?r=eyJrIjoiZDMwMWNkYjctNGI4Ni00YjZjLWIwZDEtMjk1MjkyNTk1ZjE3IiwidCI6ImVhZjYyNGM4LWEwYzQtNDE5NS04N2QyLTQ0M2U1ZDc1MTZjZCIsImMiOjh9)

`Power BI` `DAX` `Star Schema` `Custom Theme`

**[customer-profitability-erp-dashboard](https://github.com/abdallah-bodzz/customer-profitability-erp-dashboard)** — *Enterprise Customer Profitability & Financial Control*

Rebuild of the Microsoft Customer Profitability sample with a custom "Earthy Botanical" theme, published on the [Fabric Community Themes Gallery](https://community.fabric.microsoft.com/t5/Themes-Gallery/Earthy-Botanical-Professional-Custom-Theme-for-Executive/m-p/5284502). Margin analysis, segmentation, 4-page executive report. [Live dashboard →](https://app.powerbi.com/view?r=eyJrIjoiNDhjZjY3YzgtMzBmMC00ZGRiLTliYzgtZDA4OTQ0YTFmOGViIiwidCI6ImVhZjYyNGM4LWEwYzQtNDE5NS04N2QyLTQ0M2U1ZDc1MTZjZCIsImMiOjh9)

`Power BI` `DAX` `Star Schema` `Custom Theme`

| Project | What it covers |
|---------|----------------|
| [powerbi-wake-county-budget-report](https://github.com/abdallah-bodzz/powerbi-wake-county-budget-report) | Government expenditure analysis, Wake County NC, FY2017 to 2019. Star schema from raw CSVs, YTD spend, budget utilisation, drill-through to cost-center level. |
| [mortgage-trading-analysis-powerbi](https://github.com/abdallah-bodzz/mortgage-trading-analysis-powerbi) | Mortgage trading desk simulation: loan pipeline review, counterparty bid evaluation, FICO-based pricing. |
| [financial-analysis-powerbi-dashboard](https://github.com/abdallah-bodzz/financial-analysis-powerbi-dashboard) | 12-page dark dashboard: revenue/profit decomposition, customer segmentation, NPV/IRR, DCF, payback. |
| [supply-chain-analytics-powerbi](https://github.com/abdallah-bodzz/supply-chain-analytics-powerbi) | Make-vs-buy decision tool: supplier quote analysis, volume scenario planning, manufacturing cost comparison. |
| [customer-churn-analysis-powerbi](https://github.com/abdallah-bodzz/customer-churn-analysis-powerbi) | Telecom churn analysis: 6,687 customers, 26.86% churn, broken down by reason, geography, contract, data plan. |
| [hr-analytics-powerbi](https://github.com/abdallah-bodzz/hr-analytics-powerbi) | Employee attrition on the Atlas Labs dataset; automated variance logic surfaced 3 high-attrition clusters on first load. |
| [time-series-analysis-powerbi-dashboard](https://github.com/abdallah-bodzz/time-series-analysis-powerbi-dashboard) | Retail PoS plus MSFT financials: rolling windows, YTD/YoY DAX, forecasting visuals. |

---

### Excel Financial Models

| Project | What it covers |
|---------|----------------|
| [financial-modeling-excel](https://github.com/abdallah-bodzz/financial-modeling-excel) | Income statements, cap rates, forecasts, dynamic models for real estate. |
| [net-revenue-management-excel](https://github.com/abdallah-bodzz/net-revenue-management-excel) | Full NRM business case for an FMCG supplier: market share, portfolio profitability, promotional ROI. |
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
| **Visualisation & BI** | Power BI (DAX, drill-through, bookmarks, What-If, custom theming) · Plotly · Matplotlib · Chart.js |
| **Backend & APIs** | FastAPI · Pydantic · Uvicorn · Docker |
| **Databases** | SQL Server · PostgreSQL · MySQL |
| **Tools** | Jupyter · Streamlit · Excel (DCF, 3-statement, NRM) · Git · GitHub Actions · python-dotenv · rich |

---

## Content, @data_w_bodzz

I post Power BI builds, SQL deep dives, and project breakdowns on TikTok and YouTube.

200,000+ total views, 1,500+ followers. Best video so far is on Power BI normalization and lookup tables, 16k+ views.

---

## Connect

[![Portfolio](https://img.shields.io/badge/Portfolio-abdallah--bodzz.github.io-1A5276?style=flat-square&logo=github)](https://abdallah-bodzz.github.io/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abdallah-abdelhady-4187802b2)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:xabdallahxabdallahx@gmail.com)
[![TikTok](https://img.shields.io/badge/TikTok-%23000000.svg?style=flat-square&logo=TikTok&logoColor=white)](https://tiktok.com/@data_w_bodzz)
[![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=flat-square&logo=YouTube&logoColor=white)](https://youtube.com/@abdallahabdelhady8713)
[![X](https://img.shields.io/badge/X-black.svg?style=flat-square&logo=X&logoColor=white)](https://x.com/hottestboda)
[![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?style=flat-square&logo=Instagram&logoColor=white)](https://instagram.com/abdallah_abdelhadi)
