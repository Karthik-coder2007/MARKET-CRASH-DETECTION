# MARKET-CRASH-DETECTION
📉 Market Crash Detection using CUSUM & Machine Learning
# Overview

This project focuses on detecting and predicting stock market crashes using statistical and machine learning techniques on the
S&P 500 Index and NASDAQ data.
It combines:

1.CUSUM Algorithm → Detects continuous market declines
2.Volatility Analysis → Measures market risk
3.Machine Learning Models → Predicts future crash events

# Objectives
 
Detect market crashes using CUSUM
Analyze market volatility
Predict future crashes using ML models
Compare crash behavior across multiple markets

# Dataset

Source: Yahoo Finance
Data includes:
Date
Open, High, Low, Close prices
Symbols used:
^GSPC → S&P 500
^IXIC → NASDAQ Composite

# Methodology
 
 1. Data Preprocessing
Converted closing prices to daily returns
Removed missing values

 2. CUSUM Algorithm (Crash Detection)
Detects continuous downward movements
Generates crash signals when cumulative loss exceeds a threshold

  3. Volatility Analysis
  Calculated rolling standard deviation (20-day window)

  4. Machine Learning Model

  Model used: Random Forest
  Features:
  Returns
  Volatility
  CUSUM
  Target

 5. Visualization

Price trends with crash points
CUSUM chart with threshold
Volatility analysis
Cross-market crash comparison

 6.Results
 

Successfully detected:
Continuous market declines
High-risk periods
ML model improved predictive capability over pure statistical methods

 7.Key Insights

Markets often crash due to continuous small declines, not just single-day drops
High volatility periods correlate with crashes
Combining CUSUM + ML improves detection and prediction

 8.Limitations

Sensitive to threshold selection
Class imbalance in crash data
Cannot guarantee future predictions

9.Future Improvements

Add GARCH model for volatility forecasting
Use XGBoost for better performance
Integrate news sentiment analysis (NLP)
Build real-time alert system

 10.Tech Stack
Python
Pandas, NumPy
Matplotlib
Scikit-learn
yFinance

 #Conclusion

This project demonstrates how combining statistical techniques like CUSUM with machine learning models can effectively detect and predict market crashes, providing valuable insights for financial risk management.
