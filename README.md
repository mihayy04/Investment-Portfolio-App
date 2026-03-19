# Investment Portfolio Manager 📈

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-Web_App-red.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data_Processing-150458.svg)

## 📌 Project Overview
This is a web-based financial application built with **Python** and **Streamlit** that allows users to track and manage their investment portfolios. The app fetches real-time market data, calculates profits and total values across multiple currencies, and provides interactive data visualization.

## 🚀 Key Features
* **Real-Time Data:** Integrates the Yahoo Finance API (`yfinance`) to fetch live asset prices based on stock tickers.
* **Multi-Currency Support:** Dynamically converts portfolio values and purchase prices between RON, EUR, and USD.
* **Interactive UI:** A clean, responsive user interface built with Streamlit, featuring a sidebar menu, data metric displays, and state management.
* **Data Visualization:** Generates bar charts using `matplotlib` to visually compare asset allocations and total values.
* **Excel Export:** Processes the portfolio data using `pandas` and exports fully formatted reports to Excel via `openpyxl` (with auto-adjusted column widths).

## 🛠️ Technology Stack
* **Language:** Python
* **Frontend Framework:** Streamlit
* **Data Manipulation:** Pandas
* **Financial Data API:** yfinance
* **Visualization:** Matplotlib
* **File Handling:** OpenPyXL

## ⚙️ How to Run
1. Clone this repository.
2. Install the required dependencies:
   `pip install streamlit pandas yfinance matplotlib openpyxl`
3. Run the Streamlit application:
   `streamlit run app.py`
