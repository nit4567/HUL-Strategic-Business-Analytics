# Forecasting, Sentiment & Financial Analysis for HUL (Capstone Project)

## 📄 Overview
This repository contains the documentation, research reports, and presentation slides for a Business Data Management (BDM) Capstone Project focused on **Hindustan Unilever Limited (HUL)**.

The project integrates internal financial data with external macroeconomic indicators and unstructured consumer feedback to solve critical FMCG challenges regarding inventory, production alignment, and brand perception.

## 📂 Repository Contents

| File Name | Type | Description |
| :--- | :--- | :--- |
| `Project Final Report.pdf` | **Full Report** | The complete analysis including Google Trends integration, LDA Topic Modeling, and Financial Ratio benchmarking (vs. ITC, Dabur, etc.). |
| `Project Midterm Report.pdf` | **Report** | Initial analysis comparing Ridge Regression vs. XGBoost and baseline VADER sentiment scoring. |
| `HUL Capstone Presentation.pdf` | **Slides** | The executive presentation summarizing the business context, methodology, and strategic recommendations. |

## 🧠 Key Problem Statements & Methodology

### 1. Demand Forecasting
* **Goal:** Forecast segment-wise revenue (Foods, Home Care, Personal Care) to align production with demand.
* **Approach:** Built a multivariate time-series model using 29 quarters of financial data aggregated with macroeconomic indicators (CPI, CSI).
* **Enhancement:** Integrated **Google Trends** search volume to capture consumer interest signals.
* **Result:** **Ridge Regression** outperformed XGBoost and SARIMA. The integration of Google Trends specifically improved the $R^2$ score for the difficult "Foods" segment to **0.65**.

### 2. Sentiment Analysis
* **Goal:** Analyze 3,000+ customer reviews from Walmart to uncover hidden pain points.
* **Approach:** Used **VADER** for sentiment scoring and **LDA (Latent Dirichlet Allocation)** for topic modeling.
* **Key Insight:** Identified a "Rating-Sentiment Disconnect" where products with high ratings (e.g., Pond's Cold Cream) lacked emotional enthusiasm. **Packaging (Topic 5)** was identified as the primary driver of negative sentiment (28% negative).

### 3. Financial Efficiency Analysis
* **Goal:** Benchmark HUL's operational efficiency against peers (ITC, Dabur, Britannia, Marico).
* **Metrics:** Cash Conversion Cycle (CCC), Inventory Turnover, and Asset Turnover.
* **Finding:** HUL maintains a superior **negative CCC (-55 to -85 days)**, providing a ~100-day lead-time advantage over industry peers, allowing it to self-fund operations using supplier capital.

## 🛠️ Tools & Technologies
* **Forecasting:** Ridge Regression, XGBoost, Time-Series Analysis.
* **NLP:** VADER Sentiment Analysis, LDA Topic Modeling, NLTK.
* **Financials:** Ratio Analysis (CCC, Stock-to-Sales), Z-Score Standardization.
