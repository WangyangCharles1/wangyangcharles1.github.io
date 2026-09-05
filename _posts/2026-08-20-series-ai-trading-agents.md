---
title: 'Research Series: AI/LLM Trading Agents and Market Microstructure'
date: 2026-08-20
permalink: /posts/2026/08/series-ai-trading-agents/
tags:
  - Research Series
  - AI
  - LLM
  - Market Microstructure
---

This four-paper series investigates how AI and large language model trading agents interact with—and potentially destabilize—modern market microstructure. As autonomous AI agents assume growing roles in price discovery, liquidity provision, and order routing, we must understand not only their individual performance but also their emergent collective behavior.

The series covers four interrelated dimensions:

1. **[Reasoning Is Latency](/posts/2026/08/reasoning-is-latency/)** — Examines the fundamental tradeoff between LLM reasoning depth and execution quality. We find that fill rates decline monotonically with inference latency (Spearman rho = -0.94), implying that optimal reasoning depth must be calibrated to signal decay rates.

2. **[Tacit Collusion without Communication?](/posts/2026/08/tacit-collusion-ai-market-makers/)** — Shows that Q-learning market makers independently learn to sustain supra-competitive spreads through punishment strategies, creating algorithmic tacit collusion that evades current regulatory frameworks.

3. **[AI-Powered Smart Order Routing](/posts/2026/08/ai-smart-order-routing/)** — Demonstrates that AI routing reduces costs by 26–43 bps in normal times but creates dangerous crowding externalities during stress, with venue concentration rising 40–65%.

4. **[Do LLM Trading Agents Create Informational Herding?](/posts/2026/08/llm-trading-herding/)** — Documents that shared model architectures produce correlated order flow (0.55 to 0.83), triggering flash crashes from collective misinterpretation that prompt diversification can partially mitigate.

Together, these papers argue that **AI trading agents require a new regulatory paradigm**—one that accounts for reasoning latency, emergent coordination, and cognitive homogeneity as sources of systemic risk.
