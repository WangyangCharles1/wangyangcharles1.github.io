---
title: 'Repo Netting, Central Clearing, and Dealer Balance Sheet Scarcity'
date: 2026-07-08
permalink: /posts/2026/07/repo-netting-central-clearing/
tags:
  - Repo
  - Central Clearing
  - SEC
  - Balance Sheet
  - CCP
---

In December 2023, the SEC finalized a landmark rule requiring **mandatory central clearing of US Treasury repos**. The stated goal: reduce systemic risk by netting offsetting positions and improving transparency. But does central clearing actually free up dealer balance sheet capacity, or does it merely shift the constraint?

## Evaluating the SEC Clearing Rule

We evaluate the SEC's mandatory clearing rule using a simulation of **48 dealers over 54 months**, modeling the transition from bilateral to centrally cleared repo. The results reveal two opposing forces:

**Netting benefit**: Gross balance sheet shrinks by **-20.79 units** as the central counterparty (CCP) nets offsetting repos and reverse repos. This is the primary mechanism through which clearing is supposed to improve market functioning—by reducing the balance sheet footprint of intermediation.

**Margin cost**: CCP margin requirements add **+1.34 units** of balance sheet consumption. While modest in normal times, this cost represents a new, rigid constraint that does not flex with market conditions.

## The Stress Erosion

The critical finding is that the **net benefit erodes during stress**. CCP margin models are inherently procyclical—initial margins rise with volatility, exactly when dealers need balance sheet relief most. During stress episodes, the margin cost can consume a substantial fraction of the netting benefit, reducing the effective balance sheet savings by 30–50%.

This procyclicality mirrors the liquidity multiplier dynamic documented in our companion paper on VaR risk limits. The CCP margin model becomes another channel through which volatility amplifies dealer constraints.

## Difference-in-Difference-in-Differences

Our identification strategy uses a **triple-difference (DDD) design**, exploiting variation in dealers' pre-rule clearing status, repo book composition, and time. This allows us to isolate the causal effect of mandatory clearing from concurrent changes in capital regulation and monetary policy.

## Recommendation: Countercyclical Margin Buffers

We propose that CCPs implement **countercyclical margin buffers**—requiring higher margin accumulation in calm periods to fund margin relief during stress. This mechanism, analogous to countercyclical capital buffers in banking regulation, would preserve the netting benefit when it matters most. The policy message is straightforward: central clearing is necessary but not sufficient. Without countercyclical margin design, the SEC's rule delivers less than promised when markets need it most.
