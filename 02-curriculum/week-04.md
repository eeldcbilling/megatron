# Week 4 (7–13 Dec): A swing system you can test

**Why this week exists:** until now you have traded by look and by recommendation. This week you write down one setup precisely enough that a program can trade it, then find out what it would have done. This is where the computer science background starts paying.

**Real money:** swing trades at 0.5% risk, at most 2 positions, only from the written system.

## Outcomes

- Understand moving averages, volume and relative strength as measurements, with their lag and their limits.
- Write a complete system: universe, setup, trigger, stop, exit, size.
- Backtest it with costs and without looking into the future.
- Know the main ways a backtest lies.

## Day by day

| Day | Study | Do |
|---|---|---|
| Mon | Moving averages: Varsity Module 2, MA chapter. What an EMA is mathematically, why it lags, why crossovers whipsaw in ranges. | On 10 charts: where did the 20/50 EMA help, and where did it give a signal after the move was over? |
| Tue | Volume: Varsity Module 2, volume chapter. Volume on breakouts and on pullbacks. | 10 breakouts from the last year: compare the breakout day's volume to its 20-day average. Which ones followed through? |
| Wed | Relative strength versus the index (not RSI): a stock rising more than Nifty over 3 and 6 months. Search "relative strength stock selection Minervini" or "O'Neil relative strength". Then RSI and MACD from Varsity, briefly, as descriptions of momentum. | Rank your 10 watchlist stocks by 3-month return minus Nifty's. |
| Thu | System design: Varsity Module 10, first chapters. What a complete system must specify. | Write **Swing System v1** in `04-journal/system-v1.md` using the template below. |
| Fri | Backtesting pitfalls: look-ahead bias, survivorship bias, overfitting, ignoring costs. Search "backtesting pitfalls look-ahead bias survivorship". Part Time Larry: "backtesting python". | Start lab 4. |
| Sat | Lab 4. | Concept answers. |
| Sun | Month-1 review with the mentor. | Weekly review plus month review. |

### Swing System v1 template

A starting point to edit, not a recommendation. You must be able to defend every line.

- **Universe:** Nifty 200 stocks.
- **Trend filter:** close above the 50-day EMA, and the 50-day EMA above the 200-day EMA.
- **Strength filter:** 3-month return greater than Nifty's.
- **Setup:** pullback to within 2% of the 20-day EMA.
- **Trigger:** a daily close above the previous day's high.
- **Entry:** next day's open (so the backtest cannot cheat).
- **Stop:** below the pullback's swing low.
- **Exit:** at 2R, or a close below the 20-day EMA, whichever comes first.
- **Size:** rule R2.
- **Do not trade when:** Nifty is below its 50-day EMA.

## Lab 4: an honest backtest

Folder: `05-labs/lab04/`

1. Code System v1 for 20–30 stocks over five years of daily data. Plain pandas loops are fine; clarity beats speed.
2. Signals are computed on day T's close, orders fill at day T+1's open. Subtract 0.25% per round trip for costs.
3. Output a trade list (entry date, exit date, R result) and these statistics: number of trades, win rate, average win and loss in R, expectancy in R, largest drawdown in R, longest losing streak.
4. Change one parameter (say the EMA length from 20 to 15 and 25). If the results swing wildly, write down what that suggests.
5. Split the data: design on the first three years, then run once on the last two. Compare.
6. Write in `notes.md`: is there evidence of an edge, and how much would you trust it?

Known weakness to state honestly in your notes: testing on today's index members only is survivorship bias.

## Concept questions

Answers in `06-answers/week-04.md`.

1. Why does every moving average lag, and why can no parameter choice remove the lag without adding noise?
2. In what market condition do moving-average crossovers lose money steadily, and how does your system try to avoid that condition?
3. What is the difference between relative strength against an index and the RSI indicator?
4. Why must a backtest enter on the next bar's open and not on the signal bar's close?
5. Your backtest uses today's Nifty 200 members for the last five years. What bias is this, and in which direction does it distort results?
6. You try 40 parameter combinations and pick the best. Why is its backtest result almost certainly too good?
7. Your system shows 42% wins and +0.35R expectancy over 180 trades. Roughly how many trades would you want before believing it, and why?
8. Why is a system with fewer rules usually more trustworthy than one with many?
9. What should make you stop trading System v1 with real money? State it as a rule with numbers.
10. Which single line of System v1 are you least sure about, and how would you test it?

## Checkpoint

- [ ] System v1 written and committed
- [ ] Lab 4 pushed with statistics
- [ ] 10 answers pushed
- [ ] Any real trades journaled before entry
- [ ] Month-1 review written in `03-progress/reviews/`
