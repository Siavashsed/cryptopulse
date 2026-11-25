# Backlink content - Funding Rates Quietly Cost Me $1,900 in One Week
**URL:** https://siavashsed.github.io/cryptopulse/funding-rates-futures-traders-cost-signal/
**Generated:** 2026-11-25

---

## REDDIT
**Post to:** r/CryptoCurrency, r/algotrading, r/ethtrader
**Title:** Funding rates cost me $1,900 in a week on a flat ETH position. How do you budget for them?

Back in March 2024 I held a roughly $120k ETH long on Binance perps. Price barely moved all week, so I assumed I'd finish close to flat. I didn't. Funding averaged around 0.075% per eight hours, and when I added it up I was down about $1,900 on a trade that went nowhere.

The maths is simple once you write it down. Funding is paid three times a day, so 0.075% on $120k is about $90 per payment, or roughly $270 a day. Over a week that's the whole loss. I'd been treating funding as background noise when it was really a carrying cost, like margin interest.

A few things I changed afterwards:

- I check the current and predicted funding rate before sizing any position I plan to hold more than a day.
- I treat persistently high funding as a crowding signal, not only a cost. When everyone is long and paying to stay long, the trade is usually stretched.
- For longer holds I compare perps against dated futures or spot.

Curious how others handle this. Do you set a funding threshold where you close or hedge, or just accept it as the price of leverage?

Full breakdown here: https://siavashsed.github.io/cryptopulse/funding-rates-futures-traders-cost-signal/

---

## LINKEDIN
**Hook:** A flat trade lost me $1,900 in a week, and price had nothing to do with it.

In March 2024 I held a roughly $120,000 ETH long on Binance perpetuals. Price barely moved. My account still dropped about $1,900.

The cause was funding. Longs and shorts exchange payments every eight hours to keep a perpetual contract anchored to spot. With the rate averaging around 0.075% per interval, I was paying close to $270 a day without noticing.

As a former quant trader, I should have modelled it from the start. Funding is a carrying cost, and it deserves the same line in a trade plan as fees and slippage.

The second lesson mattered more. A persistently hot funding rate tells you the market is crowded on one side. It works as a sentiment signal as well as an expense, and I now read it before I size a position.

Read the full analysis → https://siavashsed.github.io/cryptopulse/funding-rates-futures-traders-cost-signal/

#CryptoTrading #AlgorithmicTrading #Derivatives #RiskManagement #Ethereum

---

## QUORA
**Answer this question:** How do funding rates on crypto perpetual futures work, and how much can they cost a trader?

A perpetual futures contract has no expiry, so exchanges need another way to keep its price close to the spot price. That mechanism is the funding rate. Every eight hours on most major exchanges, traders on one side of the market pay traders on the other. When the perpetual trades above spot, longs pay shorts. When it trades below, shorts pay longs. The payment is the funding rate multiplied by your position size, not your margin.

That last point is where people get caught. The rate looks tiny, often 0.01% per interval, which is the common baseline. But it applies to the full notional value and is charged three times a day. In a strong bull run the rate can climb several times higher.

I learned this the expensive way in March 2024. I held a roughly $120,000 ETH long on Binance. Price barely moved all week, yet funding averaged around 0.075% per eight hours. That is about $90 per payment, roughly $270 a day, and it added up to around $1,900 for the week on a trade that went nowhere.

Practical takeaways:

1. Check the current and predicted rate before opening any position you plan to hold overnight.
2. Multiply the rate by three, then by your notional, to get a daily cost.
3. Treat unusually high funding as a warning that the trade is crowded. It often shows up before sharp reversals.
4. For longer holds, consider spot, dated futures, or a hedged structure.

Short sellers can earn funding when the market is long-heavy, which is why some funds run delta-neutral carry strategies. If you want the full walkthrough of my own numbers, I wrote it up here: https://siavashsed.github.io/cryptopulse/funding-rates-futures-traders-cost-signal/

The short version: funding is a real cost of leverage, so budget for it.
