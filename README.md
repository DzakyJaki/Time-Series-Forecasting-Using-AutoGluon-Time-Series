# 📊 Retail Sales Index Forecasting with AutoGluon & Chronos LLM

This project implements probabilistic time series forecasting on Indonesia’s **Retail Sales Index (RSI)** using models provided by **AutoGluon TimeSeries**, including **Chronos (LLM-based)** models.

## 📁 Project Overview

- Task: Monthly retail sales forecasting (2012–2025)
- Data Source: Bank Indonesia (7 product categories)
- Target: Forecast RSI for 12 months (Feb 2024 – Jan 2025)

## ⚙️ Models Used

- **Chronos** LLM (Zero-Shot & Fine-Tuned)
- Deep Learning: Temporal Fusion Transformer, DeepAR, PatchTST, TiDE
- Tabular ML: RecursiveTabular, DirectTabular (LightGBM)
- Statistical: AutoETS, DynamicTheta, NPTS
- Baseline: SeasonalNaive

## 📊 Results Summary

- **Chronos [base] (fine-tuned)** achieved the best overall performance.
- Compared 20+ model variants using 7 evaluation metrics (SQL, MAE, RMSE, etc.)

## 🧪 Notebook

The core experiment and evaluation pipeline is implemented in:

[📔 View Notebook](AutoGluon_IPR_Forecasting.ipynb)

## 📌 Notes

- Forecasting is done univariately (one model per product category).
- Data was standardized using Z-score normalization before modeling.
