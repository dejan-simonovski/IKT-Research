# Bitcoin prediction model using XGBoost (Buy/Sell Classification)

Research paper made by Dejan Simonovski 211039 & Elena Boshkoska 213040 for UKIM FCSE Skopje

This project implements a machine learning model to predict daily Bitcoin price movements based on historical market data. Using a combination of technical indicators, lag features, volatility measures, and time-based features, the model attempts to classify whether the price will increase or decrease the next day.
The model achieves an overall accuracy of 62%, indicating it captures general trends in the market. However, performance is asymmetric across classes: it is highly effective at identifying price decreases (recall ≈ 98%), but struggles to correctly predict price increases (recall ≈ 5%). This suggests that while the model is conservative and avoids false positives for price drops, it has difficulty capturing upward movements, which are less frequent in the dataset.

### Key contributions include:

* Extensive feature engineering incorporating price returns, moving averages, RSI, MACD, Bollinger Bands, ATR, volume features, and lagged/rolling statistics.

* Implementation of a time-series aware train/test split to prevent data leakage.

* Use of XGBoost with class balancing to account for moderately imbalanced target distribution.

* Comprehensive evaluation and visualization, including feature importance, correlation heatmaps, ROC curves, and prediction accuracy over time.

Overall, the project demonstrates the challenges of predicting highly volatile financial markets and provides a foundation for further improvements, such as enhancing prediction of upward trends or incorporating alternative data sources.
