# Week 8 (4–10 Jan): Option strategies and their real risk

*Draft. Tuned at the month-1 review.*

**Why this week exists:** you asked for strategies that make "less-risk profit": straddles, strangles, spreads. This week tests that phrase against numbers. Some of these strategies have limited risk. Some win often and occasionally lose many months of gains in a day. You need to know which is which before any real money goes near them.

**Real money:** swing system only. All strategies on paper.

## Outcomes

- Build, price and manage: bull call spread, bear put spread, credit spreads, iron condor, long and short straddle, long and short strangle.
- For each: maximum profit, maximum loss, break-evens, margin, Greeks, and the market view it expresses.
- Separate defined-risk from undefined-risk structures, and probability of profit from expectancy.
- Understand adjustment, and why "adjusting" often means adding risk.

## Study

| Days | Topic | Source |
|---|---|---|
| Mon | Debit spreads: bull call, bear put | Varsity Module 6, chapters 1–5 |
| Tue | Credit spreads and the iron condor | Varsity Module 6, credit spread chapters. Option Alpha: "iron condor" |
| Wed | Long straddle and strangle: buying volatility | Varsity Module 6, straddle and strangle chapters |
| Thu | Short straddle and strangle: selling volatility; tail risk; margin | Varsity Module 6, same chapters from the seller's side. tastylive: "short strangle risk". Natenberg, chapter on volatility spreads |
| Fri | Choosing a structure from view plus IV level; position sizing for options; expiry and event risk | Sensibull strategy builder. *In The Money* newsletter, any two issues |

## Practical

Paper trades on Sensibull virtual trading, each with a journal entry containing view, structure, max loss in rupees, Greeks at entry, exit plan:

1. Two debit spreads (one bullish, one bearish).
2. Two credit spreads.
3. One iron condor held to within two days of expiry.
4. One long straddle around a known event.
5. One short strangle **with** protective wings and one without. Compare margin, max loss and daily P&L swings.

For each, record daily P&L and what drove it (delta, theta or vega).

## Lab 8: strategy analyser and a short-volatility backtest

Folder: `05-labs/lab08/`

1. Extend the lab 6 plotter with your lab 7 pricer: show today's P&L curve as well as the expiry payoff, and the position Greeks.
2. For each strategy above, print max profit, max loss, break-evens and the reward-to-risk ratio.
3. Simple backtest of a weekly short strangle on Nifty using daily index data and your pricer with VIX as the volatility input: sell at a fixed distance, hold to expiry, no adjustments. Five years. Report win rate, average win, average loss, worst week, and the equity curve.
4. Repeat with wings (an iron condor). Compare the worst week and the overall expectancy.
5. Write in `notes.md`: what does "low risk" mean for each version?

State the limits of this backtest in your notes: model prices are not traded prices, and weekly expiry rules changed during the period.

## Concept questions

Answers in `06-answers/week-08.md`.

1. Bull call spread: buy 25,000 call at ₹180, sell 25,200 call at ₹95, lot 65. Max profit, max loss, break-even?
2. Why does a credit spread have a higher probability of profit than a debit spread on the same strikes in the opposite direction, and why does that not make it better?
3. An iron condor collects ₹40 on 100-point wings. Max loss per lot? How many winning weeks does one full loss erase?
4. When would you buy a straddle, and what has to happen for it to pay? Why do most long straddles before events lose?
5. A short strangle wins 85% of weeks in your backtest. What do the other 15% look like, and what does the worst one do to a ₹1 lakh account?
6. What is the practical difference in margin and in sleep between a short strangle and an iron condor?
7. "I will adjust if the market moves against me." What does an adjustment usually do to the position's risk?
8. Implied volatility is at its lowest level in a year. Which structures does that favour, and why?
9. With ₹1 lakh and a 1% risk rule, which of this week's structures can you size correctly at lot size 65? Show the arithmetic for one.
10. Now define "low-risk profit" for yourself: do you want a high win rate or a small maximum loss? What are you giving up with your choice?

## Gate 2

- [ ] Options exam with the mentor (payoffs, Greeks, strategy risk): 70% or more
- [ ] Your pricer reproduces market prices from your own IVs
- [ ] 8 paper trades journaled with Greeks
- [ ] Swing journal compliance at 90% or more for weeks 5–8
- [ ] Month-2 review written

## Checkpoint

- [ ] Lab 8 and answers pushed
- [ ] Gate 2 result recorded
