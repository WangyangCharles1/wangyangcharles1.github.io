---
title: 'Do LLM Trading Agents Create Informational Herding? Shared Models, Correlated Beliefs, and Market Fragility'
date: 2026-08-15
permalink: /posts/2026/08/llm-trading-herding/
tags:
  - LLM
  - Herding
  - Systemic Risk
  - Trading Agents
---

When thousands of trading agents share the same underlying language model, do they think alike—and trade alike? Our research demonstrates that **architectural homogeneity creates correlated order flow**, producing a form of informational herding that has no precedent in human trading and poses novel risks to market stability.

## Shared Models, Correlated Beliefs

We simulate populations of LLM-based trading agents varying in model architecture, training data, and prompt engineering. Across **6,000 parameter combinations** generating over **60 million market interactions**, we find that order flow correlation rises from **0.55 to 0.83** as model similarity increases. Agents built on the same base model, fine-tuned on similar data, and given comparable prompts develop nearly identical market views—even when processing different information.

This correlation is not driven by common information alone. It reflects **shared representational biases**: the same model encodes the same priors about how news maps to price movements, creating systematic agreement in interpretation that goes beyond what rational Bayesian updating would predict.

## Flash Crashes from Collective Misinterpretation

The most alarming finding is that correlated beliefs can trigger **flash crashes from collective misinterpretation**. When agents share a common model and encounter an ambiguous signal—say, a headline that the model associates with recession—they simultaneously revise positions in the same direction. The resulting order flow overwhelms market-making capacity, causing prices to overshoot before correcting.

We document multiple instances in simulation where correlated LLM agents produce drawdowns of 5–15% within seconds, followed by rapid reversals—the hallmark signature of herding-induced flash crashes.

## Prompt Diversification as a Mitigation

A practical mitigation emerges from our experiments: **prompt diversification reduces order flow correlation by 30–40%**. By varying prompt structures, few-shot examples, and reasoning frames across agents, practitioners can break the representational alignment that drives herding—without sacrificing individual agent performance.

This finding has implications for both **portfolio managers** deploying multiple AI agents and **regulators** concerned with systemic risk. Just as diversification across asset classes reduces portfolio risk, diversification across AI reasoning frameworks reduces systemic herding risk. The question for regulators is whether to mandate minimum diversity in AI trading model deployments—a form of **cognitive diversification requirement** for algorithmic trading firms.
