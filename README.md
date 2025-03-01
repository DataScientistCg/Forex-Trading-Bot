# Forex Trading Bots

This repository contains **3 separate Forex Trading Bots**, each implementing different trading strategies:

1. **LSTM-Based Trading Bot** (`A_Final_Testing_code_.py`)
2. **Klinger Volume Oscillator (KVO) Bot** (`kvo_fx.py`)
3. **Supertrend Indicator Bot** (`supertrendx.py`)

## **1️⃣ LSTM-Based Trading Bot (`A_Final_Testing_code_.py`)**
This bot is **ML-based** and requires **data processing, machine learning, and trading-related** libraries.

### **Libraries Used:**
- `MetaTrader5` → For executing trades on MT5.
- `colorama` → For colored terminal output.
- `datetime` → Handling date and time.
- `joblib` → Saving and loading trained ML models.
- `numpy` → Numerical computations.
- `pandas` → Handling and manipulating data.
- `sklearn.preprocessing` → Data scaling and preprocessing.
- `ta` → Technical analysis indicators.
- `tensorflow.keras.models` → Implementing the LSTM model.
- `time` → Handling time-based operations.
- `traceback` → Debugging and error handling.
- `warnings` → Suppressing unnecessary warnings.

---

## **2️⃣ Klinger Volume Oscillator (KVO) Bot (`kvo_fx.py`)**
This bot is **volume-based** and uses libraries for **technical analysis and trade execution**.

### **Libraries Used:**
- `MetaTrader5` → For executing trades on MT5.
- `datetime` → Handling date and time.
- `numpy` → Numerical computations.
- `pandas` → Handling and manipulating data.
- `ta` → Technical indicators (like ATR, Pivot Points).
- `time` → Handling time-based operations.
- `traceback` → Debugging and error handling.
- `warnings` → Suppressing unnecessary warnings.

---

## **3️⃣ Supertrend Indicator Bot (`supertrendx.py`)**
This bot focuses on **trend-following strategies** using the **Supertrend indicator**.

### **Libraries Used:**
- `MetaTrader5` → For executing trades on MT5.
- `datetime` → Handling date and time.
- `numpy` → Numerical computations.
- `pandas` → Handling and manipulating data.
- `ta` → Technical indicators (like ATR, Pivot Points, Supertrend).
- `time` → Handling time-based operations.
- `traceback` → Debugging and error handling.
- `warnings` → Suppressing unnecessary warnings.

---

### **Conclusion**
- **All three bots** use:
  - `MetaTrader5`, `datetime`, `numpy`, `pandas`, `ta`, `time`, `traceback`, `warnings`.
- **LSTM bot** additionally uses:
  - `joblib`, `sklearn.preprocessing`, `tensorflow.keras.models`, `colorama`.

Would you like me to add this breakdown in the README as well? 😊

---

## 1️⃣ LSTM-Based Trading Bot (`A_Final_Testing_code_.py`)
### Overview
This bot utilizes a **Machine Learning (LSTM)** model for **Forex price prediction** and **automated trading**. It employs **multiple technical indicators** to analyze market trends and generate entry/exit signals.

### Features
- **LSTM Model for Price Prediction**
- **Technical Indicators**:
  - Bollinger Bands, ADX, Fibonacci Levels, RSI, MACD, SMA, Stochastic Oscillator, ATR.
- **Signal Detection Functions**:
  - `determine_ichimoku_cloud_signal()` - Detects Ichimoku Cloud trends.
  - `determine_pivot_signal()` - Applies pivot point strategy.
  - `determine_donchian_channels_signal()` - Identifies breakouts using Donchian Channels.
- **Volatility & Market Trend Detection**:
  - `calculate_volatility()` - Analyzes market volatility.
  - `is_sideways_market()` - Checks if the market is trending or moving sideways.
- **Trade Execution**:
  - `market_order_with_atr()` - Executes trades with ATR-based stop loss.
  - `close_order_with_atr()` - Closes open trades based on ATR logic.

### Run the Bot
```sh
python A_Final_Testing_code_.py
```

---

## 2️⃣ Klinger Volume Oscillator (KVO) Bot (`kvo_fx.py`)
### Overview
This bot uses the **Klinger Volume Oscillator (KVO)** for **volume-based trend detection** and trade execution.

### Features
- **Volume Analysis**:
  - `klinger_volume_oscillator()` - Calculates the Klinger Volume Oscillator.
  - `get_ohlc_data_with_volume()` - Fetches OHLC data along with volume.
- **Technical Indicators**:
  - `calculate_atr()` - Computes **Average True Range (ATR)**.
  - `calculate_pivots()` - Calculates pivot points.
  - `calculate_support_resistance()` - Identifies support and resistance levels.
- **Trade Execution**:
  - `market_order()` - Places market orders.
  - `close_order()` - Closes open trades.
  - `calculate_sl_tp()` - Computes **Stop Loss (SL) and Take Profit (TP)**.

### Run the Bot
```sh
python kvo_fx.py
```

---

## 3️⃣ Supertrend Indicator Bot (`supertrendx.py`)
### Overview
This bot implements a **Supertrend Indicator-based strategy** for detecting and trading trends in the Forex market.

### Features
- **Trend Detection**:
  - `signal()` - Generates Buy/Sell trading signals.
  - `get_trend_dominance_for_timeframes()` - Analyzes trend dominance across multiple timeframes.
- **Technical Indicators**:
  - `calculate_atr()` - Computes **Average True Range (ATR)**.
  - `calculate_pivots()` - Calculates pivot points.
  - `calculate_support_resistance()` - Identifies support and resistance levels.
- **Trade Execution**:
  - `market_order()` - Places market orders.
  - `close_order()` - Closes open trades.
  - `get_exposure()` - Calculates market exposure.
  - `calculate_sl_tp()` - Sets **Stop Loss (SL) and Take Profit (TP)**.

### Run the Bot
```sh
python supertrendx.py
```

---

## Installation
### Prerequisites
Ensure you have the following installed:
- Python 3.x
- Required Python libraries (install using `requirements.txt` if available)

### Setup
```sh
# Clone the repository
git clone https://github.com/yourusername/Forex_Trading_Bot.git
cd Forex_Trading_Bot

# Install dependencies
pip install -r requirements.txt
```

### Dependencies
The project requires the following Python libraries:
- **MetaTrader5** - MT5 trading platform integration
- **colorama** - For colored terminal output
- **datetime** - Date and time handling
- **joblib** - For saving/loading ML models
- **numpy** - Numerical computations
- **pandas** - Data handling and manipulation
- **sklearn.preprocessing** - Data scaling and preprocessing
- **ta** - Technical analysis indicators
- **tensorflow.keras.models** - LSTM model implementation
- **time** - Time-related operations
- **traceback** - Error handling and debugging
- **warnings** - Suppressing warnings

---

## Disclaimer
This bot is for educational and research purposes only. Trading in Forex markets involves risks, and users should trade at their own discretion.

## Contributions
Feel free to fork this repository and submit pull requests for improvements.

## License
This project is licensed under the MIT License.

---

### Notes:
- If there are more features or configurations, they can be added to the README.
- If `requirements.txt` is missing, we can generate one by checking dependencies.

