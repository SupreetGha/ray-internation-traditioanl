# 📊 Ray Dalio-Inspired Portfolio Diversification Analysis
### Quantitative Portfolio Comparison & Risk Assessment
A data-driven deep dive into the risk-return tradeoffs of diversified portfolios across market regimes.

## 📌 Project Overview

This project investigates the long-term performance of Ray Dalio's risk-parity-inspired diversification strategy and compares it with two commonly adopted investment approaches:
1. A traditional 60% stock / 40% bond allocation
2. A globally diversified stock portfolio (36% US / 64% international)
Using historical data from 2000 to 2024, we simulate the portfolio growth of each strategy, analyze their risk-return profiles, and evaluate performance during major financial crises. This project aims to explore how diversification—especially across uncorrelated asset classes—impacts returns and volatility.

## Technologies Used
- Python 🐍
  -Pandas, NumPy for data wrangling
- Matplotlib for visualization
- yFinance for financial data extraction
- Jupyter Notebook for interactive development
## 📈 Analysis & Methodology
### 📂 Data Sourcing 
- Fetched historical price data (2000–2024) using yfinance for all portfolio components:

  - Stocks: VTI (US), VXUS (Intl)

  - Bonds: BND, TLT, LQD

  - Alternatives: GLD (Gold), DBC (Commodities), VNQ (Real Estate), PSP (Private Equity)

🧮 Portfolio Simulation
- Created an investment simulation starting with $1,000,000 across each strategy.

- Applied normalized prices and fixed weights to simulate portfolio value over time.

📉 Risk Metrics Calculated
- Annualized Return

- Annualized Volatility

- Sharpe Ratio (assumed risk-free rate = 0%)

- Maximum Drawdown

## 🧠 Key Metrics
<table>
  <thead>
    <tr>
      <th>Portfolio</th>
      <th>Annualized Return</th>
      <th>Volatility</th>
      <th>Sharpe Ratio</th>
      <th>Max Drawdown</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Traditional 60/40</td>
      <td>9.59%</td>
      <td>12.88%</td>
      <td>43.35%</td>
      <td>-27.39%</td>
    </tr>
    <tr>
      <td>36% US / 64% Intl</td>
      <td>8.16%</td>
      <td>17.55%</td>
      <td>23.68%</td>
      <td>-34.40%</td>
    </tr>
    <tr>
      <td>Ray Dalio Diversified</td>
      <td>5.59%</td>
      <td>10.24%</td>
      <td>15.53%</td>
      <td>-26.69%</td>
    </tr>
  </tbody>
</table>

## 🔥 Crisis Performance Snapshot


<table>
  <thead>
    <tr>
      <th>Crisis Period</th>
      <th>Ray Dalio Diversified</th>
      <th>Traditional 60/40</th>
      <th>36% US / 64% Intl</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>COVID Crash</td>
      <td>-14.61%</td>
      <td>-14.72%</td>
      <td>-24.97%</td>
    </tr>
    <tr>
      <td>2022 Inflation Shock</td>
      <td>-15.46%</td>
      <td>-17.03%</td>
      <td>-17.85%</td>
    </tr>
  </tbody>
</table>



## 📢 Results & Insights
- Analyzed distributions of all features via histograms to understand their spread and skewness.

- Identified top features influencing portfolio risk and performance using correlation and factor decomposition techniques.

- Developed portfolio construction logic inspired by Ray Dalio’s "All Weather" strategy.

- Compared long-term return paths and volatility profiles to quantify differences in portfolio behavior.

- Additional Accomplishments:

  - Visualized cumulative returns across all strategies from 2005 to 2024.

  - Highlighted maximum drawdowns using drawdown plots for each strategy.

  - Simulated performance across four major market crises, revealing stark differences in capital preservation.

  - Built functions to calculate and format annualized return, standard deviation, Sharpe ratio, and max drawdown for automated reporting.

  - Demonstrated how correlation among asset classes can be used to engineer lower-volatility portfolios.

  - Showed that the Ray Dalio Portfolio had the lowest drawdown (-26.7%) while maintaining a respectable Sharpe Ratio (0.55), making it an ideal candidate for risk-conscious, long-term investors.
