````markdown
# RSI Trading Analysis

A Jupyter Notebook–based project that retrieves historical market data, computes the Relative Strength Index (RSI), and visualizes 
trading signals for data-driven decision making.

---

## 📋 Project Overview

This repository contains a single Jupyter Notebook (`RSI.ipynb`) in which I:

1. Fetch Historical Price Data :
   - Use `yfinance` (or similar APIs) to pull OHLCV data for assets like BTC–USD.  

2. Compute RSI Indicator:  
   - Implement an RSI function in pandas (default period = 14).  
   - Identify overbought/oversold conditions (e.g., RSI > 70 or < 30).  

3. Generate Buy/Sell Signals:  
   - Mark potential entry/exit points based on RSI crossovers.  

4. Visualize Results:  
   - Plot price chart with RSI subplot and annotated signals.  

5. Export Findings:
   - Save plots as images and signal data as CSV for further analysis.

---

## 🛠️ Tech Stack & Libraries

- Python 3.8+ 
- Jupyter Notebook for interactive analysis  
- pandas for data manipulation  
- numpy for numerical operations  
- matplotlib / plotly for plotting  
- yfinance (or CCXT) for data retrieval  
- TA-Lib *(optional)* for RSI calculation  

---

## 🚀 Getting Started

1. Clone the repository  
   ```bash
   git clone https://github.com/sakshyambanjade/RSI-Trading-Bot-.git
   cd RSI-Trading-Bot-
````

2. Create & activate a virtual environment

   ```bash
   python3 -m venv venv
   source venv/bin/activate    # macOS/Linux
   venv\Scripts\activate.bat   # Windows
   ```

3. Install dependencies

   ```bash
   pip install -r requirements.txt
   ```

4. Launch Jupyter Notebook

   ```bash
   jupyter notebook RSI.ipynb
   ```

5. Run all cells to fetch data, compute RSI, and view your visualizations.

---

## 📈 Notebook Structure

| Section                  | Description                                        |
| ------------------------ | -------------------------------------------------- |
| 1. Imports & Config  | Load libraries, set asset symbol & date range.     |
| 2. Data Retrieval    | Fetch OHLCV data via `yfinance` or `CCXT`.         |
| 3. RSI Calculation   | Compute RSI values and add to DataFrame.           |
| 4. Signal Generation | Flag buy/sell points where RSI crosses thresholds. |
| 5. Visualization     | Plot price & RSI; annotate entry/exit signals.     |
| 6. Export            | Save signals to CSV and charts as PNG.             |

---

## 📝 How to Interpret the Results

* RSI Subplot:

  * Overbought (>70) and oversold (<30) bands marked.
  * Green markers for “Buy” points; red for “Sell” points.
* Signal CSV: Each row includes the timestamp, price, RSI value, and signal type.

