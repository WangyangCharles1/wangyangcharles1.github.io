---
title: 'Research Series: Machine-Learned Liquidity Measures and Causal Inference'
date: 2026-06-28
permalink: /posts/2026/06/series-ml-liquidity-measures/
tags:
  - Research Series
  - Machine Learning
  - Liquidity
  - Causal Inference
---

This four-paper series develops and applies machine-learned measures of market liquidity across diverse asset classes and market structures, while establishing rigorous methods for causal inference with generated measures.

The series progresses from measurement to application to methodology:

1. **[Does Market Opening Improve True Liquidity?](/posts/2026/06/market-opening-liquidity/)** — Deploys a GBM-based liquidity measure (R-squared = 0.59) across 20 emerging markets and 36,500 market-days. Market opening reduces effective spreads by 8.60 bps (-23.3%), with 87.2% of the improvement driven by adverse-selection compression.

2. **[Dealer Constraints and Hidden Liquidity Deterioration](/posts/2026/06/dealer-constraints-hidden-liquidity/)** — Develops an ML measure from TRACE data achieving R-squared of 0.84, dramatically outperforming Roll (0.13) and Amihud (0.03). Finds that 89% of crisis illiquidity is funding/inventory driven, with SMCCF eligibility providing 27 bps of relief.

3. **[Tokenized but Illiquid?](/posts/2026/06/tokenized-illiquid/)** — Measures trading costs across 153 RWA protocols ($26.6bn TVL), finding a 23x cost gap (131 bps vs 5.7 bps). Decomposes costs into fragmentation (57%), oracle-lag (27%), and residual (17%).

4. **[When Liquidity Measures Become Treatments](/posts/2026/06/measures-as-treatments/)** — Identifies four pathologies (measurement error, generated-regressor failure, post-treatment leakage, look-ahead bias) in causal inference with ML measures and validates corrections including pre-treatment training, cross-fitting, SIMEX, and DML.

Together, these papers establish that **machine-learned liquidity measures are powerful but require careful handling**—both in construction and in subsequent causal analysis.
