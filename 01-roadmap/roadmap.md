# Roadmap: 16 Nov 2026 – 7 Feb 2027

## The idea in one paragraph

Real money goes into one thing only: swing trades in liquid cash equities, at tiny size, with a written system. Everything else (futures, options, order flow) is learned deeply and practised on paper. Each week has four parts: study, screen time, a Python lab, and written answers. Three gates decide whether you move to the next month.

## Where the study material is

This page is the overview. The "Main sources" column names what each week is built on. The day-by-day assignments (which chapter, which video, which reading portion) are in each week file under `02-curriculum/`, and every link, channel, book and tool is listed in [`resources.md`](../resources.md).

Videos outside Zerodha Varsity are given as a channel name plus a search phrase, because only verified links are written down. At the start of each week the mentor checks and pins the exact video links for that week in the week file.

## Daily rhythm (about 2.5 hours)

| Block | Time | What |
|---|---|---|
| Study | 60–75 min, any time | The day's video or reading from the week file, with notes in your own words |
| Lab or answers | 30–45 min, any time | Python lab or written concept answers |
| Screen | 2:30–3:30 pm | Watch Nifty and your watchlist live. Write one prediction in `04-journal/prediction-log.md` at 2:30, check it at 3:30 |
| Journal | 10–15 min, evening | Update the trade journal, note one thing you saw today, commit and push |

Miss a day and you carry on from where you stopped. Miss three days in a row and you tell the mentor, who adjusts the plan.

## Weekly rhythm

- **Mon–Fri:** daily rhythm above.
- **Saturday (2 hours):** finish the lab, write remaining answers, push for evaluation.
- **Sunday (1 hour):** weekly review from the template, scan for next week's watchlist.

## Month 1: how markets and prices work

| Week | Dates | Theme | Main sources | Milestone |
|---|---|---|---|---|
| [1](../02-curriculum/week-01.md) | 16–22 Nov | Market mechanics: who trades, order types, how a price forms, costs | Varsity Module 1 (text + videos); Zerodha support pages on order types; broker brokerage calculator; *Trading in the Zone* | You can explain what happens between clicking buy and owning the share; TradingView set up on PC; first data pulled in Python |
| [2](../02-curriculum/week-02.md) | 23–29 Nov | Price structure: candles, trend, swings, support and resistance, multiple timeframes | Varsity Module 2 (candles, S&R, Dow theory) + Varsity TA videos; Rayner Teo; Murphy (reference) | 50 charts marked up by hand; a swing-detection script |
| [3](../02-curriculum/week-03.md) | 30 Nov–6 Dec | Risk and expectancy: position sizing, R-multiples, risk of ruin, psychology | Varsity Module 9; Van Tharp on R-multiples and expectancy; *Trading in the Zone* | Position-size calculator and a Monte Carlo of your rules; **Gate 1**; first real trades at 0.5% risk |
| [4](../02-curriculum/week-04.md) | 7–13 Dec | Building and testing a swing system: moving averages, volume, relative strength, backtesting | Varsity Module 2 (MA, volume, RSI/MACD); Varsity Module 10; Part Time Larry (backtesting in Python) | Swing system v1 written down and backtested with costs |

**Gate 1 (end of week 3):** rules quiz at 70% or more, position-size calculator working, two weeks of prediction log filled. Passing it unlocks real trades.

## Month 2: futures and options

| Week | Dates | Theme | Main sources | Milestone |
|---|---|---|---|---|
| [5](../02-curriculum/week-05.md) | 14–20 Dec | Futures: contracts, margin, mark-to-market, basis, rollover, leverage | Varsity Module 4; Khan Academy (futures margin); Natenberg, opening chapters | You can compute the P&L and margin of any futures position by hand |
| [6](../02-curriculum/week-06.md) | 21–27 Dec | Options foundations: payoffs, moneyness, intrinsic and time value, put-call parity, option chain | Varsity Module 5; projectfinance; Khan Academy (put-call parity); Natenberg; NSE and Sensibull option chain | Payoff plotter in Python; you can read an option chain |
| [7](../02-curriculum/week-07.md) | 28 Dec–3 Jan | Pricing and Greeks: Black-Scholes, implied volatility, delta, gamma, theta, vega | Varsity Module 5 (volatility, Black-Scholes, Greeks); MIT OCW 18.S096; projectfinance; Natenberg | Black-Scholes and an IV solver written by you, checked against live prices |
| [8](../02-curriculum/week-08.md) | 4–10 Jan | Strategies: vertical spreads, iron condor, straddle, strangle, and their real risk | Varsity Module 6; Option Alpha; tastylive; Natenberg (volatility spreads); Sensibull virtual trading | 8 paper trades logged with Greeks; **Gate 2** |

**Gate 2 (end of week 8):** options exam at 70% or more, your own pricer matches market prices within reason, paper-trade log complete, swing journal compliance at 90% or more.

## Month 3: auction, order flow, systematic work

| Week | Dates | Theme | Main sources | Milestone |
|---|---|---|---|---|
| [9](../02-curriculum/week-09.md) | 11–17 Jan | Auction market theory, volume profile, VWAP | Dalton, *Mind Over Markets*; Trader Dale (volume profile); GoCharting education | Volume profile built in Python from intraday data; 5 days profiled by hand |
| [10](../02-curriculum/week-10.md) | 18–24 Jan | Order flow: order book, tape, footprint, delta, absorption | Harris, *Trading and Exchanges* (reference); GoCharting order flow course; Trader Dale; Axia Futures | 10 annotated closing-hour sessions |
| [11](../02-curriculum/week-11.md) | 25–31 Jan | Systematic trading: honest backtesting, walk-forward, broker API, automated scan | Aronson and Chan (reference chapters); Varsity Module 10; QuantInsti; broker API docs (Fyers) | A daily scanner that produces your watchlist by itself |
| [12](../02-curriculum/week-12.md) | 1–7 Feb | Capstone: playbook, three-month review, next 90 days | Your own journal, labs and notes. No new material | **Gate 3**: playbook written, journal statistics computed, specialisation chosen |

## What real money does across the 12 weeks

| Weeks | Real money | Paper |
|---|---|---|
| 1–2 | No new trades. Existing holdings untouched. | Daily prediction log; paper swing picks |
| 3–4 | Swing trades, 0.5% risk, max 2 positions (after Gate 1) | Same |
| 5–8 | Swing trades, 1% risk if compliance is 90%+, max 3 positions | Futures and options strategies |
| 9–12 | Same swing system; no new styles with real money | Order-flow observation, system signals |

## What "done" looks like on 7 Feb 2027

1. A written playbook: your setups, entry, stop, exit, sizing, when not to trade.
2. A journal of at least 15 real swing trades with statistics: win rate, average R, expectancy, rule violations.
3. A backtester and a scanner you wrote and understand.
4. A Black-Scholes pricer you wrote, and the ability to explain any option strategy's risk in numbers.
5. A first working read of volume profile and order flow.
6. A decision, backed by your own data, on what to specialise in next.

Profit is not on this list. A small loss with full rule compliance is a pass. A profit made by breaking rules is a fail.
