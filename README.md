S&P 500 Stock Performance Analytics Dashboard
A Comprehensive 5-Year Financial Analysis in Power BI
📊 Project Overview
This project provides an interactive analysis of historical stock data for all companies currently in the S&P 500 index. Using a dataset of over 600,000 rows, the dashboard allows users to deep-dive into individual stock trends, compare sector-wide performance, and analyze trading volumes from 2013 to 2018.

🛠️ Tools & Technologies
Power BI Desktop: Data Visualization & Dashboarding.

Power Query (M): Data transformation, cleaning, and null handling.

DAX: Advanced measures for ROI calculation and time-intelligence.

Dataset: Historical stock data (CSV format) including Open, High, Low, Close, and Volume.

💡 Key Features
Individual Stock Deep-Dive: Real-time filtering for 505 unique tickers with automated "Latest Price" and "Total ROI %" cards.

Interactive Tooltips: Custom report-page tooltips that display the daily High vs. Low price range when hovering over the price line.

Market Comparison: A secondary analysis page for benchmarking multiple stocks against each other using multi-legend line charts.

Trading Volume Analysis: Heatmaps and bar charts to identify market liquidity and "hype" periods.

📈 DAX Measures Used
Latest Price: CALCULATE(SUM('Fact_Stocks'[Close ($)]), LASTDATE('Fact_Stocks'[Date]))

Total ROI %: Calculates percentage growth from the stock's first appearance in the dataset to the latest date.

52-Week High/Low: Dynamic measures that track the peak and trough within a rolling 365-day window.

🚀 How to Use
Clone this repository.

Open the .pbix file using Power BI Desktop.

If the data source is broken, update the file path in Transform Data > Data Source Settings to point to the all_stocks_5yr.csv included in the repo.
