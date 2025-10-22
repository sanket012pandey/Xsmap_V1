Xsmap_v1 is an advanced stock market prediction model designed to forecast high-risk volatility regimes in the Indian stock market (NSE). The model combines historical market data, cross-market features, macroeconomic indicators, momentum and trend analysis, and spectral/cyclical features to generate robust predictions using a hybrid ensemble of XGBoost, Random Forest, and LightGBM, stacked into a meta-model.

This project is ideal for quantitative finance enthusiasts, algorithmic traders, and data scientists interested in predictive analytics for financial markets. 
Features

Historical Data Analysis: Uses 10 years of daily NSE index data.

Cross-Market Context: Integrates Bank Nifty, India VIX, S&P500, Nasdaq, USD/INR, Crude Oil, and Gold.

Enhanced Feature Engineering:

Volatility (ATR, rolling std, GK volatility, volatility ratios)

Momentum divergence (price, RSI, MACD, volume)

Trend indicators (SMA, EMA, Bollinger Bands)

Spectral & cyclical features (FFT analysis, yearly/monthly/weekly cycles)

Macro features (bull/bear regime, global flows proxy, volatility regime)

Data Cleaning & Validation: Handles missing values, outliers (Z-score), duplicates, and zero volume entries.

Machine Learning Ensemble: XGBoost, Random Forest, LightGBM with hyperparameter tuning via RandomizedSearchCV.

Stacked Meta-Model: Combines all three models with a logistic regression meta-estimator.

Imbalanced Data Handling: Uses SMOTETomek to balance the training dataset.

Model Evaluation: Test accuracy, classification report, confusion matrix, and feature importance.
