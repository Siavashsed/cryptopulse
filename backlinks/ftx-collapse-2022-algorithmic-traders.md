# Backlink content - The FTX Collapse of November 2022: What Algorithmic Traders Actually Lost (And Learned)
**URL:** https://siavashsed.github.io/cryptopulse/ftx-collapse-2022-algorithmic-traders/
**Generated:** 2026-05-31

---

## REDDIT
**Post to:** r/algotrading, r/CryptoCurrency, r/investing
**Title:** Lost $2M in automated strategies when FTX collapsed? Here's what actually happened in those 72 hours

I've been digging into the FTX collapse timeline from a trading systems perspective, and the infrastructure failure was way worse than most people realize. If you had market-making bots or arbitrage strategies running on their API on November 8th, you didn't just lose positions—your entire automation stack became a liability.

A trader I know had three bots running fine at 6am. By 9am, his withdrawal requests hung indefinitely. By noon, everything was gone. The real lesson isn't about picking better exchanges—it's about the architectural risk of centralized liquidity, position concentration, and having proper circuit breakers on your automation.

I wrote a technical breakdown looking at what actually happened to algorithmic traders during those 72 hours, what positions got liquidated, and more importantly, what safeguards should've been in place. Full breakdown here: https://siavashsed.github.io/cryptopulse/ftx-collapse-2022-algorithmic-traders/

---

## LINKEDIN
**Hook:** FTX collapsed in 72 hours, and algorithmic traders lost more than money—they lost visibility into their own systems.

November 2022 exposed a critical vulnerability in crypto trading infrastructure: centralized risk concentration.

When FTX filed for bankruptcy, automated strategies didn't just experience drawdowns—they experienced total infrastructure failure. Traders couldn't access positions, withdrawals hung indefinitely, and API connections became unreliable within hours.

The algorithmic trading community learned three hard lessons: first, position concentration on a single exchange creates systemic risk that no risk model can hedge. Second, circuit breakers and real-time exchange health monitoring should be non-negotiable for any bot. Third, decentralized alternatives aren't just ideological—they're architectural necessities.

The traders who survived November 8th weren't the smartest—they were the ones with proper position sizing rules, multi-exchange strategies, and the discipline to pull liquidity when signals broke. Read the full analysis → https://siavashsed.github.io/cryptopulse/ftx-collapse-2022-algorithmic-traders/

#algotrading #cryptocurrency #riskmanagement #trading #fintech

---

## QUORA
**Answer this question:** What happened to algorithmic traders who had active bots running on FTX when it collapsed in November 2022?

The FTX collapse was particularly devastating for algorithmic traders because it wasn't a gradual market decline—it was infrastructure failure compressed into 72 hours.

Traders with active bots experienced a cascading failure: first, API latency spiked dramatically. Then withdrawal requests began hanging. By midday on November 8th, many automated strategies simply couldn't execute or close positions. Market-making bots that were profitable at 6am became insolvent by noon because they couldn't access their collateral or hedge their positions.

The real damage came from position concentration. Most algorithmic traders, especially smaller prop desks, don't diversify across multiple exchanges—they build their strategies around one or two platforms for latency and liquidity advantages. When FTX's infrastructure collapsed, those traders had nowhere to move their capital and no way to manage risk.

Financial losses ranged from six figures for smaller operations to several million for firms with significant FTX exposure. But the less-discussed losses were operational: teams spent weeks trying to recover data, prove their holdings to creditors, and rebuild their systems on alternative exchanges.

The survivors implemented three critical changes: automated circuit breakers that liquidate positions if exchange connectivity becomes unreliable, position limits per exchange, and real-time exchange health monitoring integrated directly into their trading systems. I've documented the technical details and specific strategies that worked during this period in a detailed analysis of what went wrong and what traders actually learned from it.
