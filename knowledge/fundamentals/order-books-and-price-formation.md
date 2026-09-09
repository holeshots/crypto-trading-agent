---
Title: Order Books and Price Formation
Category: fundamentals
Status: NEEDS_REVIEW
Evidence Quality: STRONG
Last Updated: 2026-09-09
Related Files: [trading-venues-and-fragmentation.md, trading-costs-and-slippage.md]
---

# Order Books and Price Formation

## Summary

An order book describes resting buying and selling interest for an instrument. A last trade describes a past transaction. Neither guarantees the price or quantity of a future fill.

## Why It Exists

THEORETICAL EXPLANATION: a matching mechanism lets willingness to trade at different prices meet incoming demand for execution. A queue allocates scarce liquidity; it is not a forecast of fair value.

## How It Works

Definitions used here: best bid `b` is the highest resting buy price, best ask `a` the lowest resting sell price. For an ordinary uncrossed book, spread `s=a-b`; midpoint `m=(a+b)/2`; spread in basis points `10,000*s/m`. Midpoint is a reference, not a promised fill.

FACT, Coinbase API: L1 exposes best prices, L2 aggregates orders by price, and L3 exposes non-aggregated orders. L2 size already sums orders at that level; multiplying it by order count overstates depth. Auction quotes may be indicative rather than firm. [S003](https://docs.cdp.coinbase.com/api-reference/exchange-api/rest-api/products/get-product-book)

FACT, Coinbase matching documentation: executions occur at resting-order prices. An acknowledgment or open order is not itself a fill; self-trade prevention can alter the lifecycle. [S002](https://docs.cdp.coinbase.com/exchange/concepts/matching-engine)

Derived illustration, not market data: asks contain 1 unit at 101 and 2 at 103. Buying 2 units against that frozen book gives `(101+103)/2=102` before fees, not 101 for both units. Assumptions: those quantities remain available, no intervening messages, and the order permits both prices.

## Bullish Interpretation

TRADER INTERPRETATION: more displayed bid depth is sometimes called buying support. It is a hypothesis about future behavior; displayed interest can change without executing.

## Bearish Interpretation

More ask depth is equally ambiguous. Quotes alone do not identify motive or subsequent price direction.

## Market Conditions

Applies to order-book venues; do not impose continuous matching assumptions on auctions or AMMs.

## Timeframes

Event time and snapshots. Candles aggregate away order sequence and queue position.

## Confirmations

RESEARCH PROPOSAL: reconcile timestamped snapshots, updates and actual executions before claiming depth was consumed. Canceled quantity is not traded quantity.

## Invalidation

Sequence gaps, stale snapshots, wrong units or a change of trading mode invalidate a reconstruction until repaired.

## Strengths

Separates quoted liquidity, executed trades and derived reference prices.

## Weaknesses

L2 aggregation does not expose an individual order's queue position. Neither a screenshot nor OHLCV reconstructs all execution constraints.

## Common Failure Modes

Assuming every limit order supplies liquidity; assuming acknowledged means filled; overlooking hidden quantity; treating all matching engines as identical.

## Relationship to Other Concepts

[Venue identity](trading-venues-and-fragmentation.md) specifies which book is relevant; [cost accounting](trading-costs-and-slippage.md) distinguishes a benchmark from the realized price.

## Automation Potential

HIGH for arithmetic and data-integrity checks once feed semantics are specified. Predictive interpretation is unvalidated; no feed or execution code exists.

## Evidence Quality

STRONG for explicitly scoped definitions and documented mechanics, UNKNOWN for directional edge. Unresolved documentation details below prevent treating this as a complete execution specification.

## Sources

[S001 trading rules](https://www.coinbase.com/legal/trading_rules), [S002 matching engine](https://docs.cdp.coinbase.com/exchange/concepts/matching-engine), [S003 book schema](https://docs.cdp.coinbase.com/api-reference/exchange-api/rest-api/products/get-product-book), [S008 product metadata](https://docs.cdp.coinbase.com/api-reference/exchange-api/rest-api/products/get-all-known-trading-pairs). See [register](../../research/sources/market-mechanics-sources.md).

## Research Notes

CONFLICT C001: S002 describes price-time priority; S001 sections 1.71–1.72 specify price-display-time and hidden iceberg treatment. Both prioritize price, but only the latter covers displayed versus hidden interest. Possible reason: simplified or unevenly updated documentation. Preserve both; obtain venue clarification before later queue modeling.

CONFLICT C002: S008 announces removal of several size fields while following prose still describes them. Use neither prose nor examples as a timeless schema. Later work needs dated schema/changelog reconciliation. This review has not called a market endpoint.
