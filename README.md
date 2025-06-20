# Favorita Store Sales Forecasting

This project applies Time Series Forecasting techniques using tree-based ensemble models (XGBoost and LightGBM) on the Favorita grocery store dataset to predict item sales.

## Problem Statement

Forecast unit sales for thousands of products sold across multiple Favorita stores in Ecuador — accounting for seasonality, holidays, promotions, and store-level variations.

## Dataset

- Source: Kaggle - [https://www.kaggle.com/competitions/store-sales-time-series-forecasting/data]
- Includes sales data by item, store, date, promotions, holidays, and transactions

## Key Techniques

- **Data preprocessing**: Dataset Relationship Mapping & Merging Strategy
- **Time Series EDA**: Seasonal trends, outliers, spikes, holiday effects
- **Feature Engineering**:
  - Lag features & rolling means
  - Date Features, promo flags, holiday indicators, Oil Feature Imputation & Smoothing
  - Payday Feature, Earthquake Period Flag (Post-April 16, 2016)
- **Modeling**:
  - LightGBM with hyperparameter tuning (RMSLE: 0.6154)
  - XGBoost with optimized config (RMSLE: 0.4573)
  - SHAP for model explainability
- **Forecast Horizon**: 15-day window

## Power BI Dashboard

An interactive Power BI dashboard was created to visualize:

- Sales KPIs
- Trends & seasonality
- Store-wise performance
- Forecast accuracy 

Dashboard Files:
- [Dashboard PDF](./favorita_powerbi_dashboard.pdf) — quick view (included in this repo)
- [Power BI File (.pbix on Google Drive)](https://drive.google.com/file/d/1zTfQq9k-w6pll2BUGerZ-Dbl7wqEYFC7/view?usp=sharing) — open/edit in Power BI Desktop


## Tools Used

- Python: `pandas`, `seaborn`, `matplotlib`, `xgboost`, `lightgbm`, `shap`
- Power BI for interactive visualization

---

## How to Run

1. Clone this repo or open the notebook in Google Colab / Jupyter
2. Download data from Kaggle and place in the working directory
3. Run the notebook cells in order

---

This project demonstrates real-world time series modeling combined with business-focused visualization for actionable insights.
