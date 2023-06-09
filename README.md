# Stock Market Portolio

(Work in Progress)
The code constructs an optimized portfolio based on historical stock data from the S&P 500 by fetching a list of the companies and extracting ticker symbols, and historical stock data from Yahoo Finance. Necessary libraries include yfinance, pandas, numpy, matplotlib, and PyPortfolioOpt.

The close prices are extracted from the downloaded stock data for each ticker symbol and using the PyPortfolioOpt library, the code calculates the expected returns (mu) and covariance matrix (S) of the stocks based on their historical adjusted close prices. 

Next, the code creates an instance of the EfficientFrontier class and optimizes the portfolio to maximize the Sharpe ratio, balancing risk and return. The resulting raw weights are cleaned up to remove negligible weights, and the cleaned weights for the optimized portfolio are displayed, indicating the proportion of each stock to be held for maximum Sharpe ratio. 

Using the PyPortfolioOpt library further, an instance of the CLA (Critical Line Algorithm) class is created and to help visualize the optimal portfolios offering the best risk-return trade-offs a plot the efficient frontier is displayed. 
