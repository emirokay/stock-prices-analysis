# BIST Banking Stock Performance — Which Turkish Bank Gave the Best Risk-Adjusted Returns?

Analysis of 5 Turkish banking stocks (Akbank, Garanti BBVA, İş Bankası, Yapı Kredi, Halkbank) vs the BIST 100 index, covering Jan 2021 – Jun 2026. Data sourced from Yahoo Finance via `yfinance`.

## TL;DR

Garanti BBVA wins by every measure — highest total return (1,606%), best Sharpe ratio (0.80), and a max drawdown (-38%) better than the sector average. Halkbank is the outlier: -54% max drawdown, Sharpe of 0.53, and weakest correlation to other banks (~0.60 vs 0.75+ for private banks). All five banks beat the BIST 100 (832% return).

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook stock_price_analysis.ipynb
```

Then click **Run All** in the notebook menu.

## Key Finding

Garanti BBVA delivered the best risk-adjusted returns over 5.5 years of Turkey's high-inflation era. The sector as a whole crushed the broad index, but individual risk profiles varied significantly — Halkbank's state ownership makes it a very different investment than the four private banks.

## Charts

- **Relative performance** — All banks indexed to 100, showing Garanti and Yapı Kredi pulling ahead in late 2023
- **Annual returns** — Grouped bar chart showing the monster 2023 vs the 2024 correction
- **Drawdown comparison** — 3×2 grid of drawdowns with max drawdown annotated for each bank + index
- **Correlation heatmap** — Daily return correlations showing the private bank cluster vs Halkbank

## Statistical Test

Pearson correlation between Garanti BBVA and BIST 100 daily returns: r = 0.654, p < 0.001. Garanti moves in the same direction as the index but with amplified swings.

## Built With

pandas, numpy, matplotlib, seaborn, scipy, yfinance

## License

MIT
