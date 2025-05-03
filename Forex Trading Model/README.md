# Forex Trading Strategy Using Machine Learning

## Objective
To develop a regression-based trading model that predicts currency pair movements and classifies pairs by forecastability, using Python, PyCaret, and real-time data from Polygon API.

## Tools Used
- Python (PyCaret, pandas, scikit-learn)
- MongoDB
- Polygon API
- Matplotlib
- CSV export

## Key Features
- Real-time data ingestion for 10 major currency pairs
- Feature engineering: volatility, momentum, fractal dimension
- Model comparison: Linear Regression, Ridge, Lasso
- Predictability classification of currency pairs
- Output includes CSV summary and PDF report

## Files
- `Forex_Trading.py` — Main code
- `classification_results.csv` — Output of forecastability classification
- `Final project.pdf` — Report summary with charts and findings

## Result
The model identified 3 currency pairs with consistently low MAE and strong signal strength, enabling selective risk-aware trading strategies.
