# Risk-Budgeting-Performance-Analytics


# QuantRisk: Systematic Risk Budgeting & Multi-Pair Performance Analytics
Gogglesheet:
https://docs.google.com/spreadsheets/d/1CRw9NT8JfIxb5GrdOW81dGCmoDWeFYDWB6Kq-NK-BZY/edit?gid=1476966166#gid=1476966166

![Quant Finance](https://img.shields.io/badge/Domain-Quantitative%20Finance-blue)
![Python](https://img.shields.io/badge/Language-Python-green)
![Risk Management](https://img.shields.io/badge/Focus-Risk%20Budgeting-red)
![Sharpe Ratio](https://img.shields.io/badge/Sharpe-4.12-gold)

## 📌 Project Overview
This project presents a comprehensive **Risk Budgeting** framework for a multi-pair systematic trading strategy operating on a 15-minute timeframe. Based on 14 months of historical backtesting (642 trades) and 6 weeks of live execution validation, the analysis focuses on capital allocation efficiency and statistical robustness.

The core objective is to move beyond simple "return chasing" and establish a professional **Capital at Risk** model that ensures long-term survival and scalability.

## 📊 Key Performance Metrics (14-Month Dataset)
The strategy demonstrates institutional-grade performance with high consistency:

| Metric | Value |
| :--- | :--- |
| **Total Net Return** | 177 Units |
| **Sharpe Ratio** | **4.12** |
| **Profit Factor** | 1.55 |
| **Weekly Win Rate** | **82% (50/61 weeks)** |
| **Max Weekly Drawdown** | -6.62 Units |
| **Backtest/Live Correlation** | **~99%** |

## 🛡️ The Risk Budgeting Model
Instead of traditional position sizing, this framework utilizes **Drawdown-based Risk Budgeting**. We allocate a specific "Risk Capital" to the strategy, defining a hard stop-out level to protect the master portfolio.

* **Allocated Risk Budget:** 15 Units (Maximum loss threshold)
* **Expected Monthly Return:** 12.5 Units
* **Operational Warning Level:** -11 Units (Trigger for regime analysis)
* **System Termination Level:** -15 Units (Full strategy review/halt)

## 📈 Backtest vs. Live Validation
A critical highlight of this project is the near-perfect alignment between the backtest mean and real-world execution, proving the model's resilience against overfitting.

* **Backtest Weekly Mean:** 3.02 Units
* **Live (6-Week) Weekly Mean:** 3.00 Units

## 🔍 Quantitative Insights
* **Fat-Tail Dynamics:** The strategy benefits from volatility expansions. The average "best week" (+11.6) is ~2.9x larger than the average "worst week" (-4.0), providing a strong positive skew in the long run.
* **Monte Carlo Stress Test:** 10,000 iterations of return shuffling indicate a **Risk of Ruin (breaching the 15-unit budget) of <0.2%**.
* **Regime Robustness:** The 14-month data encompasses various market cycles, including high-volatility trends and low-volatility ranges.

## 📂 Repository Structure
* `data/`: Weekly performance logs (Backtest & Live).
* `scripts/`: Python analytics for Sharpe, Drawdown, and Monte Carlo simulations.
* `Risk_Budgeting_Model.xlsx`: Interactive Excel dashboard for capital allocation.

---
**Author:** [Yunus Bilgiç](https://github.com/yunusbilgic)  
*Kaggle Master | Quantitative Analyst*
