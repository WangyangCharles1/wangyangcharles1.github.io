---
title: 'Dealer Constraints and Hidden Liquidity Deterioration: A Machine-Learning Measure from TRACE'
date: 2026-06-08
permalink: /posts/2026/06/dealer-constraints-hidden-liquidity/
tags:
  - Corporate Bonds
  - TRACE
  - Machine Learning
  - Dealer Constraints
---

Corporate bond markets are opaque. Unlike equities, where order books are visible and transaction costs can be measured directly, corporate bonds trade over-the-counter through dealer intermediation. This opacity creates a fundamental measurement problem: **how do you monitor liquidity in a market where you cannot directly observe it?**

## A Machine-Learning Breakthrough

We develop a machine-learned liquidity measure from TRACE (Trade Reporting and Compliance Engine) data that achieves **R-squared of 0.84** against actual institutional transaction costs. The improvement over traditional proxies is dramatic: the **Roll measure achieves 0.13** and the **Amihud measure achieves 0.03** on the same benchmark.

The ML model captures complex, nonlinear patterns in TRACE data that linear proxies cannot: the interaction between trade size and frequency, the information content of dealer-to-dealer versus customer-to-dealer trades, and the dynamics of price impact across the liquidity spectrum.

## The Sparsity Advantage

The ML measure's advantage **widens with data sparsity**. For frequently traded investment-grade bonds, traditional proxies perform adequately. But for the long tail of less liquid bonds—the ones most vulnerable during stress—the ML measure provides dramatically better signal. This is precisely where accurate liquidity measurement matters most for surveillance and risk management.

## Identifying the Binding Constraint

We decompose illiquidity into funding and inventory channels using the **SMCCF (Secondary Market Corporate Credit Facility) eligibility** as a natural experiment. When the Fed's SMCCF made certain bonds eligible for purchase, it provided exogenous funding relief to dealers holding those bonds.

The results are clear: **89% of crisis-period illiquidity** in corporate bonds is attributable to the funding/inventory channel. Bonds that became SMCCF-eligible experienced **27 basis points of liquidity relief** on funding-related costs alone, with minimal change in information-related costs.

## Policy Implications

Our findings support the deployment of **ML-based liquidity surveillance systems** for corporate bond markets. Regulators currently rely on coarse proxies that miss the majority of liquidity variation. An ML-based system could provide real-time, bond-level liquidity monitoring—detecting deterioration early enough for preemptive intervention rather than post-crisis autopsy.

The SMCCF evidence also suggests that **central bank facilities targeting dealer funding** are highly effective at restoring corporate bond liquidity, providing a template for future crisis response tools.
