# Portfolio Risk Analysis

This project performs a risk analysis on a stock portfolio, including calculations of annualized returns, volatility, Sharpe ratio, and various visualizations of portfolio performance over time.

## Prerequisites

Ensure you have the following Python packages installed: yfinance, pandas, numpy, matplotlib, and seaborn. These can be installed using pip if they are not already available.

## Usage

### Input Portfolio Data

Modify the portfolio DataFrame to include your own portfolio data, specifying stock tickers and the number of shares held.

### Time Horizon for Analysis

Set the start date and end date for the analysis period.

### Fetch Historical Price Data

The code uses yfinance to download the adjusted closing prices of the stocks in the portfolio.

### Calculate Portfolio Value and Returns

The portfolio value is calculated over time based on the number of shares held for each stock. Daily returns and annualized metrics such as volatility, return, and Sharpe ratio are then computed.

### Risk Metrics Calculation

- **Annualized Volatility**: This metric is calculated using the standard deviation of daily returns, scaled to an annual figure.
- **Annualized Return**: This metric is derived from the compounded daily returns, annualized over the number of days in the analysis period.
- **Sharpe Ratio**: The Sharpe ratio is calculated by subtracting the risk-free rate from the annualized return and dividing by the annualized volatility.

### Wealth Index and Drawdown Analysis

The wealth index represents the value of the portfolio over time, assuming an initial investment of 1000 units. Drawdown measures the percentage decline from the previous peaks in the wealth index.

### Visualization

Various visualizations are created using matplotlib and seaborn to show stock price trends, the wealth index, previous peaks, drawdowns, and correlations between the stocks in the portfolio.

### Output

The code prints the annualized volatility, annualized return, Sharpe ratio, and maximum drawdown of the portfolio. It also provides visualizations to better understand the portfolio's performance and risk over time.

## Example

The output includes:

- Annualized Volatility
- Annualized Return
- Sharpe Ratio
- Max Drawdown

For instance, you might see the following results:

Annualized Volatility: 0.2842
Annualized Return: 0.3774
Sharpe Ratio: 1.1346
Max Drawdown: -0.2475

Visualizations will display various aspects of the portfolio's performance over the specified period.
