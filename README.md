# Predictive-Equity-Modeling-with-Factor-Based-Machine-Learning

This project implements a multi-factor stock return prediction model using the Fama-MacBeth regression framework, applied to S&P 1500 stocks over a 40-year historical dataset (1980–2019).
We designed, trained, and evaluated a rolling-window supervised learning model to generate monthly return forecasts and backtest a long-short portfolio strategy.

Project Overview
Objective: Identify statistically significant return-predictive factors and build a model capable of forecasting equity returns with strong risk-adjusted performance.

Data: 50+ monthly financial factors and returns for S&P 1500 stocks, covering 1980–2019.

Techniques:

Feature engineering with z-score normalization, winsorization, and multicollinearity screening

Factor selection based on Fama-MacBeth two-pass regression and t-statistics filtering

Construction of a rolling-window prediction pipeline for out-of-sample testing

Evaluation using Sharpe ratio, alpha analysis, and factor-model residual diagnostics

Key Results
Identified a robust set of six predictive factors after rigorous statistical screening.

Built a dynamic monthly retraining model capable of adapting to evolving market conditions.

While the hedge portfolio underperformed benchmarks during out-of-sample testing, the framework highlights valuable lessons in model selection, training window sensitivity, and the challenges of financial predictive modeling.

Collaborators
This project was completed as part of the CFM 301 Financial Data Analytics course at the University of Waterloo.
Team Members:

Jack Zhao (Jiaxi Zhao)

Sean Lee

Germain Zhang-Houle

Rain Luo

Alan Zheng

Ballerina Liang

Repository Contents
CFM301_Final_Project.ipynb: Full modeling pipeline and backtesting code

merged_df.sas7bdat: Raw factor dataset (dataset not uploaded due to licensing restrictions)

ff_factors.xlsx: Fama-French benchmark factor dataset

Project report (CFM301 Financial Data Analytics Report.pdf): Detailed methodology and findings

Technologies Used
Python (pandas, numpy, scipy, statsmodels, linearmodels, matplotlib, seaborn)

Fama-MacBeth cross-sectional regression modeling

Portfolio construction and backtesting techniques
