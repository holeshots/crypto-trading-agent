---
Title: Trading Costs and Slippage
Category: fundamentals
Status: NEEDS_REVIEW
Evidence Quality: MODERATE
Last Updated: 2026-09-09
Related Files: [order-books-and-price-formation.md, amm-and-dex-mechanics.md, trading-venues-and-fragmentation.md]
---

# Trading Costs and Slippage

## Summary

Cost measurement requires a named benchmark, units, side, size and time. Report explicit charges separately from price differences; otherwise spread and impact may be counted twice.

## Why It Exists

THEORETICAL EXPLANATION: execution consumes liquidity and takes time. An intended price and realized price can differ even when a direction hypothesis was reasonable. Trading economics must use actual fills and all applicable charges.

## How It Works

FACT, Coinbase rules: maker/taker fees can differ, a single order can contain portions of both, and rates depend on applicable schedules. Do not equate “limit” with “maker,” or hardcode an illustrative fee as current. [S001](https://www.coinbase.com/legal/trading_rules)

Research accounting convention for a completed, unlevered, same-quantity spot round trip, all terms in one quote unit:

`net PnL = q*(exit fill price - entry fill price) - explicit charges`.

For multiple fills, use quantity-weighted entry/exit prices. This is not a derivative or inverse-contract PnL formula. If using actual fills, their spread crossing and impact are already embedded. Add only charges not included in those prices. Borrowing and funding require separate treatment in later batches.

Define one-way signed execution shortfall in quote units as `side*q*(fill-reference)`, where side is +1 for a buy and -1 for a sell. State whether reference is a decision midpoint, arrival midpoint or executable quote. Negative shortfall is improvement. This definition measures outcomes, not the causal split between own impact, market movement and adverse selection.

Synthetic example: buy 2 units at 102, sell 2 at 104, and pay 1 quote unit in total charges. Net is `2*(104-102)-1=3`. These invented numbers illustrate accounting only; they are not performance data.

## Bullish Interpretation

Lower measured friction does not itself support a long position. A favorable price forecast still needs an independently established edge after costs.

## Bearish Interpretation

The same applies to short interpretations; this spot accounting example is not a short-borrow model.

## Market Conditions

Relevant in every regime, especially when expected price movement is small compared with round-trip friction.

## Timeframes

Every holding period. Shorter intervals do not justify omitting latency; longer intervals do not justify omitting exit costs.

## Confirmations

RESEARCH PROPOSAL: reconcile fill prices, sizes, timestamps, fee currency and conversion method. Record both the chosen reference and actual fill, not just a chart close.

## Invalidation

Unknown benchmark, missing fills, inconsistent fee units or unrecorded charges make a net-outcome claim incomplete.

## Strengths

Provides an auditable identity without assuming a strategy's success rate or optimal settings.

## Weaknesses

An accounting identity does not estimate fill probability, market impact causality or the cost of an unfilled order.

## Common Failure Modes

Subtracting spread twice; using fee tiers unavailable to the account; comparing a mid-price signal with frictionless fills; treating slippage tolerance as either a fee or guaranteed execution.

## Relationship to Other Concepts

Read [order books](order-books-and-price-formation.md) for benchmark prices, [AMMs](amm-and-dex-mechanics.md) for size-dependent swaps, and [venue fragmentation](trading-venues-and-fragmentation.md) before comparing markets.

## Automation Potential

HIGH for later accounting with complete records; uncertain cost forecasts require empirical evaluation. None has been performed.

## Evidence Quality

MODERATE overall: official documentation supports fee mechanics. EMPIRICAL FINDING: Adams et al.'s abstract reports that cost composition varied by trade size in two studied Uniswap pools; gas mattered more for small swaps, impact and slippage for larger swaps. This is external, sample-specific evidence, reviewed at abstract level only—not an independently replicated result. [S006](https://arxiv.org/abs/2309.13648)

## Sources

S001, S004, S005, S006: see the [source register](../../research/sources/market-mechanics-sources.md).

## Research Notes

CONFLICT C003, NEEDS_REVIEW:

- Interpretation A: Uniswap's swaps guide describes slippage as pending-transaction movement beyond price impact. [S004](https://developers.uniswap.org/docs/get-started/concepts/traders/swaps)
- Interpretation B: its glossary allows slippage to include price impact. [S005](https://developers.uniswap.org/docs/get-started/concepts/glossary)
- Shared assumption: an expectation is compared with execution. Difference: which expectation and which components it includes. Likely reason: benchmark conventions. Preserve both definitions; later datasets must document their calculation and reconcile quote/fill examples before combining measures.

Counterevidence to “DEX swaps are costless” or “a fixed basis-point estimate fits all sizes”: S006's reported cost heterogeneity. It does not refute or validate any trading strategy.

HYPOTHESIS H002: observed depth and quote age may explain execution shortfall better than candle volume alone. Future evaluation must separate size, venue, latency and regime; test across held-out periods and include failed/unfilled orders. No parameters are optimal or selected here.

[Back to knowledge index](../INDEX.md)
