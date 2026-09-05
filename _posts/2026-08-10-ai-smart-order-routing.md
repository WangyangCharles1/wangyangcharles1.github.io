---
title: 'AI-Powered Smart Order Routing and the New Best Execution Problem'
date: 2026-08-10
permalink: /posts/2026/08/ai-smart-order-routing/
tags:
  - Smart Order Routing
  - AI
  - Best Execution
  - Systemic Risk
---

Smart order routing (SOR) has always been about finding the best venue. But when AI agents control routing decisions across fragmented markets, the definition of "best" becomes far more complex. Our research shows that AI-powered routing delivers superior execution in calm markets but introduces **systemic crowding risk** during stress.

## AI Routing Performance in Normal Times

Using a **multi-agent contextual bandit model** trained on order-book features, latency profiles, and historical fill rates, we find that AI routing achieves **26–43 basis points lower transaction costs** compared to static routing heuristics. The AI learns to exploit fleeting liquidity pockets across venues, dynamically rebalancing order flow to minimize market impact.

In benign conditions, this is unambiguously beneficial. Execution quality improves, spreads tighten, and the cost of trading falls.

## The Crowding Externality

The problem emerges during periods of market stress. When volatility spikes and liquidity retreats, AI routing agents **herd toward the same safe-haven venues**. We document that venue-level Herfindahl-Hirschman Index (HHI) rises **40–65%** during stress episodes—a massive concentration of order flow that overwhelms the very venues the AI selected for their liquidity.

This creates a **crowding externality**: each individual agent's optimal routing decision degrades execution quality for all others. The result is a coordination failure that amplifies market dislocations precisely when liquidity is most scarce.

## A Venue Congestion Surcharge

We propose a **venue congestion surcharge mechanism**—a Pigouvian correction that internalizes the crowding externality. By pricing venue congestion into routing decisions, the surcharge disperses order flow more efficiently and reduces the amplification of stress events. Simulations show the surcharge reduces peak HHI concentration by roughly 30% while preserving most of the cost savings AI routing provides.

## Regulatory Gaps

Current best execution frameworks are not designed for AI-driven crowding. **SEC Rule 605** requires broker-dealers to report execution quality by venue but does not address systemic concentration of order flow. **MiFID II's** best execution obligations focus on per-order optimization without considering aggregate routing patterns.

Our findings suggest regulators need a new systemic lens: monitoring **aggregate AI routing distributions** across venues as a macro-prudential indicator, much as banking regulators monitor systemic risk through interconnectedness metrics.
