# MEMORANDUM

*Corporate Value-at-Risk (C-VaR) Analysis: FX, Commodity, and Interest Rate Risk*

| | |
|---|---|
| **Author** | Rudrani Patel |
| **Re** | Downside Earnings Risk Assessment and Hedging Effectiveness, FY2024 Pre-Tax Earnings |

---

## Purpose

This memo summarizes the results of a Corporate Value-at-Risk (C-VaR) analysis conducted to quantify the downside earnings risk of a multinational firm exposed to EUR/USD exchange rate movements, aluminum input cost volatility, and short-term interest rate changes. The objective is to identify which risk factors contribute most to earnings downside and to evaluate whether targeted hedging can meaningfully reduce that exposure ahead of the fiscal year ending December 31, 2024.

## Methodology

Pre-tax earnings were modeled using Monte Carlo simulation built on bootstrapped historical quarterly growth rates for the three risk factors, drawn from 1999 through 2023. This non-parametric approach preserves the real-world skew and tail behavior of each series rather than imposing a normal distribution. Downside risk was measured using 95% Conditional Value-at-Risk (C-VaR), defined as the gap between mean simulated earnings (the benchmark) and average earnings in the worst 5% of outcomes. Five scenarios were run: an unhedged base case, a stress case with growth rate volatility increased 50% in absolute terms, an FX-hedged case with EUR/USD locked at its 12/31/2023 level, a commodity-hedged case with aluminum prices locked at the same date, and a robustness check that scaled the simulation from 4,000 to 15,000 paths.

## Key Findings

**Table 1. 95% Corporate C-VaR across the base case, stress case, hedged scenarios, and robustness check**

| Scenario | Simulations | Mean Earnings ($000s) | 95% C-VaR ($000s) | C-VaR (% of Benchmark) |
|---|---|---|---|---|
| Base Case (Unhedged) | 4,000 | 123,533.9 | 10,678.0 | 8.64% |
| Stress: +50% Growth Rate Volatility | 4,000 | 123,009.0 | 16,332.3 | 13.28% |
| FX Hedge (EUR/USD Locked) | 4,000 | 123,259.2 | 10,283.0 | 8.34% |
| Commodity Hedge (Aluminum Locked) | 4,000 | 124,758.9 | 3,578.3 | 2.87% |
| Robustness Check (Simulation Scale) | 15,000 | 123,064.2 | 10,412.3 | 8.46% |

Three findings stand out from the scenario comparison:

- **Downside risk is material even though expected earnings remain positive in every scenario.** In the unhedged base case, the worst 5% of outcomes fall roughly $10.7 million below benchmark earnings, equal to 8.64% of the benchmark, confirming that average performance alone understates the firm's true earnings risk.
- **Risk factors are not equally important.** Doubling down on volatility (the +50% stress case) pushes C-VaR up to 13.28% of benchmark, the worst result across all scenarios, showing that earnings risk is highly sensitive to the overall volatility regime rather than any single shock.
- **Hedging effectiveness differs sharply by risk factor.** Locking the EUR/USD rate reduces C-VaR by only 8.1% (from $11.2 million to $10.3 million), while locking aluminum prices reduces C-VaR by 68.0% (from $11.2 million to $3.6 million) and lifts mean earnings by roughly $1.1 million, indicating that commodity input cost volatility, not currency translation, is the dominant driver of the firm's tail risk.

### Hedging Effectiveness Comparison

**Table 2. Reduction in 95% C-VaR achieved by each single-factor hedge, measured against its paired unhedged simulation**

| Hedging Strategy | Unhedged C-VaR ($000s) | Hedged C-VaR ($000s) | Reduction in C-VaR |
|---|---|---|---|
| FX Hedge (EUR/USD Locked) | 11,186.9 | 10,283.0 | 904.0 (8.1%) |
| Commodity Hedge (Aluminum Locked) | 11,186.9 | 3,578.3 | 7,608.7 (68.0%) |

The robustness check further supports the reliability of these results. Scaling the simulation from 4,000 to 15,000 scenarios moves the benchmark and C-VaR by less than one percentage point (8.46% versus 9.05% on the paired 4,000-path run), and the relative ranking of scenarios by downside risk does not change. This indicates the conclusions reflect genuine structural exposure rather than simulation noise.

## Conclusions and Recommendations

A blanket hedging policy is not the most capital-efficient response to this risk profile. Because aluminum price volatility accounts for the largest share of downside risk, commodity hedging should be prioritized, particularly during periods of sharp upward price movement in input costs. FX hedging still provides a measurable, if smaller, improvement in downside protection and remains worth pursuing where currency translation risk is elevated or correlated with broader macro stress. In both cases, hedging should be evaluated on its ability to compress the left tail of the earnings distribution relative to the benchmark, not on its effect on expected earnings, since neither hedge materially shifts the mean outcome on its own.

Management should adopt the C-VaR framework as a recurring monitoring tool rather than a one time exercise, reassessing hedge ratios as commodity and currency market conditions evolve. The stress scenario result, a 57.2% increase in C-VaR when volatility rises 50% against its paired baseline, also argues for building contingency hedging capacity ahead of periods of anticipated macro stress rather than reacting after volatility has already increased.

### Limitations

The model assumes historical growth rate distributions remain representative of future conditions and does not capture implementation costs, liquidity constraints, or basis risk associated with actual hedging instruments. The scenarios also apply static, full period hedges; layered or dynamic hedging strategies were not tested and could alter the reported effectiveness. Results should be read as directional guidance for prioritizing risk management effort, not as a substitute for instrument level hedge design.
