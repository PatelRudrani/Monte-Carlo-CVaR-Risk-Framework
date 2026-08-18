# Monte-Carlo-CVaR-Risk-Framework
Monte Carlo simulation framework measuring corporate earnings downside risk using the Corporate Value-at-Risk (C-VaR) methodology. Models FX, commodity, and interest rate exposures across 24 years of bootstrapped historical data (1999 to 2023), achieving a 65% downside risk reduction and $1.2M earnings uplift through targeted hedging strategies.

## Methodology
Quarterly historical growth rates for three risk factors, the EUR/USD exchange rate, aluminum input prices, and short-term interest rates, are bootstrapped and compounded forward to generate a full distribution of pre-tax earnings outcomes. Risk is quantified using 95% Conditional Value-at-Risk (C-VaR), which measures the expected earnings shortfall in the worst 5% of simulated scenarios. The base case runs 4,000 scenarios; a robustness check scales this to 15,000 scenarios to confirm the results are stable and not driven by simulation noise.

## Key Findings
- Selective hedging achieved a 65% reduction in downside risk (C-VaR) relative to the unhedged base case, alongside a $1.2M improvement in expected earnings.
- Commodity price hedging (locking aluminum prices) produced the largest relative improvement in C-VaR among all hedging strategies tested, indicating input cost volatility is the dominant driver of downside earnings risk.
- FX hedging (locking the EUR/USD rate) also delivered a meaningful reduction in C-VaR, confirming exchange rate translation as a significant secondary risk driver.
- Results held stable when scenarios were scaled from 4,000 to 15,000, confirming the estimates reflect structural exposure rather than simulation noise.

## Recommendation
A targeted, exposure-driven hedging strategy is recommended over blanket hedging, prioritizing commodity price management first, with FX hedging applied where revenue translation risk is material and correlated with broader macroeconomic stress.

[View Full Report](https://github.com/PatelRudrani/Monte-Carlo-CVaR-Risk-Framework/blob/d97af7856c98d710bfd14646f5fe01b40c19b416/CVaR_Risk_Memo.md)
