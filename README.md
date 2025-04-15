# Investment-Portfolio-Optimization

**Introduction**
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
The goal of this project is to optimize an investment portfolio using predictive analytics and optimization algorithms. By leveraging historical stock data, financial ratios, and other key metrics, we identify the best stock to invest in. This optimization process is carried out using two machine learning algorithms: K-Means clustering and Hill Climbing. The selected stock is then evaluated based on multiple financial criteria to make data-driven investment decisions.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Representative Data**

The dataset used in this project includes stock data from 15 prominent companies listed in the Nifty50 index. The companies analyzed are:
ADANIENT, ADANIPORTS, APOLLOHOSP, ASIANPAINT, AXISBANK, BAJAJ-AUTO, BAJFINANCE, BAJAJFINSV, BEL, BHARTIARTL, CIPLA,COALINDIA, DRREDDY

The key metrics used for portfolio optimization are:
1. PE Ratios (Price to Earnings Ratio)
2. Debt to Equity Ratio (DER)
3. Sales in Crore (2023 and 2024)
4. Simple Moving Average (SMA)

Additionally, live stock data is integrated using Zerodha Kite and Google Finance, providing tick-by-tick market data for real-time analysis during market hours.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Executive Driven Questions**
1. Which stock has the best potential for investment based on financial metrics?
2. How can we optimize a stock portfolio to maximize returns using historical data and financial ratios?
3. Can machine learning techniques like K-Means and Hill Climbing improve decision-making in investment?
4. Which stock among the selected Nifty50 companies aligns best with our investment criteria for 2024?

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Analytical Framework**
1. K-Means Clustering: This algorithm is used to group stocks based on their financial similarities. The clusters are used to understand the general performance and trends of similar stocks within the Nifty50 index.

2. Hill Climbing Algorithm: This optimization algorithm is used to fine-tune the stock selection. Starting with an initial stock, the algorithm iteratively moves to the next best stock based on an evaluation score that considers PE Ratios, DER, Sales in Crore, and SMA.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Data Best Practices**
1. Data Cleaning: All stock data and financial metrics were cleaned for missing or erroneous values before analysis.
2. Normalization: Financial metrics such as PE Ratios, DER, and SMA were normalized to ensure that they contribute equally to the optimization process.
3. Live Data Integration: Using APIs like Zerodha Kite and Google Finance, the portfolio's performance is tracked in real time, with OHLC (Open, High, Low, Close) data being fed into the model for up-to-date predictions and decisions.
4. Historical Data Validation: Data was validated against historical performance to test the effectiveness of the optimization algorithms.
