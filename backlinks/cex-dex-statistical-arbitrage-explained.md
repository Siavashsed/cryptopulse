# Backlink content - Most CEX-DEX Arbitrage Profit Goes to Block Builders, Not You
**URL:** https://siavashsed.github.io/cryptopulse/cex-dex-statistical-arbitrage-explained/
**Generated:** 2026-11-15

---

## REDDIT
**Post to:** r/algotrading, r/defi, r/ethfinance
**Title:** Spotting the CEX-DEX price gap was the easy part. Keeping the profit was where I struggled.

Something I wish someone had told me before I spent months on CEX-DEX arb: finding the gap is the easy part. Keeping the profit is the hard part.

The basic trade is simple. Binance moves first, the Uniswap pool lags, so you trade into the pool and hedge on the CEX. The edge is real. The question is who ends up with it. In March 2023 I was running a small ETH-USDC strategy off a rented server in Frankfurt. Trades that looked good on paper kept coming back close to breakeven once I paid to get included in a block.

This is what changed my thinking. On Ethereum, the searcher who spots the gap has to outbid other searchers for block inclusion, and that auction sends most of the surplus to the block builder. The more people chase the same gap, the more of your edge goes into the bid. Lower latency, a cheaper hedge venue or private orderflow can shift the split. For a small operator, though, you usually do the work and the builder keeps the margin.

Has anyone found a setup where the split still works at small size?

Full breakdown here: https://siavashsed.github.io/cryptopulse/cex-dex-statistical-arbitrage-explained/

---

## LINKEDIN
**Hook:** In CEX-DEX arbitrage, the trader who spots the price gap often keeps the smallest share of the profit.

Arbitrage between centralized and decentralized exchanges sounds like a clean trade. Binance moves, a Uniswap pool lags, and you close the gap and hedge.

The edge is real. The question is who keeps it. On Ethereum, searchers compete for block inclusion, and that competition is an auction. The more traders chase the same gap, the more of the expected profit goes into the bid, and the block builder collects it.

I learned this running a small ETH-USDC strategy in 2023. Trades that looked profitable in backtests came back thin once I was paying real inclusion costs.

The lesson goes beyond crypto. When an edge depends on access to a scarce resource, whoever owns that resource tends to capture the surplus. Measure your edge after the cost of access, not before.

Read the full analysis → https://siavashsed.github.io/cryptopulse/cex-dex-statistical-arbitrage-explained/

#AlgorithmicTrading #DeFi #MEV #QuantitativeFinance #Ethereum

---

## QUORA
**Answer this question:** Is CEX-DEX arbitrage still profitable for individual traders?

Short answer: the opportunity still exists, but for most individual traders the profit no longer stays with them.

This is how the trade works. Prices move first on large centralized exchanges like Binance. Automated market maker pools like Uniswap only reprice when someone trades against them, so for a few seconds the pool price is out of date. A CEX-DEX arbitrageur trades the pool back toward the CEX price and hedges the position on the centralized exchange. These gaps are real and they show up all the time.

The problem is getting the trade executed. On Ethereum, landing your trade in a block at the right position means competing with other searchers who see the same gap. That competition works like an auction. Each searcher bids part of their expected profit to the block builder to get included. When several well-equipped players chase the same opportunity, the bids rise toward the full value of the trade. The builder ends up with most of the surplus and the searcher keeps a thin margin.

I ran into this myself in March 2023 with a small ETH-USDC strategy on a rented server in Frankfurt. The signals were fine and the fills were fine. What ate the result was the cost of getting included ahead of everyone else.

What can still work for a smaller trader:
- Less contested pairs or chains, where builder competition is weaker
- Lower hedging costs, since fees on the CEX leg add up quickly
- Treating it as research first and measuring your edge after inclusion costs, not before

I wrote a longer breakdown of how the trade works and where the money actually goes here: https://siavashsed.github.io/cryptopulse/cex-dex-statistical-arbitrage-explained/

If you are considering it, backtest with realistic bid costs. Most strategies that look good on paper fail on that line alone.
