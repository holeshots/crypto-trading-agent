# Knowledge Index

Last Updated: 2026-09-09

Phase: 1 — Knowledge Acquisition. Overall status: INCOMPLETE.

Read only the relevant concept, its evidence limitations, and linked sources. RESEARCHED means a bounded literature review, not validated predictive usefulness. NEEDS_REVIEW identifies an unresolved source or terminology conflict.

## By topic

| ID | Document | Coverage and alternate names | Status |
|---|---|---|---|
| F001 | [Trading venues and fragmented markets](fundamentals/trading-venues-and-fragmentation.md) | CEX, DEX, exchange, trading pair, base/quote, settlement, price discovery, venue premium | RESEARCHED |
| F002 | [Order books and price formation](fundamentals/order-books-and-price-formation.md) | Bid, ask, spread, midpoint, last price, depth, L1/L2/L3, matching, maker/taker | NEEDS_REVIEW |
| F003 | [AMM and DEX mechanics](fundamentals/amm-and-dex-mechanics.md) | Liquidity pool, swap, reserves, constant product, concentrated liquidity | RESEARCHED |
| F004 | [Trading costs and slippage](fundamentals/trading-costs-and-slippage.md) | Fees, execution price, price impact, slippage, gas, latency, cost accounting | NEEDS_REVIEW |

## By strategy family

No strategy documents yet. These are prerequisite reading paths, not strategy endorsements:

- Trend, momentum, breakout, mean reversion: F002 → F004.
- Order-flow and liquidity hypotheses: F002 → F001 → F004.
- Cross-venue arbitrage hypotheses: F001 → F004.
- AMM/DEX execution hypotheses: F003 → F004.

Future strategy specifications live in `../strategies/researched/`; `knowledge/strategies/` is reserved for family comparisons, avoiding duplicate specifications.

## By market regime

| Context | Retrieve | Limit |
|---|---|---|
| Trend or range | [F002](fundamentals/order-books-and-price-formation.md), [F004](fundamentals/trading-costs-and-slippage.md) | Mechanics apply; regime detection is unresearched |
| Thin liquidity or rapid repricing | [F002](fundamentals/order-books-and-price-formation.md), [F004](fundamentals/trading-costs-and-slippage.md) | No measured cost threshold |
| Venue dislocation | [F001](fundamentals/trading-venues-and-fragmentation.md) | A premium is not proof of attainable arbitrage |
| AMM liquidity concentrated away from price | [F003](fundamentals/amm-and-dex-mechanics.md) | No directional forecast |

## By trading style and timeframe

- Scalp/day trade; 1m, 3m, 5m, 15m, 1H: F002 and F004. Execution information exists below candle resolution; no interval is endorsed.
- Swing/position; 4H, daily, weekly, monthly: F001 and F004. Holding longer does not eliminate entry, exit, or venue constraints.
- Arbitrage/event time: F001, F002, F003, F004. Compare synchronized observations and actual instrument identity.

## By data type

- Product metadata and venue rules: F001, F002.
- Trades, last price, bid/ask, depth snapshots: F002.
- Pool reserves, ticks, swap receipts and quotes: F003.
- Fill records, fee schedules, timestamps and cost benchmarks: F004.
- OHLCV alone: insufficient to reconstruct queues or intrabar fills; see F002.
- Funding, mark/index price, OI, options, on-chain metrics, macro and sentiment: not yet researched.

## Research queue and coverage boundary

The full 38-area scope is retained in the [original brief](../research/phase-1-brief.md). Directory existence does not mean researched coverage. After each authorized batch, replace the relevant queue entry with links and explicit gaps.

1. Crypto market mechanics — batch 001 delivered above; source conflicts remain explicitly flagged.
2. **Next: spot versus futures** — ownership/exposure, long/short, dated contracts, specifications and settlement; options orientation.
3. Perpetual futures.
4. Orders and execution — complete order-type taxonomy including conditional, stop-limit, reduce-only, post-only and trailing orders.
5. Leverage and margin.
6. Liquidations and auto-deleveraging.
7. Funding.
8. Market structure.
9. Support and resistance.
10. Price action and chart patterns.
11. Liquidity and sweep interpretations.
12. Volume.
13. Order flow.
14. Futures and derivatives data.
15. Market regimes.
16. Risk management.
17. Technical indicators — per-indicator formulas and limitations.
18. Trend-following strategies.
19. Mean-reversion strategies.
20. Breakout strategies.
21. Scalping.
22. Day trading and sessions.
23. Swing/position trading and multi-timeframe analysis.
24. Advanced discretionary methodologies — ICT/SMC, harmonics, Elliott Wave, Wyckoff and Fibonacci.
25. Statistical strategies.
26. Quantitative strategies; grid, DCA/position building, martingale/anti-martingale comparisons.
27. Arbitrage.
28. On-chain analysis.
29. Macro/intermarket and news/events.
30. Sentiment.
31. Trading psychology.
32. Trade management.

## Governance and audit

[Research standards](../research/research-standards.md) · [Sources](../research/sources/market-mechanics-sources.md) · [Research log](../research/research-log.md) · [Knowledge template](../research/templates/knowledge-template.md) · [Strategy template](../research/templates/strategy-template.md)

No strategy has been tested, promoted, validated, or rejected. Batch completion does not authorize moving into the next category.
