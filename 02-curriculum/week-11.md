# Week 11 (25–31 Jan): Systematic trading

*Draft. Tuned at the month-2 review.*

**Why this week exists:** this is the part you said fascinates you most. You have a system, a backtester and ten weeks of live results. This week makes the testing more honest and automates the daily routine, so the computer does the scanning and you do the deciding.

**Real money:** swing system only. Nothing places orders automatically.

## Outcomes

- Know the standard defences against a lying backtest: out-of-sample testing, walk-forward, parameter stability, realistic costs.
- Compare your live journal with what the backtest said should happen.
- Fetch data from a broker API and run a daily scan without manual work.
- Understand, at a high level, the rules for retail algo trading in India and why you are not automating orders yet.

## Study

| Days | Topic | Source |
|---|---|---|
| Mon | What a backtest can and cannot prove; data-mining bias | Aronson, *Evidence-Based Technical Analysis*, the chapters on data mining (reference). Chan, *Quantitative Trading*, backtesting chapter |
| Tue | Walk-forward analysis and out-of-sample testing | Varsity Module 10. Search "walk forward analysis explained". QuantInsti: "walk forward optimization" |
| Wed | Metrics: expectancy, Sharpe ratio, maximum drawdown, profit factor, and what each hides | Part Time Larry or freeCodeCamp "Algorithmic Trading Using Python", metrics sections |
| Thu | Broker APIs: authentication, historical data, rate limits | Fyers API documentation (free data). Kite Connect documentation for comparison |
| Fri | The retail algo framework in India: static IP, order limits, what counts as an algo | Your broker's support pages on the SEBI retail algo rules |

## Practical

- Compute statistics from your real swing journal: trades, win rate, average R, expectancy, violations. Put them next to the lab 4 backtest numbers.
- Write a paragraph on every difference larger than you expected, and whether the cause was the market, the system or you.

## Lab 11: scanner and walk-forward

Folder: `05-labs/lab11/`

1. Refactor the lab 4 backtester into functions: data, signals, execution, statistics. Add a few tests for the pieces most likely to hide look-ahead errors.
2. Walk-forward: choose parameters on years 1–2, test on year 3; roll forward a year; repeat. Report the out-of-sample results only.
3. Daily scanner: after the close, pull data for the Nifty 200, apply System v1 filters, and write tomorrow's candidates with entry, stop and quantity to `04-journal/scans/YYYY-MM-DD.md`.
4. Schedule it (Task Scheduler or cron) on one machine. It commits and pushes the file.
5. Optional: a message to your phone when the scan finds something.

## Concept questions

Answers in `06-answers/week-11.md`.

1. Why is an out-of-sample test only valid the first time you look at it?
2. Describe walk-forward analysis and what it protects against.
3. Your system's Sharpe ratio is 1.4 in backtest. Name three things that will reduce it in live trading.
4. A strategy's results collapse when a parameter moves from 20 to 22. What do you conclude?
5. Your live win rate is 10 points below the backtest after 18 trades. Is the system broken? How would you decide?
6. What is profit factor, and what does it fail to show?
7. Why is a scanner that proposes trades safer for you right now than a bot that places them?
8. What does the static-IP requirement apply to, and what does it not apply to?
9. What data problem makes backtesting an options strategy much harder than a stock strategy?
10. If you had to bet on one source of edge for yourself over the next three years (selection, timing, risk management, automation), which, and what evidence from these eleven weeks supports it?

## Checkpoint

- [ ] Journal statistics versus backtest written up
- [ ] Walk-forward results pushed
- [ ] Scanner running on a schedule
- [ ] Answers pushed
