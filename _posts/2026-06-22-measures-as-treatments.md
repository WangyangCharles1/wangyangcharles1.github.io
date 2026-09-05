---
title: 'When Liquidity Measures Become Treatments: Causal Inference with Machine-Learned Market Quality'
date: 2026-06-22
permalink: /posts/2026/06/measures-as-treatments/
tags:
  - Causal Inference
  - Machine Learning
  - Methodology
  - DiD
---

Machine-learned liquidity measures are transforming empirical finance. But using a predicted measure as an outcome variable in causal analysis introduces subtle statistical pathologies that can invalidate standard inference. This paper provides the first systematic treatment of these problems—and their solutions.

## Four Pathologies

We identify and quantify **four distinct pathologies** that arise when ML-predicted liquidity measures are used as dependent variables or treatments in causal regressions:

1. **Classical measurement error**: Prediction noise attenuates estimated treatment effects toward zero, biasing results against finding significant effects.

2. **Generated-regressor failure**: Standard errors computed as if the measure were observed (rather than predicted) **understate true uncertainty by 2–5x**, leading to massive over-rejection of the null hypothesis.

3. **Post-treatment leakage**: When the ML model is trained on data that includes post-treatment periods, the predicted measure absorbs part of the treatment effect. This causes **90% attenuation**—in our simulations, a true treatment effect of **tau = -0.40** is estimated as a statistically insignificant **-0.04**.

4. **Look-ahead bias**: When future information leaks into feature construction or model selection, the measure is contaminated by information that should not be available at the time of measurement.

## Monte Carlo Evidence

Our simulation study uses **2,000 replications across 6 different liquidity measures** to quantify the severity of each pathology. The results are sobering: naive application of standard causal inference methods to ML-predicted measures produces severely biased estimates and misleading confidence intervals in the majority of replications.

## Solutions

We propose and validate a toolkit of corrections:

- **Pre-treatment training**: Train the ML model exclusively on pre-treatment data to eliminate post-treatment leakage
- **Cross-fitting**: Use sample-splitting to reduce overfitting bias in the predicted measure
- **SIMEX (Simulation-Extrapolation)**: Correct for classical measurement error by simulating additional noise and extrapolating back to zero measurement error
- **Double/Debiased Machine Learning (DML)**: Combine cross-fitting with Neyman-orthogonal moment conditions to achieve root-N consistent estimates even with ML-generated measures

## Practical Guidance

The takeaway for applied researchers: **never naively regress an ML-predicted measure on a treatment variable and trust the standard errors**. The pathologies we document are not theoretical curiosities—they arise routinely in empirical work and can reverse the sign and significance of estimated effects. Our proposed corrections restore valid inference and should become standard practice in empirical market microstructure research.
