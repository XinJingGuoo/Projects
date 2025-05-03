# Forex Trading Strategy Using Machine Learning

This project develops a real-time trading system for major currency pairs using Python, PyCaret, and the Polygon API. It combines market data ingestion, statistical feature engineering, model selection, and performance classification to identify the most forecastable pairs for quantitative trading strategies.

---

## Objective

To predict currency pair price movements using machine learning regression models and classify pairs based on forecastability using Mean Absolute Error (MAE) thresholds.

---

## Tools and Libraries

- **Programming**: Python, PyCaret, scikit-learn, pandas
- **Data Ingestion**: Polygon.io Forex API
- **Data Storage**: MongoDB
- **Modeling**: Linear Regression, Ridge, Lasso (via PyCaret)
- **Evaluation**: MAE (Mean Absolute Error)
- **Output**: CSV (model results), PDF Report

---

## Workflow

1. **Data Collection**:  
   - Fetched real-time forex data for 10 major currency pairs via Polygon API.  
   - Stored time-series exchange rate data in MongoDB.

2. **Feature Engineering**:  
   - Calculated volatility, Keltner Bands, fractal dimension, and correlation features.  
   - Constructed synthetic indicators from top pairs for ensemble prediction.

3. **Modeling**:  
   - Used PyCaret’s AutoML to compare regression models (based on MAE).  
   - Trained model on historical stats for synthetic pairs, saved best model.

4. **Forecastability Classification**:  
   - Measured MAE on each pair's 20-point test window.  
   - Ranked pairs into `FORECASTABLE`, `UNDEFINED`, and `NON-FORECASTABLE`.

5. **Output**:  
   - PDF report with analysis and conclusion  
   - CSV file with MAE and classification results for all currency pairs

---

## Files in this Repository

| File | Description |
|------|-------------|
| `Forex_Trading.py` | Full pipeline for data ingestion, processing, modeling, and classification |
| `classification_results.csv` | Forecastability classifications and MAE scores |
| `Final project.pdf` | Presentation-ready summary of methodology and findings |

---

## Results

- **Top Forecastable Pairs**: EURUSD, GBPCHF, USDCHF  
- **MAE Accuracy**: Best-performing model achieved < MAE: 0.0035 for forecastable pairs  
- **Impact**: Enables targeted FX strategies based on quantifiable predictability

---

## Example Output

- **Hour 6**: GBPUSD to USDJPY ratio: 1.2187216742, Profit 
- **Hour 7**: GBPUSD to USDJPY ratio: 1.2169976626, Profit 
- **Hour 8**: GBPUSD to USDJPY ratio: 1.2169976626, Profit



---

## Author

**Xinjing Guo**  
- Master’s in Management of Technology, NYU  
- GitHub: [XinJingGuoo](https://github.com/XinJingGuoo/Projects)  
- Website: [Portfolio](https://xinjingguoo.github.io/xinjingguo.github.io/)

---

## Contact

If you're a hiring manager or interested in discussing the strategy further, feel free to [connect on LinkedIn](https://www.linkedin.com/in/xinjing-guo/).
