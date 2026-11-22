# Backlink content - Black Thursday 2020 Halved Bitcoin in a Day and Broke Every Lazy Bot
**URL:** https://siavashsed.github.io/cryptopulse/black-thursday-2020-crypto-bots/
**Generated:** 2026-11-22

---

## REDDIT
**Post to:** r/algotrading, r/CryptoCurrency, r/BitcoinMarkets
**Title:** What did your bots actually do on March 12, 2020? Mine failed in ways the price chart never showed

I was running a small market-making bot on BitMEX that morning, and Black Thursday taught me something I still think about. Bitcoin fell from roughly $7,900 to under $4,000 in about 24 hours, but the price drop wasn't what hurt most bots. The infrastructure behaving badly was.

Exchange APIs slowed down or timed out. Order acknowledgements arrived late or not at all, so bots didn't know their real position. Liquidation cascades pushed spreads far beyond anything in the backtests. Plenty of strategies assumed a working order book and a working API, and both assumptions broke at the same moment.

The bots that survived mostly had boring protections: hard position limits, kill switches that triggered on stale data, and logic that stopped quoting when latency spiked instead of trying to be clever. The ones that died were optimized for normal conditions and had no plan for the exchange itself being the failure point.

I'm curious how others handled it. Did your bot go flat, keep quoting, or get liquidated? And did you change anything structural afterward, or just add more margin?

I wrote up what I saw and what I'd build differently. Full breakdown here: https://siavashsed.github.io/cryptopulse/black-thursday-2020-crypto-bots/

---

## LINKEDIN
**Hook:** Bitcoin halved in a day in 2020, and the price was not what broke most trading bots.

On March 12, 2020, Bitcoin fell from roughly $7,900 to under $4,000 in about 24 hours. I was running a small market-making bot on BitMEX that morning, and I watched the plumbing fail in real time.

The real damage came from the machinery. APIs timed out, order confirmations went missing, and spreads blew out far past anything the backtests had modeled. Bots assumed a healthy exchange, and the exchange was the thing that failed.

The systems that survived were rarely the smartest. They had hard position limits, kill switches tied to stale data, and a willingness to stop quoting when conditions became unreliable.

The lesson applies well beyond crypto: automated systems should be designed around the failure of their dependencies, not just the movement of the market. Resilience is a feature you have to build before the bad day arrives.

Read the full analysis → https://siavashsed.github.io/cryptopulse/black-thursday-2020-crypto-bots/

#AlgorithmicTrading #Bitcoin #RiskManagement #QuantFinance #CryptoMarkets

---

## QUORA
**Answer this question:** Why did so many crypto trading bots fail during the March 2020 Black Thursday crash?

I was running a small market-making bot on BitMEX on March 12, 2020, so I saw this one from the inside. Bitcoin dropped from roughly $7,900 to under $4,000 in about a day, but the price move alone doesn't explain why so many bots failed. The bigger problem was that the infrastructure they depended on stopped behaving normally.

First, exchange APIs degraded. Requests timed out, order acknowledgements arrived late or never, and rate limits tightened just when bots needed to act. A bot that can't confirm its own orders doesn't actually know its position, and that's a dangerous place to be in a falling market.

Second, liquidity vanished. Backtests typically assume you can quote and exit at reasonable spreads. During the crash, order books thinned out and spreads widened dramatically, so stop-losses filled far worse than modeled, and liquidation cascades fed on themselves.

Third, most strategies were tuned for normal conditions. They had no concept of an exchange outage as a risk, only price risk.

The bots that made it through tended to have unglamorous protections: hard position limits, kill switches that fired on stale data or latency spikes, and logic that simply stopped quoting when conditions looked unreliable. Margin buffers helped too, but they only delay the problem if the logic underneath is fragile.

If you're building anything automated, I'd treat dependency failure as a first-class scenario in testing, not an edge case. Simulate dropped connections, delayed fills, and spreads ten times normal, and see what your system does.

I wrote a longer account of what I saw and what I'd change if you want more detail: https://siavashsed.github.io/cryptopulse/black-thursday-2020-crypto-bots/
