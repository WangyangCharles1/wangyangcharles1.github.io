---
title: 'Trading Desk Risk Limits and the US Treasury Liquidity Multiplier'
date: 2026-07-01
permalink: /posts/2026/07/trading-desk-risk-limits/
tags:
  - Treasury
  - Dealer Constraints
  - VaR
  - Risk Limits
  - Liquidity
---

Why does US Treasury market liquidity evaporate during stress? The conventional answer points to regulatory capital constraints—post-crisis leverage ratio and SLR requirements that make balance sheet expensive. Our research identifies a different, more powerful channel: **dynamic VaR risk limits that tighten precisely when markets need liquidity most**.

## The Dynamic VaR Channel

We decompose dealer constraints into static capital requirements and dynamic risk limits, finding that the **dynamic VaR risk-limit channel dominates** in explaining Treasury market illiquidity. The key interaction term is **gamma = +0.31 bp per unit of volatility (sigma)**, meaning that each standard-deviation increase in market volatility tightens risk limits enough to widen bid-ask spreads by roughly a third of a basis point.

This creates what we term a **"liquidity multiplier"**: an amplification mechanism where volatility triggers risk-limit tightening, which reduces dealer market-making capacity, which increases volatility further—a self-reinforcing spiral.

## Data and Identification

Our empirical strategy combines the **Hu-Pan-Wang noise measure** (a high-frequency proxy for Treasury market illiquidity) with **NY Fed primary dealer position data** to isolate the risk-limit channel from confounding factors. By exploiting variation in dealers' internal risk-model calibrations, we separate the effect of dynamic limits from static capital constraints.

The results show that during stress episodes, dynamic risk limits explain a substantially larger share of liquidity deterioration than regulatory capital requirements alone. Dealers are not constrained because regulators force them to be—they constrain themselves because their internal risk models demand it.

## Policy Implications

The procyclicality of internal risk limits has received far less regulatory attention than capital requirements, yet our findings suggest it is the **binding constraint during crises**. We recommend that supervisors consider:

- **Countercyclical risk-limit adjustments** that allow temporary relaxation during stress
- **Standardized VaR floors** that prevent models from overreacting to volatility spikes
- **Stress-testing of risk-limit procyclicality** as part of supervisory review

The liquidity multiplier is a feature of internal risk management, not regulation. Addressing it requires looking beyond capital rules into the models dealers use to manage their own risk.
