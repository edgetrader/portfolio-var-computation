# Portfolio Risk Measurement of Crude Oil Futures

## Summary
This analysis demonstrates  how portfolio VaR can be calculated by historical simulation method. Each position in the portfolio is revalued based on historical scenarios on current market prices and rates. VaR is calculated on the simulated P&L of each position. Portfolio VaR is calculated on aggregated simulated P&L of all positions.

Historical simulation approach performs full revaluation of all positions on scenario rates. Consistent scenario rates generation process is of utmost importance here in order to maintain correlation across all factors/parameters passed in as inputs to valuation models.

Specifically, for future revaluation, prices of future contracts are not continuous. Number of days to maturity of each future contract reduces every other day. Scenario rates generation needs consistent continual time series. To convert them into consistent continual time series, we usually construct Nearbys or Constant Maturity price series for future prices.

Below demostrated the generation and creation of such time series and follow by Portfolio VaR calculaton using the Constant Maturity price series.

## Attachments
1. [Python Notebook](https://github.com/edgetrader/portfolio-var-computation/blob/master/notebook/var-computation-crude-oil.ipynb)
2. [PDF Document](https://github.com/edgetrader/portfolio-var-computation/blob/master/notebook/var-computation-crude-oil.pdf)
