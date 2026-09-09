# Market Mechanics Source Register

Batch: 001. Date Accessed for every entry: 2026-09-09. No crawler dates are treated as publication dates. Official documentation is a version-sensitive description, not evidence of trading edge. Only the review scopes below were inspected; no datasets were downloaded or results replicated.

## S001 — Coinbase trading rules

Source Name / Organization: Coinbase
Page / Article Title: Coinbase Exchange Trading Rules (Trading Rules page)
Author: Coinbase; individual author not stated
URL: https://www.coinbase.com/legal/trading_rules
Publication Date: Not stated in reviewed material
Last Updated: Not stated in reviewed material
Date Accessed: 2026-09-09
Type: Official venue rules
Reviewed: central book/pair definitions; sections 1.7–1.9 on priority, settlement and fees; maintenance context. Browser returned localized variants, including en-br; no jurisdiction-wide legal conclusion is drawn.
Use: F001, F002, F004. Authority limited to named venue/products.
Limit: C001 is tracked in F002; verify effective rules before later execution work.

## S002 — Coinbase matching engine

Source Name / Organization: Coinbase Developer Documentation
Page / Article Title: Exchange Matching Engine
Author: Coinbase; individual author not stated
URL: https://docs.cdp.coinbase.com/exchange/concepts/matching-engine
Publication Date: Not stated
Last Updated: Not stated
Date Accessed: 2026-09-09
Type: Official technical documentation
Reviewed: priority description, self-trade prevention, price improvement and lifecycle sections.
Use: F002. Does not resolve C001's iceberg detail.

## S003 — Coinbase order-book schema

Source Name / Organization: Coinbase Developer Documentation
Page / Article Title: Get product book
Author: Coinbase; individual author not stated
URL: https://docs.cdp.coinbase.com/api-reference/exchange-api/rest-api/products/get-product-book
Publication Date: Not stated
Last Updated: Not stated
Date Accessed: 2026-09-09
Type: Official API documentation
Reviewed: levels, aggregation, indicative auction quotes and auction states. Documentation examples only; no endpoint call.
Use: F002. L-level semantics are venue-specific.

## S004 — Uniswap swaps

Source Name / Organization: Uniswap Developers
Page / Article Title: Understanding Swaps on Uniswap
Author: Organization attribution; individual author not stated
URL: https://developers.uniswap.org/docs/get-started/concepts/traders/swaps
Publication Date: Not stated
Last Updated: Not stated
Date Accessed: 2026-09-09
Type: Official protocol documentation
Reviewed: swap mechanism, version distinctions, protection parameters, price impact and slippage sections.
Use: F001, F003, F004. C003 compares this page with S005.
Limit: The page's broad gas-fee/order-speed explanation is not adopted as a universal transaction-ordering rule; modern ordering needs separate verification.

## S005 — Uniswap glossary

Source Name / Organization: Uniswap Developers
Page / Article Title: Uniswap Protocol Glossary
Author: Organization attribution; individual author not stated
URL: https://developers.uniswap.org/docs/get-started/concepts/glossary
Publication Date: Not stated
Last Updated: Not stated
Date Accessed: 2026-09-09
Type: Official glossary
Reviewed: AMM, constant product, liquidity, price impact/slippage and version-related architecture definitions.
Use: F003 and F004. C003 remains unresolved as terminology.
Limit: Some pool wording is inconsistent with the same page's singleton account; implementation must use version-specific sources. Do not infer that every v4 pool is a separately deployed contract.

## S006 — DEX execution costs

Source Name: arXiv
Page / Article Title: Don't Let MEV Slip: The Costs of Swapping on the Uniswap Protocol
Authors: Austin Adams; Benjamin Y Chan; Sarit Markovich; Xin Wan
URL: https://arxiv.org/abs/2309.13648
Version URL: https://arxiv.org/abs/2309.13648v2
Publication Date: Initial arXiv submission 2023-09-24
Last Updated: arXiv v2, 2024-04-17
Date Accessed: 2026-09-09
Citation: Adams et al., arXiv:2309.13648v2; DOI 10.48550/arXiv.2309.13648.
Type: Academic preprint; journal peer-review status not verified
Reviewed: abstract, author list and submission history only. Full paper, code, sample dates and identification assumptions not inspected.
Use: F004, limited qualitative cost-composition observation from two pools. No numerical performance claims imported. Affiliations and conflicts of interest not verified.

## S007 — Historical market fragmentation

Source Name / Organization: MIT Sloan Consumer Finance Initiative
Page / Article Title: Trading and Arbitrage in Cryptocurrency Markets
Authors: Igor Makarov; Antoinette Schoar
URL: https://mitsloan.mit.edu/cfi/trading-and-arbitrage-cryptocurrency-markets
Publication Date: Article citation identifies 2020; institutional page date not stated
Last Updated: Not stated
Date Accessed: 2026-09-09
Citation: Makarov, I., and Schoar, A. (2020). Trading and arbitrage in cryptocurrency markets. Journal of Financial Economics, 135(2), 293–319.
Type: Authors' institutional summary of a peer-reviewed publication
Reviewed: institutional research summary and bibliographic information, not full methods or dataset.
Use: F001. Historical external finding; not a claim about current markets or project-tested arbitrage.

## S008 — Coinbase product metadata

Source Name / Organization: Coinbase Developer Documentation
Page / Article Title: Get all known trading pairs
Author: Coinbase; individual author not stated
URL: https://docs.cdp.coinbase.com/api-reference/exchange-api/rest-api/products/get-all-known-trading-pairs
Publication Date: Not stated
Last Updated: Not stated; removal notice says June 30 without a year in the reviewed text
Date Accessed: 2026-09-09
Type: Official API documentation
Reviewed: increments, trading-mode flags, mutable fields and order-size removal notice.
Use: F002. C002 records contradictory size-field prose. No current parameter values are adopted.

## Search disposition

Discovery searches covered matching rules, AMM mechanics, crypto fragmentation and execution-cost counterevidence. Social posts, aggregators and unsourced claims in search results were not relied on. The two academic records above support only narrow claims at the reviewed depth. A full-paper review remains a named gap, not a completed verification step.
