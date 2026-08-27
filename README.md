# Sugar Market Statistical Arbitrage

Quantitative trading project applying statistical arbitrage techniques to the sugar commodity market (2019–2024).

Built a 14-asset universe (Sugar Futures SB=F, sector ETFs, sugar value-chain equities) and implemented two trading strategies:

- **Multivariate stat-arb**: market-neutral basket optimization under cointegration constraints (Gurobi quadratic programming)
- **Pairs trading**: mean-reversion strategy on the SB=F/MDLZ spread, selected via Engle-Granger and Johansen cointegration tests, with a rolling Z-score signal and volatility filter

Best strategy achieved a Sharpe ratio of 1.35, 83.8% win rate and -11.6% max drawdown over the backtest period.

**Tools**: Python, Gurobi, statsmodels, yfinance
