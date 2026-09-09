You are responsible for Phase 1 of this project: building a comprehensive, structured cryptocurrency trading knowledge base.

Do NOT build a trading bot yet.

Do NOT place trades.

Do NOT attempt to predict the current market.

Do NOT perform backtests yet.

Do NOT claim that any strategy is profitable unless that profitability has been established through actual testing in a later phase.

Your sole objective during Phase 1 is to:

RESEARCH → UNDERSTAND → VERIFY → DOCUMENT → ORGANIZE → INDEX

cryptocurrency trading knowledge so that another agent can later retrieve this knowledge when analyzing live markets.

The long-term purpose of this knowledge base is to support a future Crypto Futures Trading Analysis Agent that evaluates whether a trade has positive expected value and can eventually return:

LONG

SHORT

WAIT

NO TRADE

with:

* Entry zone
* Entry trigger
* Stop loss
* TP1
* TP2
* TP3
* Risk/reward
* Expected value
* Invalidation
* Relevant strategy
* Supporting evidence
* Opposing evidence

However, that functionality belongs to later phases.

Phase 1 is strictly a KNOWLEDGE ACQUISITION phase.

---

# PRIMARY OBJECTIVE

Build a highly comprehensive, trustworthy, structured, searchable, and evidence-aware cryptocurrency trading knowledge repository.

Research cryptocurrency trading from foundational concepts through advanced professional, discretionary, quantitative, statistical, derivatives, and market-microstructure methodologies.

Your objective is NOT to blindly collect strategies from the internet.

Your objective is to understand:

WHAT each concept is.

WHY traders use it.

HOW it is supposed to work.

WHEN it may work.

WHEN it may fail.

WHAT evidence supports it.

WHAT evidence contradicts it.

HOW it can eventually be tested.

HOW it relates to other concepts.

Do not assume popularity equals validity.

Treat every trading strategy as a hypothesis until it has been empirically tested.

---

# FIRST TASK — REPOSITORY STRUCTURE

Inspect the existing repository before making changes.

Create missing directories only when necessary.

Establish approximately the following structure:

knowledge/

* fundamentals/
* market-structure/
* price-action/
* liquidity/
* smart-money/
* indicators/
* volume/
* order-flow/
* derivatives/
* strategies/
* market-regimes/
* quantitative/
* on-chain/
* macro/
* sentiment/
* risk-management/
* trade-management/

strategies/

* researched/
* candidates/
* validated/
* rejected/

research/

* sources/
* research-log.md

backtests/

data/

src/

Create:

knowledge/INDEX.md

if it does not exist.

Maintain knowledge/INDEX.md as the central navigation layer for the entire trading knowledge repository.

Do NOT populate candidates/, validated/, or rejected/ with strategy classifications during Phase 1 unless they already contain material from an earlier completed phase.

During Phase 1, discovered strategies remain RESEARCHED / NOT TESTED / NOT VALIDATED.

---

# RESEARCH SCOPE

Research cryptocurrency trading comprehensively.

Your research should eventually include, but is not limited to, the following areas.

---

# 1. CRYPTO MARKET FUNDAMENTALS

Study:

* Cryptocurrency exchanges
* Centralized exchanges
* Decentralized exchanges where relevant
* Spot markets
* Futures markets
* Perpetual futures
* Options
* Margin trading
* Leverage
* Long positions
* Short positions
* Contract specifications
* Settlement
* Mark price
* Index price
* Bid
* Ask
* Spread
* Market depth
* Liquidity
* Slippage
* Maker fees
* Taker fees
* Order execution
* Market orders
* Limit orders
* Stop orders
* Stop-limit orders
* Conditional orders
* Reduce-only orders
* Post-only orders
* Trailing stops

Understand how exchange mechanics affect real trading outcomes.

---

# 2. LEVERAGE, MARGIN, AND LIQUIDATION

Study:

* Initial margin
* Maintenance margin
* Isolated margin
* Cross margin
* Leverage
* Liquidation price
* Liquidation engines
* Auto-deleveraging where applicable
* Bankruptcy price
* Margin requirements
* Position sizing
* Leverage risk

Understand leverage mathematically.

Never confuse leverage with trading edge.

---

# 3. PERPETUAL FUTURES AND FUNDING

Study:

* Perpetual swaps
* Funding rates
* Positive funding
* Negative funding
* Funding intervals
* Funding arbitrage
* Crowded positioning
* Funding-rate extremes
* Relationship between funding and market sentiment

Document both common trader interpretations and stronger empirical evidence where available.

---

# 4. MARKET STRUCTURE

Study:

* Swing highs
* Swing lows
* Higher highs
* Higher lows
* Lower highs
* Lower lows
* Trend structure
* Range structure
* Break of Structure
* Change of Character
* Market Structure Shift
* Support
* Resistance
* Supply
* Demand
* Consolidation
* Expansion
* Accumulation
* Distribution
* Reaccumulation
* Redistribution
* Breakouts
* Retests
* Failed breakouts
* Price discovery

When terminology differs across trading schools, document those differences.

---

# 5. PRICE ACTION

Study:

* Candlestick behavior
* Pin bars
* Engulfing candles
* Inside bars
* Outside bars
* Doji
* Rejection candles
* Momentum candles
* Compression
* Expansion
* Break-and-retest
* Trend continuation
* Pullback trading
* Reversal trading
* Range trading
* Momentum trading
* Exhaustion behavior

Determine where concepts are objectively definable and where interpretation is subjective.

---

# 6. LIQUIDITY

Study:

* Liquidity pools
* Buy-side liquidity
* Sell-side liquidity
* Equal highs
* Equal lows
* Previous highs
* Previous lows
* Previous day high/low
* Previous week high/low
* Session highs/lows
* Stop runs
* Stop hunts
* Liquidity sweeps
* Liquidity grabs
* Inducement
* Internal liquidity
* External liquidity
* Sweep-and-reversal setups
* Sweep-and-continuation setups

Distinguish observable market behavior from trader theories about why that behavior occurs.

---

# 7. SMART MONEY / ICT-STYLE CONCEPTS

Research objectively:

* Order blocks
* Breaker blocks
* Mitigation blocks
* Fair Value Gaps
* Inverse Fair Value Gaps
* Imbalances
* Displacement
* Liquidity voids
* Premium and discount
* Optimal Trade Entry
* Power of Three
* Judas Swing
* Kill zones
* Balanced Price Range
* Consequent encroachment
* SMT divergence
* Turtle Soup
* Dealing ranges
* Market maker models

Do NOT treat these concepts as scientifically proven simply because they are widely discussed.

Where possible, identify overlaps with older technical-analysis or market-microstructure concepts.

---

# 8. TECHNICAL INDICATORS

Study:

* SMA
* EMA
* WMA
* VWMA
* RSI
* Stochastic RSI
* MACD
* Bollinger Bands
* ATR
* ADX
* CCI
* ROC
* Momentum indicators
* Williams %R
* Parabolic SAR
* Ichimoku Cloud
* Supertrend
* Donchian Channels
* Keltner Channels
* Pivot points
* Fibonacci retracement
* Fibonacci extension
* VWAP
* Anchored VWAP
* Volume Profile
* Market Profile
* OBV
* Money Flow Index
* Chaikin Money Flow

For each indicator understand:

* Formula
* Interpretation
* Common parameters
* Lag
* Strengths
* Weaknesses
* False-signal conditions
* Suitable market regimes
* Unsuitable market regimes
* Relationship to other indicators

Do not assume default settings are universally optimal.

---

# 9. VOLUME ANALYSIS

Study:

* Trading volume
* Relative volume
* Volume spikes
* Volume confirmation
* Volume divergence
* Volume Profile
* Point of Control
* Value Area High
* Value Area Low
* High-volume nodes
* Low-volume nodes
* Cumulative volume
* Buy/sell volume
* Volume imbalance
* Absorption
* Exhaustion

---

# 10. ORDER FLOW

Study:

* Order books
* Level 2 data
* Market depth
* Footprint charts
* Bid/ask delta
* Cumulative Volume Delta
* Aggressive buyers
* Aggressive sellers
* Absorption
* Exhaustion
* Iceberg orders
* Spoofing concepts
* Large resting orders
* Order-flow imbalance
* Liquidation clusters

Understand that displayed order-book liquidity can change or disappear and may not represent true intent.

---

# 11. OPEN INTEREST AND DERIVATIVES DATA

Study:

* Open interest
* Open-interest changes
* Funding rates
* Long/short ratios
* Liquidation data
* Futures basis
* Futures premiums
* Contango
* Backwardation
* Options implied volatility
* Options skew
* Put/call ratios
* Gamma-related concepts where relevant

Study interpretations of:

Price increasing + OI increasing

Price increasing + OI decreasing

Price decreasing + OI increasing

Price decreasing + OI decreasing

Document limitations and alternate interpretations.

---

# 12. TREND-FOLLOWING STRATEGIES

Research:

* Moving-average trends
* Moving-average crossovers
* Breakout systems
* Donchian systems
* Turtle Trading concepts
* Momentum continuation
* Trend pullbacks
* Supertrend systems
* ADX filters
* Multi-timeframe alignment

---

# 13. MEAN-REVERSION STRATEGIES

Research:

* Bollinger Band reversion
* RSI extremes
* VWAP reversion
* Z-score strategies
* Statistical mean reversion
* Range extremes
* Deviation-from-average systems

Document when mean reversion becomes especially dangerous during strong directional markets.

---

# 14. BREAKOUT STRATEGIES

Research:

* Range breakouts
* Support/resistance breakouts
* Volatility breakouts
* Opening-range concepts
* Donchian breakouts
* Volume-confirmed breakouts
* Breakout-retest setups
* Failed breakout strategies

---

# 15. SCALPING

Study:

* 1-minute scalping
* 3-minute scalping
* 5-minute scalping
* Momentum scalping
* VWAP scalping
* Range scalping
* Breakout scalping
* Order-flow scalping
* Liquidation-based scalping

Account for:

* Fees
* Spread
* Slippage
* Latency
* Execution quality

A strategy that appears profitable before transaction costs may fail after costs.

---

# 16. DAY TRADING

Study:

* Session structure
* Asian session
* London session
* New York session
* Session overlap
* Previous-day levels
* Intraday VWAP
* Intraday liquidity
* Opening volatility
* Momentum
* Reversals
* Breakouts

---

# 17. SWING TRADING

Study:

* Daily structure
* 4H structure
* Multi-day support/resistance
* Trend continuation
* Pullbacks
* Breakouts
* Macro conditions
* Position management

---

# 18. POSITION TRADING

Study:

* Weekly structure
* Monthly structure
* Market cycles
* Macro trends
* Fundamental analysis
* On-chain information
* Monetary conditions
* Bitcoin cycles
* Longer-term position management

---

# 19. MULTI-TIMEFRAME ANALYSIS

Study combinations involving:

* Monthly
* Weekly
* Daily
* 4H
* 1H
* 15m
* 5m
* 1m

Research top-down analysis and timeframe alignment.

Document which timeframe combinations are typically used for different trading styles.

---

# 20. CHART PATTERNS

Research:

* Head and shoulders
* Inverse head and shoulders
* Double tops
* Double bottoms
* Triple tops
* Triple bottoms
* Triangles
* Flags
* Pennants
* Wedges
* Channels
* Cup and handle
* Rounding formations

Investigate statistical evidence where reliable evidence exists.

---

# 21. HARMONIC TRADING

Study:

* Gartley
* Butterfly
* Bat
* Crab
* Shark
* Cypher
* AB=CD

Document Fibonacci requirements, interpretation, subjectivity, and invalidation.

---

# 22. ELLIOTT WAVE

Study:

* Impulse waves
* Corrective waves
* Wave counting
* Fibonacci relationships
* Common practitioner rules
* Subjectivity
* Criticisms
* Potential failure modes

---

# 23. WYCKOFF

Study:

* Accumulation
* Distribution
* Springs
* Upthrusts
* Sign of Strength
* Sign of Weakness
* Last Point of Support
* Last Point of Supply
* Wyckoff phases
* Composite operator theory

Separate observable price/volume behavior from theoretical interpretations.

---

# 24. FIBONACCI TRADING

Study:

* Retracements
* Extensions
* Golden pocket
* Fibonacci confluence
* Projection targets

Research whether empirical evidence supports common interpretations.

---

# 25. STATISTICAL TRADING

Study:

* Mean reversion
* Z-scores
* Correlation
* Cointegration
* Regression
* Volatility models
* Time-series momentum
* Cross-sectional momentum
* Statistical arbitrage
* Pairs trading

---

# 26. QUANTITATIVE STRATEGIES

Study:

* Rule-based systems
* Momentum models
* Trend models
* Mean-reversion algorithms
* Factor models
* Volatility targeting
* Regime classification
* Ensemble approaches
* Machine-learning approaches

Understand:

* Overfitting
* Curve fitting
* Data snooping
* Look-ahead bias
* Survivorship bias
* Selection bias
* Data leakage
* Parameter instability

---

# 27. ARBITRAGE

Study:

* Cross-exchange arbitrage
* Triangular arbitrage
* Spot/futures arbitrage
* Cash-and-carry
* Basis trading
* Funding-rate arbitrage
* Statistical arbitrage

Account for:

* Fees
* Transfer delays
* Counterparty risk
* Execution risk
* Withdrawal restrictions
* Liquidity
* Capital requirements

---

# 28. GRID TRADING

Study:

* Neutral grids
* Long grids
* Short grids
* Arithmetic grids
* Geometric grids
* Dynamic grids

Understand how grid strategies can fail during strong directional moves.

---

# 29. DCA AND POSITION BUILDING

Research:

* Dollar-cost averaging
* Value averaging
* Dynamic DCA
* Trend-adjusted DCA
* Scaling into positions
* Scaling out
* Pyramiding

Clearly distinguish investment approaches from leveraged futures strategies.

---

# 30. MARTINGALE AND ANTI-MARTINGALE

Research:

* Martingale
* Anti-martingale
* Position escalation
* Risk of ruin
* Drawdown behavior
* Pyramiding into winners

Treat martingale approaches as high-risk.

Do not normalize them simply because historical examples appear profitable.

---

# 31. ON-CHAIN ANALYSIS

Study:

* Exchange inflows/outflows
* Whale activity
* Active addresses
* Realized cap
* MVRV
* NUPL
* SOPR
* Dormancy
* Coin Days Destroyed
* Long-term holder behavior
* Miner activity
* Stablecoin supply
* Network activity

Document latency and interpretation limitations.

---

# 32. SENTIMENT

Study:

* Fear & Greed
* Social sentiment
* Search trends
* News sentiment
* X/Twitter sentiment
* Reddit sentiment
* Funding sentiment
* Retail positioning
* Contrarian sentiment strategies

Treat sentiment data carefully and distinguish measurement from narrative.

---

# 33. NEWS AND EVENT TRADING

Study effects of:

* CPI
* FOMC
* Interest-rate decisions
* Employment reports
* ETF developments
* Exchange failures
* Hacks
* Regulation
* Token listings
* Token unlocks
* Protocol upgrades
* Major lawsuits
* Geopolitical events

Document event-risk, liquidity, spread, and volatility concerns.

---

# 34. INTERMARKET AND MACRO ANALYSIS

Research relationships between crypto and:

* Nasdaq
* S&P 500
* DXY
* Treasury yields
* Interest rates
* Gold
* Global liquidity
* Equity volatility
* Stablecoin liquidity

Do not assume correlations are permanent.

---

# 35. MARKET REGIMES

Learn to classify:

* Bull trend
* Bear trend
* Sideways/range
* High volatility
* Low volatility
* Expansion
* Compression
* Risk-on
* Risk-off

Determine which strategies are theoretically or empirically better suited to each regime.

---

# 36. RISK MANAGEMENT

Treat risk management as more important than entry strategy.

Study:

* Position sizing
* Fixed fractional risk
* Percentage risk
* Volatility-adjusted sizing
* ATR-based stops
* Structure-based stops
* Risk/reward
* Expectancy
* R-multiples
* Maximum drawdown
* Daily loss limits
* Weekly loss limits
* Correlated exposure
* Risk of ruin
* Kelly criterion
* Fractional Kelly
* Maximum adverse excursion
* Maximum favorable excursion

Never assume high win rate means profitability.

---

# 37. TRADE MANAGEMENT

Study:

* Fixed take profits
* Partial take profits
* Scaling out
* Scaling in
* Trailing stops
* Breakeven management
* Structure-based exits
* Volatility-based exits
* Time-based exits
* Runner positions
* Re-entry

---

# 38. TRADING PSYCHOLOGY

Study:

* FOMO
* Revenge trading
* Overtrading
* Loss aversion
* Recency bias
* Confirmation bias
* Gambler's fallacy
* Anchoring
* Overconfidence
* Tilt
* Discipline
* Patience
* Process-oriented trading

Where possible, translate psychological lessons into objective risk or process rules.

---

# KNOWLEDGE FILE RULES

Prefer approximately one Markdown file per meaningful concept or strategy.

Examples:

knowledge/liquidity/liquidity-sweep.md

knowledge/derivatives/open-interest.md

knowledge/indicators/vwap.md

knowledge/strategies/trend-pullback.md

Do NOT create one giant document containing all trading knowledge.

However, do NOT create excessive tiny files for minor observations.

Group closely related concepts where appropriate.

Optimize for retrievability rather than file count.

---

# FILE NAMING RULES

Use lowercase kebab-case filenames.

GOOD:

market-structure.md

break-of-structure.md

liquidity-sweep.md

open-interest.md

funding-rate.md

trend-pullback.md

vwap-mean-reversion.md

BAD:

final-strategy.md

new-strategy-2.md

random-notes.md

strategy123.md

misc.md

Use descriptive, stable filenames.

---

# KNOWLEDGE FILE FRONT MATTER

At the beginning of every substantial knowledge document include:

Title:

Category:

Status:
RESEARCHED / NEEDS_REVIEW / INCOMPLETE

Evidence Quality:
STRONG / MODERATE / WEAK / ANECDOTAL / UNKNOWN

Last Updated:

Related Files:

---

# REQUIRED KNOWLEDGE FILE FORMAT

Every substantial knowledge file should approximately follow:

# Concept Name

## Summary

Explain the concept clearly.

## Why It Exists

Explain the underlying market behavior, mechanism, or theory.

## How It Works

Describe the concept thoroughly.

## Bullish Interpretation

When applicable.

## Bearish Interpretation

When applicable.

## Market Conditions

Explain the environments where the concept is typically relevant.

## Timeframes

Describe applicable timeframes where relevant.

## Confirmations

Describe possible confirming evidence.

## Invalidation

Explain what would invalidate the interpretation.

## Strengths

## Weaknesses

## Common Failure Modes

## Relationship to Other Concepts

Reference related knowledge files.

## Automation Potential

LOW / MEDIUM / HIGH

Explain why.

## Evidence Quality

STRONG / MODERATE / WEAK / ANECDOTAL / UNKNOWN

Explain why this rating was assigned.

## Sources

Record credible sources.

## Research Notes

Document:

* uncertainties
* disagreements
* alternative interpretations
* hypotheses
* parameters requiring future testing

---

# STRATEGY DOCUMENT FORMAT

Whenever you discover an actual trading strategy, document it separately.

Use:

# Strategy Name

## Metadata

Status: RESEARCHED

Backtest Status: NOT TESTED

Validation Status: NOT VALIDATED

Evidence Quality:

Strategy Family:

## Description

## Market

## Trading Style

SCALP / DAY TRADE / SWING / POSITION / ARBITRAGE / OTHER

## Market Regime

## Recommended Timeframes

## Required Data

## Indicators or Tools

## Long Conditions

## Short Conditions

## Entry Method

## Entry Confirmation

## Stop Loss Rule

## Take Profit Rule

## Position Management

## Invalidation

## Do Not Trade Conditions

## Expected Advantages

## Known Weaknesses

## Common Failure Modes

## Transaction Cost Sensitivity

## Subjectivity

LOW / MEDIUM / HIGH

## Automation Potential

LOW / MEDIUM / HIGH

## Evidence Quality

STRONG / MODERATE / WEAK / ANECDOTAL / UNKNOWN

## Related Strategies

## Sources

## Testable Components

Identify components that could eventually be converted into deterministic rules.

## Parameters Requiring Testing

Do not invent optimal parameters.

## Research Notes

---

# STRATEGY STATUS RULE

Every newly discovered strategy begins as:

Status: RESEARCHED

Backtest Status: NOT TESTED

Validation Status: NOT VALIDATED

During Phase 1, do NOT promote strategies to:

CANDIDATE

VALIDATED

or

REJECTED

Those decisions belong to later phases after empirical testing.

---

# NEVER INVENT PERFORMANCE DATA

Do NOT invent:

* Win rate
* Expectancy
* Profit factor
* Sharpe ratio
* Sortino ratio
* Maximum drawdown
* Average R
* Historical returns
* Historical trade count
* Backtest performance
* Probability of success

If a credible source reports a number, clearly attribute it to that source.

Do not treat externally reported results as independently validated project results.

---

# SOURCE QUALITY

Prefer:

1. Peer-reviewed research
2. Academic papers
3. Official exchange documentation
4. Primary documentation
5. Reputable quantitative research
6. Established financial literature
7. Professional market research
8. Experienced practitioners with transparent methodologies

Treat cautiously:

* Trading blogs
* YouTube
* Social media
* Forums
* Influencers
* Anonymous strategies
* Screenshot-based claims
* Affiliate marketing content

A weak source may still be useful for discovering a hypothesis.

It must not automatically become established knowledge.

---

# SOURCE RECORDING

For important web sources record when available:

Source Name:

Page / Article Title:

Author:

URL:

Publication Date:

Last Updated:

Date Accessed:

Do NOT fabricate unavailable source metadata.

For academic sources record appropriate citation information.

For official documentation record the organization and page/document title.

---

# CLAIM CLASSIFICATION

Distinguish important statements as appropriate between:

FACT

EMPIRICAL FINDING

THEORETICAL EXPLANATION

TRADER INTERPRETATION

ANECDOTAL CLAIM

HYPOTHESIS

PARAMETER TO TEST

Do not present:

TRADER INTERPRETATION

as:

FACT.

---

# CONFLICT HANDLING

When credible sources disagree:

Do not silently choose one interpretation.

Document:

INTERPRETATION A

INTERPRETATION B

Evidence supporting A

Evidence supporting B

Shared assumptions

Differences

Possible reason for disagreement

What testing would help distinguish them

Mark the topic:

NEEDS_REVIEW

or:

NEEDS_VALIDATION

when appropriate.

---

# COUNTEREVIDENCE

For promising trading concepts and strategies, actively search for counterevidence.

Ask:

* Has the effect failed in other studies?
* Does it disappear after fees?
* Is it regime-dependent?
* Could it result from hindsight?
* Could it result from data snooping?
* Is it overfit?
* Does it work only on BTC?
* Does it work across exchanges?
* Does it survive different time periods?
* Is there a plausible alternative explanation?

Do not research only evidence that supports a strategy.

Attempt to falsify claims.

---

# DUPLICATION RULE

Before creating a new knowledge file:

1. Search the repository.
2. Check knowledge/INDEX.md.
3. Check related folders.
4. Check alternative terminology.
5. Determine whether the same concept already exists.

If equivalent knowledge already exists:

UPDATE the existing file.

Add alternate names where useful.

Do NOT create a duplicate.

Many strategies use different names for almost identical mechanics.

Group them into strategy families when appropriate.

---

# CROSS-LINKING

Knowledge files should reference related files using relative paths where useful.

Example:

Related concepts:

* ../market-structure/change-of-character.md
* ../liquidity/liquidity-sweep.md
* ../volume/cumulative-volume-delta.md
* ../derivatives/open-interest.md

Build a connected knowledge repository rather than isolated documents.

---

# INDEX.MD

Maintain:

knowledge/INDEX.md

INDEX.md is the primary navigation system for future trading agents.

A future agent should NOT need to read the entire repository to analyze a market.

INDEX.md should organize knowledge by:

* Topic
* Strategy family
* Market regime
* Trading style
* Data type
* Timeframe where useful

Example:

## Trending Markets

Relevant knowledge:

* market-structure/trend-structure.md
* strategies/trend-pullback.md
* strategies/breakout-retest.md
* indicators/moving-averages.md
* derivatives/open-interest.md

## Ranging Markets

Relevant knowledge:

* price-action/range-trading.md
* strategies/mean-reversion.md
* liquidity/liquidity-sweep.md
* indicators/vwap.md

## Liquidity Reversal Setups

Relevant knowledge:

* liquidity/liquidity-sweep.md
* market-structure/change-of-character.md
* volume/cumulative-volume-delta.md
* derivatives/open-interest.md

The purpose of INDEX.md is to minimize unnecessary context and token usage during future live analysis.

---

# RESEARCH LOG

Maintain:

research/research-log.md

After every research batch record:

Date:

Research Category:

Topics Researched:

Files Created:

Files Updated:

Sources Reviewed:

Important Findings:

Contradictory Findings:

Knowledge Gaps:

Hypotheses Created:

Topics Requiring Future Validation:

Recommended Next Research Category:

---

# RESEARCH DEPTH

Do NOT optimize for file count.

One high-quality, well-sourced document is better than ten superficial documents.

A concept is sufficiently researched for Phase 1 when the document reasonably explains:

WHAT it is.

WHY it exists or why traders believe it exists.

HOW it works.

WHEN it may be useful.

WHEN it may fail.

HOW it relates to other concepts.

WHAT evidence supports it.

WHAT evidence challenges it.

WHAT remains uncertain.

WHAT should eventually be tested.

---

# FIRST RESEARCH ORDER

Research approximately in this order:

1. Crypto market mechanics
2. Spot vs futures
3. Perpetual futures
4. Orders and execution
5. Leverage and margin
6. Liquidations
7. Funding
8. Market structure
9. Support and resistance
10. Price action
11. Liquidity
12. Volume
13. Order flow
14. Futures and derivatives data
15. Market regimes
16. Risk management
17. Technical indicators
18. Trend-following strategies
19. Mean-reversion strategies
20. Breakout strategies
21. Scalping
22. Day trading
23. Swing trading
24. Advanced discretionary methodologies
25. Statistical strategies
26. Quantitative strategies
27. Arbitrage
28. On-chain analysis
29. Macro analysis
30. Sentiment analysis
31. Trading psychology
32. Trade management

Do NOT begin with random internet strategies.

Build foundational understanding first.

---

# PHASE 1 EXECUTION RULES

Work systematically.

Do NOT attempt to research the entire field in a single uncontrolled run.

For each research batch:

1. Select the assigned major knowledge category.

2. Review AGENTS.md and repository instructions if present.

3. Read knowledge/INDEX.md.

4. Search existing repository files.

5. Identify existing knowledge relevant to the category.

6. Research the category using credible sources.

7. Identify major concepts and strategy relationships.

8. Create new files only when necessary.

9. Update existing files where appropriate.

10. Add sources.

11. Cross-link related knowledge.

12. Update knowledge/INDEX.md.

13. Update research/research-log.md.

14. Review the work for:

* duplicate files
* unsupported claims
* contradictory statements
* fabricated precision
* weak sourcing
* missing context
* terminology conflicts

15. Correct identified problems.

16. Produce a completion report.

17. STOP.

Do not automatically move to the next research category unless the current user instruction explicitly authorizes multiple categories or tells you to continue.

---

# TOKEN AND COMPUTE CONTROL

Research quality is more important than continuous autonomous activity.

Do not repeatedly reread the entire repository.

Use:

knowledge/INDEX.md

and repository search to locate relevant material.

Do not conduct endless research loops.

Do not repeatedly search for the same information after sufficient high-quality coverage has been achieved.

Stop a research category when:

* Major concepts are adequately documented.
* Additional sources mainly repeat existing knowledge.
* Further progress requires empirical testing rather than research.
* Reliable sources have been reasonably exhausted.
* The assigned research batch has been completed.

---

# PHASE 1 COMPLETION REPORT

At the end of every research batch output:

PHASE:
Phase 1 — Knowledge Acquisition

CATEGORY COMPLETED:

FILES CREATED:

FILES UPDATED:

SOURCES REVIEWED:

IMPORTANT FINDINGS:

CONFLICTING INFORMATION:

KNOWLEDGE GAPS:

HYPOTHESES DISCOVERED:

TOPICS REQUIRING FUTURE VALIDATION:

RECOMMENDED NEXT CATEGORY:

STATUS:
COMPLETE / PARTIAL / NEEDS_REVIEW

Then STOP unless explicitly instructed to continue.

---

# QUALITY CONTROL

Before finishing every batch ask:

Did I rely too heavily on weak sources?

Did I confuse trader theory with market fact?

Did I create duplicate knowledge?

Did I invent parameters?

Did I imply profitability without evidence?

Did I ignore fees, funding, spread, or slippage where relevant?

Did I ignore contradictory evidence?

Did I overstate certainty?

Did I distinguish research from validated trading knowledge?

Did I properly update INDEX.md?

Did I properly update the research log?

Correct problems before completing the task.

---

# PHASE 1 SUCCESS CRITERIA

Phase 1 is successful when:

* Major crypto trading concepts have organized documentation.
* Foundational market mechanics are thoroughly covered.
* Strategy families are documented.
* Strategies use consistent structured templates.
* Important claims contain source references.
* Weak and anecdotal evidence is identified.
* Conflicting theories are preserved rather than hidden.
* Duplicate concepts are consolidated.
* INDEX.md provides effective navigation.
* Files are cross-linked where useful.
* Future agents can retrieve relevant knowledge without reading everything.
* No strategy profitability has been fabricated.
* No strategy has been incorrectly labeled validated.
* Strategies requiring empirical testing are identifiable.
* The repository is ready for Phase 2 strategy formalization.

The objective is NOT to create the largest possible repository.

The objective is to create a knowledge repository that is:

ACCURATE

STRUCTURED

SEARCHABLE

RETRIEVABLE

EVIDENCE-AWARE

TESTABLE

MAINTAINABLE

and useful for future positive-expected-value trading analysis.

---

# LONG-TERM ARCHITECTURE

Remember that this project will eventually proceed through separate phases:

PHASE 1
Knowledge Acquisition

↓

PHASE 2
Strategy Formalization

↓

PHASE 3
Backtesting

↓

PHASE 4
Validation

↓

PHASE 5
Live Market Data Integration

↓

PHASE 6
Trade Analysis

↓

PHASE 7
Paper Trading

↓

PHASE 8
Performance Evaluation

↓

PHASE 9
Small Live Deployment Consideration

↓

PHASE 10
Execution Automation Consideration

Do not perform work belonging to later phases unless explicitly instructed.

---

# FINAL PRINCIPLE

Your task during Phase 1 is not to become confident about trading.

Your task is to build reliable knowledge.

Do not optimize for finding profitable-sounding strategies.

Optimize for finding knowledge and strategies that can eventually be:

DEFINED

UNDERSTOOD

SOURCED

CHALLENGED

FORMALIZED

TESTED

FALSIFIED

COMPARED

VALIDATED.

For now:

RESEARCH → UNDERSTAND → VERIFY → DOCUMENT → INDEX → STOP.

Begin by inspecting the repository, creating any missing Phase 1 structure, creating or updating knowledge/INDEX.md and research/research-log.md, and then researching the first assigned foundational category.
