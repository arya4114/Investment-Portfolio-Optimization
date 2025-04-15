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
![image](https://github.com/user-attachments/assets/8b5a298a-d300-4b1d-9ad2-8f146a782299)

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
**Results**
1. Stock Clusters by PE Ratios and Sales in crore(2024)
   
 ![image](https://github.com/user-attachments/assets/1791ae5d-f625-44a8-839a-95a5be9989a9)

Top Stocks in Cluster 0:

      TICKERS      Rank
    0    ADANIENT  2.394759
    2  APOLLOHOSP  2.270597
    6  BAJFINANCE  1.808150
    5  BAJAJ-AUTO  0.700868

Top Stocks in Cluster 1:

       TICKERS      Rank
    3   ASIANPAINT -0.502096
    1   ADANIPORTS -1.742887
    10       CIPLA -2.388609
    12     DRREDDY -2.687005
    8          BEL -3.966166

Top Stocks in Cluster 2:

       TICKERS      Rank
    7   BAJAJFINSV  3.464056
    9   BHARTIARTL  1.772468
    4     AXISBANK  0.177217
    11   COALINDIA -1.301352

2. Tickers VS SMAs
   
   ![image](https://github.com/user-attachments/assets/4b18a9c7-f11d-4b9f-bc69-0e691cd56fed)


4. Selected stock using Hill Climbing Algorithm
   Initial Stock:  ADANIPORTS,  Score:  11264.98
   
   Moved to Stock:  COALINDIA,  Score: 57123.55
   
   Moved to Stock:  BHARTIARTL,  Score: 61365.01

   Best Stock Selected:
   
| TICKERS   | PE Ratios | DER  | Sales in Crore (2024) | SMA    |
|-----------|-----------|------|------------------------|--------|
| BHARTIARTL | 42.79     | 1.25 | 151418.0               | 1621.8 |



------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Data Best Practices**
1. Data Cleaning: All stock data and financial metrics were cleaned for missing or erroneous values before analysis.
2. Normalization: Financial metrics such as PE Ratios, DER, and SMA were normalized to ensure that they contribute equally to the optimization process.
3. Live Data Integration: Using APIs like Zerodha Kite and Google Finance, the portfolio's performance is tracked in real time, with OHLC (Open, High, Low, Close) data being fed into the model for up-to-date predictions and decisions.
4. Historical Data Validation: Data was validated against historical performance to test the effectiveness of the optimization algorithms.
