S&P 500 Stock Performance Analytics Dashboard
A Comprehensive 5-Year Financial Analysis in Power BI 📊



📌 Project Overview

This project presents an interactive and fully dynamic Power BI dashboard built to analyze 5 years of historical stock performance for all companies currently listed in the S&P 500.

Using a dataset of 600,000+ rows, the report enables detailed exploration of price trends, ROI growth, sector-wide insights, and trading volume analysis from 2013 to 2018.

Author: Sarvesh Kumar Roy
Repository: https://github.com/roysarvesh/S-P-500-Stock-Performance-Analytics-Dashboard-using-Power-BI

🛠️ Tools & Technologies

Power BI Desktop – Dashboard creation

Power Query (M) – Data cleaning & transformations

DAX – Advanced ROI and time-intelligence measures

Dataset – Historical OHLC + Volume (CSV)

💡 Key Features
1. Individual Stock Deep-Dive

Real-time filtering for 505 unique tickers

KPI cards showing:

Latest Price

Total ROI %

52-Week High / Low

Line charts for daily price trends

2. Interactive Tooltips

Custom tooltip page showing daily High vs Low range

Auto-displayed on hover for improved user experience

3. Market Comparison View

Multi-line trend comparison across any selected companies

Ideal for sector benchmarking and cross-analysis

4. Trading Volume Analysis

Heatmaps to detect high-activity periods

Monthly/Yearly volume patterns

Identify hype cycles and market sentiment shifts

📈 DAX Measures Used
Latest Price
Latest Price :=
CALCULATE(
    SUM('Fact_Stocks'[Close ($)]),
    LASTDATE('Fact_Stocks'[Date])
)

Total ROI %

Percentage growth from the stock’s first recorded date to the latest date.

52-Week High / Low

Rolling window calculations for the past 365 days.

🚀 How to Use

Clone the repository:
https://github.com/roysarvesh/S-P-500-Stock-Performance-Analytics-Dashboard-using-Power-BI

Open the .pbix file using Power BI Desktop.

If the data source path breaks:

Go to Transform Data → Data Source Settings → Change Source

Update the path to all_stocks_5yr.csv included in the repo.
