# 📈 NVIDIA (NVDA) Financial and Comparative Stock Analysis

This repository contains a financial analysis of **NVIDIA (NVDA)**, focusing on its stock price performance, valuation metrics (P/E ratio), and market capitalization compared to major benchmarks and peers. The analysis uses historical stock data, S\&P 500 company information, and current financial metrics for a comprehensive view.

The core of this project is a Jupyter Notebook that generates both static and interactive visualizations to explore NVDA's journey from a high-growth tech stock to a major market player.

## 🚀 Key Features

* **Comparative Stock Performance:** Analyze NVDA's price performance since 2020 against the **S\&P 500 (SPY)** and the **Technology Select Sector SPDR Fund (XLK)**, with an emphasis on the COVID-19 era.
* **Sector and Peer Valuation:** Compare NVDA's trailing and forward P/E ratios and market capitalization with tech giants **Microsoft (MSFT)** and **Google (GOOG)**.
* **Historical Context:** Visualize NVDA's date of entry into the S\&P 500 compared to the historical entries of all other companies in the index.
* **Interactive Dashboard:** The notebook integrates the `panel` library to create an **interactive dashboard**, allowing users to dynamically adjust parameters like time-frame and histogram bins for a personalized view of the data.

## 📊 Sample Visualizations

The analysis includes charts like:

### NVDA Price Performance vs. Market & Sector (2020-Present)

Comparing NVDA's growth against SPY and XLK, scaled to the same starting point to show relative returns.

### Comparative P/E Ratios

A comparison of NVDA's historical P/E ratio trends against MSFT and GOOG.

### Current Valuation Metrics

Side-by-side comparison of key financial metrics (Market Cap, Current Price, P/E) for NVDA, MSFT, and GOOG.

## 🛠️ Prerequisites

To run the analysis notebook, you will need the following Python libraries installed:

* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `param`
* `panel`
* `hvplot`
* `holoviews`
* `altair`
* `plotly`
* `json`

You can install the necessary packages using `pip`:

```bash
pip install pandas numpy matplotlib seaborn param panel hvplot holoviews altair plotly
````

## 📂 Data

The analysis depends on several local `.csv` and `.json` files, which are assumed to be in the same directory as the notebook. These files contain:

  * **PE Ratio Data:** `NVDA PE Ratio Historical Data.csv`, `MSFT PE Ratio Historical Data.csv`, `GOOG PE Ratio Historical Data.csv`
  * **Price Data:** `NVDA.csv`, `SPY.csv`, `XLK.csv`, `MSFT.csv`
  * **S\&P 500 Information:** `SP500.csv`
  * **Financial Snapshots (from yfinance):** `NVDA.json`, `MSFT.json`, `GOOG.json`

## ⚙️ How to Run the Analysis

1.  **Clone the Repository:**
    ```bash
    git clone https://github.com/thesjhu/nvda
    cd nvda
    ```
2.  **Ensure Data Files are Present:** Acquire the necessary financial data files and place them in the repository's root directory.
3.  **Open the Notebook:** Launch a Jupyter environment (e.g., JupyterLab or Jupyter Notebook).
4.  **Execute:** Open the `nvda.ipynb` file and run all cells.
5.  **Interactive App:** The final cell, which creates a `pn.Column` object, will launch an interactive dashboard in a new browser tab for exploring the results with widgets.

Feel free to contribute, suggest improvements, or fork this repository for your own financial analysis projects\!
