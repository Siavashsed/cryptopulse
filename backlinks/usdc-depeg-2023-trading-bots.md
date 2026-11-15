# Backlink content - USDC Hit 87 Cents and Exposed Every Lazy Stablecoin Bot
**URL:** https://siavashsed.github.io/cryptopulse/usdc-depeg-2023-trading-bots/
**Generated:** 2026-11-15

---

## REDDIT
**Post to:** r/algotrading, r/CryptoCurrency, r/defi
**Title:** Does your bot still mark stablecoins at a hardcoded 1.00? The USDC depeg showed why that's a risk

Looking back at the March 2023 USDC depeg, what still bugs me is how many bots treated a stablecoin as a hardcoded 1.00. They didn't use a price feed. They used a constant.

When Circle disclosed $3.3B stuck at SVB, USDC slid to roughly 0.87 on some venues over the weekend. Any bot that marked USDC collateral at par kept reporting healthy margin while the real value was falling. That covered basis trades, grid bots quoting in USDC, and anything using it as the 'risk-free' leg. The PnL looked fine right up until you tried to exit.

A few things that would have caught it:
- Price the stablecoin like any other asset, from more than one source (a CEX order book plus a DEX pool like Curve)
- A deviation threshold, something like 0.5% off peg, that halts new orders
- A weekend and off-hours alert path that actually wakes a human

Curious how others handle this now. Do you mark stables at par or use a live price? And did anyone have a peg circuit breaker in place before March 2023?

Full breakdown here: https://siavashsed.github.io/cryptopulse/usdc-depeg-2023-trading-bots/

---

## LINKEDIN
**Hook:** In March 2023, most crypto trading bots assumed one USDC equals one dollar. It did not.

When Silicon Valley Bank failed and Circle disclosed $3.3 billion in deposits there, USDC traded as low as roughly 87 cents over a single weekend.

Holders weren't the only ones hit. Trading systems that hardcoded the stablecoin at par kept marking collateral as healthy, kept quoting, and kept sizing positions against a number that no longer existed.

The lesson reaches well beyond crypto: every constant in a risk model is an untested assumption. A peg is a market price with a strong prior, not a fact. Systems should price it live, from multiple venues, with a deviation threshold that halts trading and pages a human.

The desks that came through that weekend cleanly did not know more about SVB than anyone else. They just never trusted a number they had not measured.

Read the full analysis → https://siavashsed.github.io/cryptopulse/usdc-depeg-2023-trading-bots/

#AlgorithmicTrading #Stablecoins #RiskManagement #CryptoTrading #QuantFinance

---

## QUORA
**Answer this question:** How did the 2023 USDC depeg affect crypto trading bots?

The short version: it punished any bot that treated USDC as exactly $1.00 instead of as an asset with its own price.

Some background. On Friday, March 10, 2023, Silicon Valley Bank failed, and that evening Circle disclosed that about $3.3 billion of USDC reserves were held there. Over the weekend USDC traded as low as roughly $0.87 on some venues, and Curve's main stablecoin pool became heavily imbalanced as people swapped out of USDC. DAI fell with it because much of its backing was USDC. The peg recovered by Monday, March 13, after US regulators guaranteed SVB deposits.

For bots, the failure modes were predictable once you saw them:

1. Hardcoded par marking. Many systems valued USDC collateral at 1.00, so margin and PnL looked healthy while real value fell. Basis and carry bots were especially exposed because USDC was supposed to be the safe leg.

2. Quote currency drift. Grid and market-making bots quoting pairs in USDC were repricing every order in a falling unit without knowing it.

3. Single-source pricing. Bots that did read a price often read only one venue, and venues disagreed badly that weekend.

4. Weekend timing. Banks were closed, desks were thin, and most alerting was built for weekdays.

I hit the first one myself. A basis bot I had run for 14 months was marking its USDC at par while Curve quoted 0.96 and falling, and I shut it down by hand late that Friday night.

The fixes are simple: price stablecoins live from at least two independent sources, set a deviation threshold of 0.5 to 1 percent that halts new risk, and make sure off-hours alerts reach a person. I wrote up the full timeline and the checks I use now here: https://siavashsed.github.io/cryptopulse/usdc-depeg-2023-trading-bots/

The broader point is that a peg is a market price with a strong prior. It is not a constant.
