---
Title: AMM and DEX Mechanics
Category: fundamentals
Status: RESEARCHED
Evidence Quality: STRONG
Last Updated: 2026-09-09
Related Files: [trading-venues-and-fragmentation.md, trading-costs-and-slippage.md]
---

# AMM and DEX Mechanics

## Summary

FACT: an automated market maker prices swaps against liquidity under protocol rules. Early Uniswap versions use a constant-product model; concentrated liquidity instead allocates liquidity within price ranges. These are specific designs, not definitions of every DEX. [S005](https://developers.uniswap.org/docs/get-started/concepts/glossary)

## Why It Exists

THEORETICAL EXPLANATION: a pricing rule allows a liquidity provider's committed assets to support exchanges without separately submitting a resting order at every possible price.

## How It Works

FACT: the simplified constant-product invariant is `x*y=k`. [S005](https://developers.uniswap.org/docs/get-started/concepts/glossary)

Mathematical derivation under explicit assumptions: ignore fees, transfers with special behavior and other transactions. Input `dx` of asset X changes reserves to `x+dx`; output of Y is `dy=y-k/(x+dx)=y*dx/(x+dx)`. Average Y received per X is `dy/dx`; the marginal pre-swap ratio is `y/x`. They differ for nonzero size. These expressions are not a universal router quote formula.

Synthetic example: `x=100`, `y=10,000`, `dx=10` gives `dy=909.0909...`, averaging `90.9091...` Y/X versus the initial ratio 100. This only demonstrates the invariant; it is neither an observed trade nor a return estimate.

FACT, Uniswap integrations: minimum output, maximum input and deadline constraints can bound acceptable execution. Protocol checks vary by version; v4 uses PoolManager and hooks. [S004](https://developers.uniswap.org/docs/get-started/concepts/traders/swaps)

## Bullish Interpretation

A swap changing a pool ratio upward for an asset is an observed local price change, not proof of continuing demand or a future long signal.

## Bearish Interpretation

The reverse change carries the same limitation. Distinguish a swap's mechanical effect from a forecast.

## Market Conditions

Relevant to pool-based trading. Total capital across a protocol is not a sufficient input to the constant-product illustration; use the actual route and applicable liquidity model.

## Timeframes

Quote time, transaction inclusion and settlement context matter more than candle choice for mechanics.

## Confirmations

RESEARCH PROPOSAL: reconcile token units, protocol version, route, pool state, specified protections and transaction result. Later analysis must identify whether a quote already includes own-trade impact.

## Invalidation

The simplified calculation is inapplicable if its fee-free, single-pool assumptions do not hold. A failed constraint invalidates the expected swap outcome; it does not establish a market reversal.

## Strengths

The model makes price-size dependence explicit and permits a transparent mathematical example.

## Weaknesses

The simple invariant cannot substitute for concentrated-liquidity, routed or hook-specific execution details.

## Common Failure Modes

Applying a v2 formula to every version; mixing token decimals; treating slippage tolerance as an expected cost; assuming a tighter tolerance guarantees execution.

## Relationship to Other Concepts

[Venues](trading-venues-and-fragmentation.md) separates market identity from mechanism. [Costs and slippage](trading-costs-and-slippage.md) records benchmark ambiguity and empirical cost limitations.

## Automation Potential

HIGH for a fully specified mathematical model; MEDIUM for later real-world reconciliation across routes and versions. No transaction-building functionality is implemented.

## Evidence Quality

STRONG for the bounded protocol concepts and algebra, UNKNOWN for strategy edge. A documented mechanism does not establish safety, best execution or profitability.

## Sources

S004 and S005; see the [source register](../../research/sources/market-mechanics-sources.md). The slippage-definition disagreement is tracked in the costs document rather than duplicated here.

## Research Notes

Future gaps: version-specific fees, transaction ordering, finality, token behavior and route simulation. These are not resolved by this introductory batch. The glossary also mixes an individual-pool description with v4's singleton description; use version-specific architecture documentation before implementation.

[Back to knowledge index](../INDEX.md)
