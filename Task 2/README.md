# Task 2: Predict Future Stock Prices – Short-Term Forecasting

## 📌 Objective
Build a regression model to predict the **next day's closing price** of a selected stock (e.g., AAPL), using historical market data (Open, High, Low, Volume).

---

## 📁 Dataset
- **Source**: [Yahoo Finance](https://finance.yahoo.com/)
- **Fetched using**: `yfinance` Python library
- **Stock**: AAPL (Apple Inc.)
- **Date Range**: 2022-01-01 to 2024-12-31
- **Features Used**: `Open`, `High`, `Low`, `Volume`
- **Target**: `Next day's Close` (created via `.shift(-1)`)

---

## 🛠️ Steps Performed

### 1. Data Fetching & Preprocessing
- Loaded daily stock data using `yfinance`
- Created target by shifting the `Close` column
- Dropped last row (NaN target)
- Split into training and test sets (80/20)

### 2. Model Training
- Applied **Linear Regression** model
- (Optional) Random Forest Regressor for improved performance

### 3. Evaluation & Visualization
- **Metric**: Root Mean Squared Error (RMSE)
  - Achieved RMSE ≈ 3.77
- Compared actual vs. predicted closing prices using line plots

---

## 🔍 Key Findings
- The model captured trends accurately with low error (~1.5–2%)
- Linear model worked surprisingly well for short-term forecasting
- Predicted line closely followed real price movement

---

## 📚 Libraries Used
- `pandas`, `numpy`, `matplotlib`, `scikit-learn`, `yfinance`

---

## Outcome
Successfully implemented a basic but effective short-term stock prediction model using real financial data. This serves as a strong baseline for future time-series models (e.g., LSTM).

