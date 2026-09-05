---
title: 'Reasoning Is Latency: LLM Trading Agents, Inference Time, and Execution Quality'
date: 2026-08-01
permalink: /posts/2026/08/reasoning-is-latency/
tags:
  - LLM
  - Trading Agents
  - Market Microstructure
  - Latency
---

In high-frequency and algorithmic trading, every millisecond of latency has a measurable cost. But what happens when the agent making trading decisions is a large language model engaged in multi-step reasoning? Our latest research uncovers a fundamental tension at the heart of AI-driven trading: **deeper reasoning improves decision quality but destroys execution quality**.

## The Latency-Reasoning Tradeoff

We document that fill rates decline monotonically with reasoning latency. Across **36,000 agent-event observations** spanning **8 reasoning depth levels** and **9 signal decay regimes**, the Spearman rank correlation is a striking **rho = -0.94**. In other words, the more an LLM "thinks," the less likely it is to execute its intended trade at the desired price.

This is not merely a technological limitation—it is a structural feature of markets where information has a half-life. A trading signal that decays within 500ms is nearly worthless by the time a chain-of-thought agent completes a five-step reasoning process.

## Sprinters vs. Marathoners

We propose a taxonomy of LLM trading agents along a spectrum from **"sprinters"** (shallow reasoning, fast execution) to **"marathoners"** (deep reasoning, slow execution). Sprinters excel in environments with rapid signal decay—news-driven momentum, earnings surprises, or order-flow imbalances. Marathoners thrive when signals are slow-moving—macro regime shifts, credit cycle analysis, or structural corporate actions.

The critical insight is that the **optimal reasoning depth is inversely proportional to the signal decay rate**. There is no universally optimal agent configuration; the right depth depends on the informational environment.

## Policy Implications

Our findings carry direct implications for best execution analysis under SEC Rule 605 and MiFID II RTS 28. Regulators and compliance teams should treat **reasoning latency as a component of transaction cost analysis**, alongside traditional factors like price improvement and execution speed. An agent that reasons deeply but misses its fill may violate best execution obligations just as surely as one that routes to an inferior venue.

The message for practitioners is clear: when deploying LLM trading agents, calibrate reasoning depth to signal half-life—and measure the cost of thinking.
