# Backlink content - Volatility Targeting Keeps Crypto Risk Steady, Until the Gap Hits
**URL:** https://siavashsed.github.io/cryptopulse/volatility-targeting-crypto-portfolios/
**Generated:** 2026-11-18

---

## REDDIT
**Post to:** r/algotrading, r/BitcoinMarkets, r/CryptoMarkets
**Title:** Volatility targeting averages your crypto risk. It doesn't cap it. How do you handle the gap?

Something I keep seeing in systematic crypto setups is that people treat volatility targeting as a risk cap. It isn't one. It's closer to a risk average.

The mechanics are simple. You pick a target (say 50% annualized), estimate realized vol over some lookback, and scale exposure by target divided by estimate. When vol rises you shrink, and when it falls you grow. Over months it does a good job of keeping the ride smooth.

The problem is that the estimate always looks backward. A calm stretch pushes your sizing up right before the market gaps, and the de-risking only happens after the move is already in your P&L. May 19, 2021 was the textbook case. BTC and ETH dropped hard intraday, and any vol-scaled book was sized for the quiet week before it.

Three things helped me: a hard leverage ceiling no matter what the formula says, blending a short and a long lookback so the estimate reacts faster, and treating weekends and thin liquidity windows as higher vol than the data claims.

How do others handle this? Do you cap leverage separately or trust the scaler?

Full breakdown here: https://siavashsed.github.io/cryptopulse/volatility-targeting-crypto-portfolios/

---

## LINKEDIN
**Hook:** Volatility targeting does not cap your crypto risk. It averages it, and the gap is where it fails.

Volatility targeting sizes a portfolio so it runs at a fixed level of expected risk. When vol rises, you cut exposure. When it falls, you add it back. On paper it is one of the cleanest risk tools in systematic trading.

The catch is that every estimate looks backward. A calm stretch pushes sizing up, and that is exactly the position you are holding when the market gaps. The scaler cuts after the loss, not before it.

I learned this running a 50% annualized vol target on a BTC and ETH sleeve through May 19, 2021. The model did what it was built to do. What it was built to do was the problem.

What I would add to any version: a hard leverage ceiling that ignores the formula, a blended short and long lookback, and a liquidity haircut for weekends and thin sessions.

Read the full analysis → https://siavashsed.github.io/cryptopulse/volatility-targeting-crypto-portfolios/

#AlgorithmicTrading #QuantitativeFinance #CryptoTrading #RiskManagement #Bitcoin

---

## QUORA
**Answer this question:** How does volatility targeting work for a crypto portfolio, and does it actually protect against crashes?

Short answer: it works well for keeping average risk steady, but it does not reliably protect you from a sudden crash. Those are two different jobs.

How it works: you choose a target level of annualized volatility for the portfolio, for example 50% for a BTC and ETH sleeve. You estimate current realized volatility, usually from a rolling window of daily or intraday returns. Your exposure is the target divided by the estimate. If realized vol doubles, you hold half the position. If it halves, you can size up, often with leverage.

Why it helps: crypto volatility clusters, so turbulent weeks tend to follow turbulent weeks. Scaling down after vol rises removes a lot of exposure during the worst stretches. Over a full cycle this usually smooths the equity curve and improves risk-adjusted returns compared with holding a fixed size.

Where it breaks: the estimate always looks backward. After a quiet period your model reads low vol and pushes you to your largest position, which is the worst place to be going into a gap. I ran a 50% target on BTC and ETH through May 19, 2021, and the de-risking arrived after the drop, not before it. I wrote up that episode and what I changed afterward here: https://siavashsed.github.io/cryptopulse/volatility-targeting-crypto-portfolios/

What I would add to any implementation:

1. A hard leverage cap that ignores the formula.
2. A blend of short and long lookbacks, so the estimate reacts faster without getting too noisy.
3. A floor on estimated vol, so a calm market cannot convince you that risk has gone away.
4. Extra caution around weekends and thin liquidity, when gaps are most likely.

Treat volatility targeting as a way to size positions, not as a stop loss. It controls how much risk you take on average, but it cannot see a gap before it happens.

Marcus Webb
