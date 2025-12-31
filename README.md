# FinancialModel
All syntax related to finance

# ETF assignment :

**Data Collection:**
Use Yahoo Finance to gather historical data for the ETF and its underlying assets. Use your discretion to pick a reasonable time frame.

**Python Implementation:**
Write a Python program that:

•	Reads the ETF's historical data from Yahoo Finance.

•	Based on the ETF's documentation and its investment strategy, simulate the ETF's returns over the given timeframe.

•	Generate the time series of the ETF's returns.

**Visualization:**

Generate plots that visualize the ETF's performance over time. Ensure your plots are clear, labeled, and easy to interpret.

**Analysis:**

Compare the replicated performance of the ETF with the actual performance data from Yahoo Finance.
Discuss any discrepancies or patterns you notice.

**Report Writing:**

Alongside your code and plots, prepare a brief report discussing your methodology, findings, and any challenges you encountered. This will help in understanding your thought process and the steps you took. 


# Final.ipnyb assignment :

-	Download the list of S&P500 firms from Wikipedia.

-	Download historical daily prices of the S&P500 firms from Yahoo! Finance.

-	Download all other data you need in later steps from appropriate sources. Such data include but may not be limited to

  o	Risk-free rates,
  
  o	S&P500 index prices and returns,

-	Convert all data to monthly frequency. You will only work with monthly data in this project.

-	Estimate the covariance matrix and expected returns of stocks every month. Your method of estimating the covariance matrices and expected returns must reflect two elements:

  o	The estimation methods we covered in class,
  
  o	An idea that you propose, based on your own thoughts or something you picked up outside the course material, to improve the estimation.

-	Form the tangency portfolio of S&P500 stocks using your estimates.

-	Calculate the Sharpe ratio for 

  o	Your tangency portfolio,
  
  o	An equally weighted portfolio of all S&P500 stocks,
  
  o	A tangency portfolio where all the covariances and expected returns are estimated using the Fama-French three factor model. (extra credit)

-	Write a report describing your results. In this report, you must include:

  o	A table of summary statistics for your monthly stock price data.
  
  o	A section explaining your method of estimating the covariance matrix and expected returns and arguing for its merit.
  
  o	A summary statistic table and a graph of the weights of stocks in your tangency portfolio; Feel free to select a few stocks for this step.
  
  o	A table and a figure describing monthly returns of your tangency portfolio.
  
  o	A table comparing the Sharpe ratios of the three portfolios above.
  
  o	A conclusion section explaining whether your proposed method works or not, and why.


# Cross-Sectional Prediction:

**Objective:** In this problem, you will predict future stock returns using past returns.

**Instructions:**

1. Download [the list of S&P500 stocks](https://en.wikipedia.org/wiki/List_of_S%26P_500_companies) from Wikipedia.

2. Download daily historical stock prices for S&P500 stocks.

3. Calculate the return and forward return for every stock/day.

4. For every stock/day, calcualte the return over prior five trading days (past week return).

5. Sort stocks into 10 bins based on prior week returns.

6. For each bin, form a daily-rebalanced, equally-weighted portfolio and calculate its daily returns.

7. Calculate the average daily return for each portfolio.

8. Form a long-short portfolio of bins 1 and 10.

9. Formally test if the long-short portfolio has positive average returns. Is the average return statistically significant?


# Cross-Sectional Prediction with Financial Statements

**Objective:** In this problem, you will learn to use fiancial statements to predict stock returns.

**Instructions:**

1. Download [the list of S&P500 stocks](https://en.wikipedia.org/wiki/List_of_S%26P_500_companies) from Wikipedia.

2. Download daily historical stock prices for S&P500 stocks.

3. Keep the last observation for each stock/month.

4. Calculate monthly returns and forward returns.

5. Restrict the observations to the time period 2010/1 - 2022/12.

6. Read in the file "consolidated_quarterly_balance_sheets.csv". This file contains balance sheets filed to EDGAR.

7. Calculate the current ratio for each observation. The current ratio is defined as

$$
Current\ Ratio = \frac{Current\ Assets}{Current\ Liabilities}.
$$

A current ratio larger than one means the firm has enough liquid assets to cover its short term liabilities.

8. Merge the balance sheet data with the monthly stock prices.

9. Fill in the missing observations of the current ratio with its last known value for the same firm.

10. Every month, sort the stocks into five bins based on their current ratios. Form an equally-weighted portfolio for each bin.

11. Calculate summary statistics of returns for each portfolio.

12. Form a long-short portfolio based on current ratio and calculate its monthly returns.

13. Formally test if the long-short portfolio yilds positive returns on average.

For more information about current ratios, refer to [Investopedia](https://www.investopedia.com/terms/c/currentratio.asp). I have compiled the balance sheet data from [this Kaggle page](https://www.kaggle.com/datasets/finnhub/reported-financials).

# Loan Default rate Prediction Analysis

**1. Introduction:**

The aim of this project is to develop a loan default prediction model by analyzing historical data and identifying key factors that contribute to loan defaults. The model will enable lenders to assess the risk associated with potential borrowers and make more informed lending decisions.

**2. Objective:**

The primary objective of this project is to accurately predict loan defaults by analyzing various factors that influence borrower behavior. By understanding the types of defaults and reasons behind loan defaults, this project will provide valuable insights into risk management and help lenders minimize potential losses.

**3. Scope:**

The project will utilize historical loan data, including borrower information, loan characteristics, and repayment behavior, to build a predictive model. The analysis will focus on identifying patterns, trends, and risk factors associated with loan defaults. The project will also explore the impact of different loan types and borrower profiles on default rates.

**4. Methodology:**

The project will follow the following steps:

a. Data Collection

b. Data Preprocessing

c. Feature Engineering

d. Exploratory Data Analysis

e. Model Development

f. Model Evaluation and Optimization

g. Results and Recommendations

**5. Deliverables:**

The project will deliver the following:

- A comprehensive analysis of loan default trends, types, and reasons.
 
- A loan default prediction model with documented methodology and performance evaluation.
 
- Visualizations, reports, codes, and presentations summarizing the findings and recommendations for lenders.
