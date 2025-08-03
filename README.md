# 📈 Forecasting Stock Market Trends Using Machine Learning

This project applies machine learning to historical stock market data to forecast both **short-term trends** (using regression models) and **long-term trends** (using Facebook Prophet). We evaluate predictive accuracy, visualize historical movements, and generate **forecasts up to 2030**.

---

## 📄 Project Overview

Financial markets are volatile and complex, but machine learning offers tools to detect patterns and support data-driven decisions. In this capstone project, we explore a complete data science pipeline from collection and preparation to modeling and evaluation.

Now extended with **long-term time-series forecasting using Prophet**, this project can project price trends years into the future.

The work is documented in one notebook:
- [`predictive_analysis.ipynb`](https://github.com/evandobler98/stock_market_capstone/blob/main/predictive_analysis.ipynb): Full pipeline (includes EDA + forecasting)

---

## 🔍 Features

- Historical stock data pulled from **Nasdaq** and MarketWatch
- Feature engineering with moving averages, RSI, and volume spikes
- Exploratory data visualization (pairplots, heatmaps, trend plots)
- Machine learning models:
  - Linear Regression  
  - Random Forest Regressor  
  - XGBoost Regressor  
- **NEW:** Long-term forecasting using **Prophet** (projects stock prices to 2030)  
- Evaluation using MAE, RMSE, and R²  
- Future ideas: NLP-based indicators, LSTM forecasting, and interactive dashboards  

---

## 🧪 Tech Stack

- Python  
- `yfinance`, `pandas`, `numpy`, `matplotlib`, `seaborn`  
- `scikit-learn`, `xgboost`, `prophet`  
- LaTeX (LLNCS Template)

---

## 📚 Documentation

- **📘 Overleaf Report:**  
  [View Full LaTeX Report on Overleaf](https://www.overleaf.com/read/qpmmxndcknyt)

- **💻 GitHub Repository:**  
  [View Source Code](https://github.com/evandobler98/stock_market_capstone)

- **📓 Notebook (Full Project):**  
  [`predictive_analysis.ipynb`](https://github.com/evandobler98/stock_market_capstone/blob/main/predictive_analysis.ipynb)

---

## 📈 Data Sources

- [Nasdaq – Main Site](https://www.nasdaq.com/)  
- [MarketWatch – Investing Portal](https://www.marketwatch.com/investing?mod=top_nav)

---

## ⚙️ Setup & Installation  

Follow these steps to set up your environment and run the project:

### 1️⃣ Create a Virtual Environment (Recommended)

**macOS/Linux:**  
```bash
python3 -m venv .venv
source .venv/bin/activate


Windows:

```bash
Copy code
python -m venv .venv
.venv\Scripts\activate
```
✅ Tip: You’ll see (.venv) before your terminal prompt once activated.

### 2️⃣ Install Dependencies
```bash
Copy code
pip install --upgrade pip  
pip install -r requirements.txt
```
If Prophet is missing, install it manually:

```bash
Copy code
pip install prophet
```

### 3️⃣ Run the Stock Forecast Script
To forecast all available stocks to 2030, run:

```bash
Copy code
python forecast_stocks.py
```
This will:
✅ Load the dataset (Stock Price Data.xlsx)
✅ Forecast each stock’s future prices to 2030 using Prophet
✅ Generate and display forecast plots
✅ Save all forecasted results to stock_forecasts_to_2030.csv

### 4️⃣ View Results
Plots → Forecasts for each stock (AAPL, TSLA, MSFT, AMZN)

CSV Output → stock_forecasts_to_2030.csv contains predicted prices (yhat), plus lower/upper confidence intervals

📦 Example requirements.txt
Save this as requirements.txt before running the installation step:

```text
Copy code
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
prophet
openpyxl   # for reading Excel files
```

### 📌 Author
#### Evan T. Dobler
#### Northwest Missouri State University
#### Email: S576852@nwmissouri.edu
#### Alt: dobler.evan.t.2016@gmail.com

