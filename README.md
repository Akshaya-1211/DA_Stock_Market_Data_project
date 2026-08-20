# 📈 Stock Market Data Analysis & Visualization

## 📌 Project Overview

This project focuses on extracting, cleaning, analyzing, and visualizing stock market data using Python.

The analysis covers **Tesla (TSLA)** and **GameStop (GME)** by combining historical stock-price data with quarterly company revenue data. The project demonstrates how financial data can be collected from different sources and transformed into meaningful visualizations.

## 🎯 Objectives

* Extract historical stock data using `yfinance`
* Collect quarterly revenue data through web scraping
* Clean and prepare financial datasets using Pandas
* Create interactive stock-price and revenue visualizations
* Compare historical stock performance with company revenue trends

## 🏢 Companies Analyzed

* **Tesla (TSLA)**
* **GameStop (GME)**

## 🛠️ Technologies & Libraries

* **Python**
* **Pandas** — data manipulation and cleaning
* **yfinance** — historical stock data extraction
* **Requests** — retrieving webpage data
* **BeautifulSoup** — web scraping and HTML parsing
* **Plotly** — interactive data visualization

## 🔍 Project Workflow

### 1. Extract Stock Data

Historical stock information was collected using the `yfinance` library.

For Tesla:

```python
tesla = yf.Ticker("TSLA")
tesla_data = tesla.history(period="max")
```

For GameStop:

```python
gamestop = yf.Ticker("GME")
gme_data = gamestop.history(period="max")
```

The extracted data includes information such as:

* Date
* Open
* High
* Low
* Close
* Volume
* Dividends
* Stock Splits

## 2. Extract Revenue Data

Quarterly revenue data for Tesla and GameStop was collected from HTML webpages using `Requests` and `BeautifulSoup`.

The extracted revenue datasets were structured with:

* `Date`
* `Revenue`

Revenue values were cleaned by removing currency symbols, commas, null values, and empty records.

## 3. Data Cleaning & Preparation

The project uses Pandas to:

* Reset DataFrame indexes
* Remove missing values
* Remove empty revenue records
* Clean currency formatting
* Prepare stock and revenue data for visualization

## 4. Data Visualization

A reusable Plotly function was created to visualize both stock price and revenue.

Each visualization contains two sections:

**Historical Share Price**

Shows the historical closing stock price.

**Historical Revenue**

Shows the company's historical quarterly revenue.

The visualizations use a shared date axis to make it easier to compare stock-price movements with revenue trends.

## 📊 Key Analysis

The project provides a visual way to explore the relationship between:

**Company Revenue → Stock Price → Historical Market Performance**

Rather than analyzing stock prices alone, the project combines market data with company financial data to provide additional business context.

## 📂 Project Structure

```text
Stock-Market-Data-Analysis/
│
├── Stock_Market_Data_Analysis.ipynb
├── README.md
└── outputs/
    └── visualizations/
```

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd Stock-Market-Data-Analysis
```

### 2. Install the required libraries

```bash
pip install yfinance pandas requests beautifulsoup4 plotly
```

### 3. Open the Jupyter Notebook

```bash
jupyter notebook
```

Open the project notebook and run the cells sequentially.

## 💡 Skills Demonstrated

This project demonstrates practical experience with:

* Financial data analysis
* API-based data extraction
* Web scraping
* Data cleaning
* Pandas DataFrames
* Exploratory data analysis
* Interactive visualization
* Python programming

## 📌 Project Context

This project was completed as part of the **IBM Skills Network — Extracting and Visualizing Stock Data** assignment. The original assignment focuses on extracting Tesla and GameStop stock and revenue data and creating visualizations from the combined datasets.

## 👩‍💻 Author

**Akshaya**

Data Analytics | Python | SQL | Power BI | Data Visualization
