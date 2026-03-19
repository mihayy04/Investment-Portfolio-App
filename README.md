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

## 📖 User Guide

### Prerequisites
Before running the application, ensure you have the required Python packages installed. You can install them via terminal:
```bash
pip install pandas streamlit yfinance matplotlib openpyxl
```

### Running the App
To start the application, open your terminal, navigate to the project folder, and run:
```bash
streamlit run your_file_name.py
```

### How to Use the Dashboard
Once the app launches in your browser, you will see a sidebar menu on the left with the following options:

* **➕ Adaugă investiție (Add Investment):** * **Important:** In the "Numele activului" (Asset Name) field, you **must use the exact stock ticker symbol**, not the full company name (e.g., type `NFLX` for Netflix, `GOOG` for Google).
  * Enter the quantity and your purchase price.
  * The app will automatically fetch and display the live price in RON, USD, and EUR. Click the "Adaugă" button to save it to your portfolio.

* **🗑️ Șterge investiție (Delete Investment):**
  * Select an existing asset from your portfolio using the dropdown menu and click "Sterge" to remove it.

* **📊 Vizualizează portofoliu (View Portfolio):**
  * Displays a detailed table of your current holdings, including purchase price, live price, and total value.
  * You can switch the display currency between RON, USD, and EUR using the dropdown menu.
  * Below the table, you'll find the **Total Portfolio Value** and your **Total Profit** (highlighted in green for positive returns and red for losses).
  * Includes a dynamic bar chart visualizing the value distribution of your assets.

* **📥 Exportă în Excel (Export to Excel):**
  * Click the download button to instantly generate and download an `.xlsx` file containing a cleanly formatted report of your entire portfolio.
