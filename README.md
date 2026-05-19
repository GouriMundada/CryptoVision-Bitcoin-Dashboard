 ₿ CryptoVision — Bitcoin Market Analysis Dashboard
f2.png)

 Project Overview
A Live Bitcoin Market Analysis Dashboard built 
using Microsoft Power BI connected to Alpha Vantage 
API. The dashboard fetches real-time Bitcoin daily 
price data and displays interactive charts and 
KPI cards for financial market analysis.

 Tools Used
- Microsoft Power BI Desktop (Free)
- Alpha Vantage API (Free Tier)
- Power Query Editor — Data Cleaning
- DAX Formulas — Calculations

 Dashboard Features
- Live Bitcoin price data via Alpha Vantage API
- 5 KPI Cards — Avg Price, High, Low, Volume, PL%
- Shaded Area Chart — Price Trend Over Time
- Donut Chart — Gain vs Loss Days (56.78% Gain)
- Bar Chart — Daily Trading Volume
- Price Range Chart — High vs Low
- Interactive Date Range Slicer
- One-click Refresh for latest data
- Professional dark navy and golden theme

 API Details
- Provider: Alpha Vantage
- Function: DIGITAL_CURRENCY_DAILY
- Symbol: BTC (Bitcoin)
- Market: USD
- Website: https://www.alphavantage.co

How to Run This Project
1. Download Power BI Desktop (free) from microsoft.com
2. Register at alphavantage.co and get free API key
3. Open Livedataanalysis.pbix file
4. Replace API key in the Web connector URL
5. Click Refresh to fetch latest Bitcoin data
6. Use date slicer to filter any time period

 Data Cleaning Steps (Power Query)
1. Renamed table to StockData
2. Renamed all columns to readable names
3. Changed data types — Text to Decimal Number
4. Removed null and blank rows
5. Created GainLoss conditional column
6. Applied Close and Apply

 DAX Measures Created
- Avg Close Price = AVERAGE(StockData[Close Price])
- Max High Price = MAX(StockData[High Price])
- Min Low Price = MIN(StockData[Low Price])
- Total Volume = SUM(StockData[Volume])
- PL Percentage = DIVIDE((AVG Close - AVG Open), AVG Open, 0) * 100



