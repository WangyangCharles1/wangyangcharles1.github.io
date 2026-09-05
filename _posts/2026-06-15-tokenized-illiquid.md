---
title: 'Tokenized but Illiquid? Measuring Market Quality in Real-World Asset Token Markets'
date: 2026-06-15
permalink: /posts/2026/06/tokenized-illiquid/
tags:
  - Tokenization
  - RWA
  - AMM
  - Uniswap
  - Market Quality
---

The tokenization of real-world assets (RWAs)—from Treasury bills to real estate to private credit—has been heralded as the next frontier in financial market infrastructure. But does tokenization actually improve market quality, or does it simply move illiquidity onto a blockchain? Our research provides the first systematic measurement of trading costs in RWA token markets.

## The 23x Cost Gap

We measure trading costs across **153 RWA protocols** with a combined **$26.6 billion in total value locked**, using **48,340 simulated swaps** to estimate effective spreads. The headline finding is stark: tokenized asset trading costs average **131 basis points**, compared to **5.7 basis points** for equivalent traditional instruments—a **23-fold gap**.

This is not a comparison of unlike assets. We match tokenized RWAs to their closest traditional counterparts and measure the incremental cost of trading the tokenized version. The gap persists after controlling for asset class, maturity, and credit quality.

## Decomposition: Where the Costs Come From

We decompose the 131 bps trading cost into three components:

- **57% pool-depth fragmentation**: Liquidity is scattered across dozens of AMM pools, DEX aggregators, and bridging routes. No single venue has sufficient depth to execute meaningful size without substantial slippage.
- **27% oracle-lag arbitrage**: Price feeds from oracles lag real-time market movements, creating systematic adverse selection against liquidity providers who must compensate for this informational disadvantage.
- **17% residual**: Gas costs, MEV extraction, and protocol fees.

## ML Market-Quality Index

We construct a **machine-learning market-quality index** that achieves **R-squared of 0.97** against observed swap costs. This composite measure integrates pool depth, oracle accuracy, trading volume, and protocol design features into a single score that predicts trading costs for any given RWA token.

## Event Studies: What Actually Helps?

We study three natural experiments where protocols implemented structural improvements:

- **Oracle upgrades** (switching to Chainlink high-frequency feeds): Trading costs fell **84%** on the oracle-lag component
- **Redemption easing** (reducing lock-up periods and fees): Trading costs fell **83%** on the fragmentation component

These event studies demonstrate that the cost gap is not inherent to tokenization—it is a product of immature market infrastructure. As protocols improve oracle integration and consolidate liquidity, the gap should narrow substantially.

The message for the RWA ecosystem: **tokenization is not enough**. Market quality requires deliberate infrastructure investment in oracles, pool consolidation, and redemption mechanisms.
