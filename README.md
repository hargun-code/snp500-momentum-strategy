# S&P 500 Momentum Strategy

A simple quantitative trading project built in Python to test whether stocks that have performed well recently continue to perform well in the following month.

## Idea

The strategy is based on momentum.

The basic idea is that stocks which have recently performed strongly may continue to perform strongly in the short term.

One possible reason is that investors react to existing price trends. When a stock rises, other investors may notice the movement and buy the stock because they expect the trend to continue.

This can create a positive feedback loop:

Price goes up → investors notice → more buying → price goes up further

The project tests whether this idea can be used to construct a simple trading strategy.

## How It Works

1. Get historical S&P 500 stock prices using yfinance.
2. Calculate the monthly return for each stock.
3. Rank the stocks based on their previous performance.
4. Select the top 10 performing stocks.
5. Calculate the return of those stocks in the following month.
6. Compare the strategy's return against the S&P 500.
7. Calculate the difference between the strategy and the benchmark.

## Results

For the period tested:

- Momentum Strategy: 9.35%
- S&P 500 Benchmark: 3.55%
- Excess Return: 5.80%

The strategy outperformed the benchmark by approximately 5.80 percentage points during the tested period.

This result is based on a limited test period and does not mean that the strategy will continue to outperform in the future.

## Technologies

- Python
- Pandas
- yfinance
- Jupyter Notebook
- Git
- GitHub

## What I Learned

Through this project I learned how to:

- Collect historical stock data
- Work with stock price data in Pandas
- Calculate percentage and monthly returns
- Rank stocks based on their performance
- Select stocks to form a simple portfolio
- Compare a strategy against a benchmark
- Calculate excess returns
- Build and test a simple quantitative trading strategy
- Use Git and GitHub to manage my project

## Limitations

This is a simple first version of the strategy.

It does not currently include:

- Transaction costs
- Slippage
- Risk metrics such as Sharpe ratio
- Maximum drawdown
- Long-term historical testing
- Different portfolio weightings (Assumes S&P 500 has equal index of all stocks within its index)

The strategy also uses a relatively limited testing period, so further testing is needed to determine whether the results are consistent.

## Future Improvements

The next step is to test the same momentum strategy using a different stock universe and compare the results.

Other potential improvements include:

- Testing a longer time period
- Testing different numbers of selected stocks
- Adding transaction costs
- Adding risk measurements
- Comparing cumulative returns
- Testing different momentum periods

## Disclaimer

This project is for educational purposes only and is not financial advice. Past performance does not guarantee future results.