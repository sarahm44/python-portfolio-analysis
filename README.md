# Python Portfolio Analysis
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/portfolio-analysis.png)

## Overview 

I was tasked with analysing a number of financial portfolios across the areas of:
* volatility
* returns
* risk
* Sharpe ratios

I created an [analysis notebook](https://github.com/sarahm44/unit-4-assignment/blob/main/whale_analysis.ipynb) that analyzes and visualizes the major metrics of the portfolios across all of these areas, and determines which portfolio outperformed the others. 

My data set included a number of different portfolios.

The three main tasks were to:
1. Read in and wrangle returns data
2. Determine success of each portfolio
3. Choose and evaluate a custom portfolio

## Data Preparation

For the data preparation I was required to do the following:

* Use Pandas to read each CSV file in as a DataFrame. 
* Detect and remove all null values. 
* Convert the S&P 500 closing prices to daily returns. 
* Join the Whale Returns, Algorithmic Returns, and the S&P 500 Returns into a single DataFrame with columns for each portfolio's individual returns. 

See the single DataFrame below:
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/data_prep.jpg)

## Quantitative Analysis
In this section, I was required to calculate and visualize performance and risk metrics for the portfolios.

### Performance Analysis
#### Daily Returns
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/daily_returns.png)

#### Cumulative Returns
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/cumulative_returns.png)

### Risk Analysis
#### Box Plot
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/box_plot.png)

#### Standard Deviation
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/standard_deviation.png)

#### Portfolios Riskier than S&P TSX 60
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/riskier_than_sp.png)

#### Annualised Standard Deviation
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/annualised_std.png)

#### Rolling Standard Deviation with a 21-day Window
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/rolling_std.png)

#### Calculate Correlation
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/correlation.png)

#### Plot Correlation
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/correlation_graph.png)

#### Beta
I was required to calculate and plot Beta for a chosen portfolio (algo 1) and the S&P 60 TSX.
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/beta.png)

## Sharpe Ratios
### Annualised Sharpe Ratios
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/annualised_sharpe_ratios.png)

### Sharpe Ratios Bar Plot
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/sharpe_graph.png)

### Determine whether the algorithmic strategies outperform both the market (S&P TSX 60) and the whales portfolios
I found as follows: 
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/algo_v_market.png)

## Custom Portfolio
### Data Preparation
I created a custom portfolio of [Cardano](https://github.com/sarahm44/unit-4-assignment/blob/main/ada_data.csv), [Bitcoin](https://github.com/sarahm44/unit-4-assignment/blob/main/btc_data.csv) and [Ethereum](https://github.com/sarahm44/unit-4-assignment/blob/main/eth_data.csv). 

I used the Google Finance function to choose a portfolio, then downloaded the data needed as CSV files.

In my notebook I read in the CSVs and joined them as a single DataFrame, as below:
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/my_portfolio_01.png)

I calculated the weighted returns for the portfolio assuming an equal number of shares for each stock:
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/my_portfolio_02.png)

Then I added these to my DataFrame containing all portfolios:
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/my_portfolio_03.png)

### Re-run the Analysis, Comparing My Portfolio

#### Annualised Standard Deviation
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/my_portfolio_04.png)

#### Rolling Standard Deviation with a 21-day Window
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/my_portfolio_05.png)

#### Calculate Correlation
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/my_portfolio_06.png)

#### Plot Correlation
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/my_portfolio_07.png)

#### Beta
I was required to calculate and plot 60-day Rolling Beta for My Portfolio compared to the S&P 60 TSX.
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/my_portfolio_08.png)

#### Annualised Sharpe Ratios
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/my_portfolio_09.png)

#### Sharpe Ratios Bar Plot
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/my_portfolio_10.png)

#### My Portfolio Compared to the Market

For my portfolio, I found as follows:
![""](https://github.com/sarahm44/unit-4-assignment/blob/main/Images/my_portfolio_11.png)


