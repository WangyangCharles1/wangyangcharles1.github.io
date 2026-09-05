---
title: 'Does Market Opening Improve True Liquidity? Evidence from Machine-Learned Microstructure Measures'
date: 2026-06-01
permalink: /posts/2026/06/market-opening-liquidity/
tags:
  - Market Opening
  - Machine Learning
  - Liquidity
  - Emerging Markets
---

When a stock market opens, does liquidity genuinely improve—or do standard measures merely give that impression? Our research combines **machine-learned liquidity measures** with a staggered market-opening identification strategy to answer this question across **20 emerging markets** and **36,500 market-days**.

## Market Opening Reduces Effective Spreads

Using the **Callaway-Sant'Anna staggered difference-in-differences estimator**, we find that market opening reduces the effective spread by **8.60 basis points (-23.3%)**. This is a large and economically meaningful effect, suggesting that extending trading hours meaningfully improves liquidity in emerging markets.

But the composition of this improvement is where the story gets interesting. Decomposing the effective spread into its adverse-selection and realized components, we find that **87.2% of the improvement comes from adverse-selection compression**. In other words, market opening primarily reduces the information asymmetry cost, not the inventory or order-processing cost.

This makes intuitive sense: longer trading hours allow information to be incorporated more gradually, reducing the adverse-selection premium that market makers charge to protect themselves against informed traders.

## ML Measures Outperform Traditional Proxies

Our machine-learned liquidity measure, trained using **gradient-boosted machines (GBM) with R-squared of 0.59** against a benchmark of proprietary institutional transaction costs, substantially outperforms traditional proxies. The ML measure captures nonlinear interactions between order flow, volatility, and market structure that linear proxies miss.

A key methodological innovation is **cross-country transportability**: we train the model on US data (where ground-truth transaction cost data is available) and deploy it across 20 emerging markets. The ML measure maintains strong out-of-sample performance, validating its use as a portable liquidity surveillance tool.

## Why This Matters

Emerging market regulators considering extended trading hours now have rigorous evidence that market opening genuinely improves liquidity—primarily through the information channel. The ML measurement framework also provides a template for **real-time liquidity monitoring** across jurisdictions where traditional transaction cost data is unavailable.

Our results suggest that market microstructure reforms in emerging economies should prioritize mechanisms that reduce information asymmetry—extended hours, enhanced disclosure, and pre-trade transparency—over interventions focused solely on reducing explicit trading costs.
