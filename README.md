# investment-portfolio

This Julia project aims to optimize an investment portfolio for a 5-year investment horizon. Real stock price data for 11 companies from the S&P 500 index was obtained from Yahoo Finance. Here's an overview of the project:

**Data Collection**
- Real stock prices were fetched from Yahoo Finance for the selected companies over the past 5 years.
- The dataset includes daily closing prices of the stocks.<br>

**Client's Investment Criteria**
- Expected rate of return for the 5-year horizon.
- Value at Risk (VAR) at 1% and 10% for the investment horizon.<br>

**Approach to Portfolio Selection**<br>
The project adopts a mean-variance optimization approach to select the optimal portfolio based on the client's risk-return preferences. Additionally, sensitivity analysis is conducted by splitting the historical data into two equal periods and performing the analysis on each period.

**Project Code Overview**
- **Data Preprocessing:** The fetched data is preprocessed to remove any unnecessary columns and to split it into two periods for sensitivity analysis.
- **Exploratory Data Analysis:** Visualizations are created to understand the dynamics of stock price changes and calculate the average returns and log returns.
- **Moving Averages and Trend Analysis:** Moving averages and trend lines are plotted to analyze the trend of stock prices over time.
- **Portfolio Optimization:** Two variants of portfolio optimization are performed:
1. Minimizing portfolio variance with a constraint on the minimum expected return.
2. Maximizing the portfolio's expected return while constraining the portfolio variance.
Risk Analysis: Value at Risk (VAR) at 1% and 10% levels is calculated to assess the downside risk of the portfolio.<br>
**Results and Conclusion**
- The optimized portfolios are presented along with their expected returns and standard deviations.
- Risk analysis results, including VAR at 1% and 10%, provide insights into the potential losses at different confidence levels.
- Sensitivity analysis helps in understanding how portfolio performance varies over different time periods.<br>

Overall, this project provides a comprehensive approach to optimizing investment portfolios based on historical stock price data, client preferences, and risk analysis metrics.
