# Week 3 (30 Nov–6 Dec): Risk, expectancy and the trader's head

**Why this week exists:** this is the most important week of the course. A mediocre entry method with sound risk management survives. A brilliant one without it does not. Your first real trades of the course come at the end of this week, after Gate 1.

**Real money:** after Gate 1 is passed, swing trades at 0.5% risk (₹500), at most 2 open positions.

## Outcomes

- Size any position from the stop distance.
- Think of every trade in R (multiples of the amount risked).
- Compute expectancy and explain why win rate alone means nothing.
- Know your own risk of ruin under your own rules, from a simulation you wrote.
- Recognise the mental errors that break rules: revenge, fear of missing out, moving stops, averaging down.

## Day by day

| Day | Study | Do |
|---|---|---|
| Mon | Varsity Module 9, chapters on risk (start to position sizing). Van Tharp's idea of R-multiples: search "Van Tharp R multiple expectancy". | For your 3 paper ideas from week 2, compute quantity by rule R2 for ₹500 risk. |
| Tue | Expectancy = (win rate × average win in R) − (loss rate × average loss in R). Varsity Module 9, position-sizing chapters. | By hand: expectancy for (a) 40% wins at 3R, (b) 70% wins at 0.5R, (c) 90% wins at 0.2R with losers at 3R. Which would you trade? |
| Wed | Drawdown mathematics: a 10% loss needs 11% to recover, 30% needs 43%, 50% needs 100%. Risk of ruin. Search "risk of ruin trading explained". | Take your worst trade: what was it in R, if R had been 1% of capital? Write the number down. |
| Thu | Psychology: Varsity Module 9, trading-biases chapters. *Trading in the Zone*, the chapters on thinking in probabilities. | Write your personal "tilt list": five situations in which you have broken your own plan before, and what you will physically do when each one appears. |
| Fri | Read `00-context/rules.md` slowly. Mark any rule you disagree with and why. | Build the watchlist for next week: 10 Nifty 200 stocks in a weekly uptrend sitting near a daily support zone. |
| Sat | Lab 3. Gate 1 quiz with the mentor. | Concept answers. |
| Sun | Finish *Trading in the Zone* if possible. | Weekly review. If Gate 1 is passed: write 2 trade plans for Monday. |

## Lab 3: position sizer and Monte Carlo

Folder: `05-labs/lab03/`

1. `size.py`: inputs are capital, risk %, entry, stop. Output: quantity, position value, loss at stop, and a warning if the position exceeds 25% of capital.
2. `montecarlo.py`: simulate 1,000 traders, each taking 200 trades with a given win rate and reward-to-risk, risking a fixed % of current capital. Report the median outcome, the worst 5% outcome, and the proportion who ever hit a 10% drawdown and a 20% drawdown.
3. Run it for 1% risk and for 5% risk with the same edge (say 45% wins at 2R). Plot 50 sample equity curves for each.
4. Run it with a slightly negative edge. See how long it can look profitable.
5. Write in `notes.md`: with your rules, how likely is the 10% stop to be hit even if your system is good?

## Concept questions

Answers in `06-answers/week-03.md`.

1. Capital ₹1,00,000, risk 0.5%. Entry ₹842, stop ₹815. What quantity? What is the position value? What do you do if the quantity comes to a fraction?
2. Why should position size come from the stop distance and not from how confident you feel?
3. A system wins 35% of the time. Under what condition is it still worth trading?
4. A system wins 85% of the time. Under what condition will it still ruin you? Which popular options strategy has this profile?
5. You are down 6% for the month after four straight losses that all followed the rules. What does the rulebook say, and why is that the right response even if the next setup looks perfect?
6. Explain why a 50% loss is far worse than twice a 25% loss.
7. What is the difference between a bad trade and a losing trade?
8. Your stop is at ₹815 and price is at ₹817, falling. You feel the urge to move the stop to ₹805 "to give it room". What is really happening, and what does R3 say?
9. From your Monte Carlo: at 1% risk and a real edge, how often did a trader touch a 10% drawdown in 200 trades? What does that say about judging a system by ten trades?
10. Write your own definition of a successful month in a way that does not mention profit.

## Gate 1

Passed when all of these are true:

- [ ] Rules quiz with the mentor: 70% or more
- [ ] `size.py` works and you use it for a live example
- [ ] 10 or more predictions logged over weeks 1–3
- [ ] Rules accepted in writing in `00-context/decisions.md`
- [ ] Dedicated course account funded with ₹1,00,000

If the gate is not passed, week 4 proceeds on paper and the gate is retaken the following Saturday.

## Checkpoint

- [ ] Tilt list written
- [ ] Lab 3 pushed
- [ ] 10 answers pushed
- [ ] Watchlist of 10 built
- [ ] Gate 1 result recorded in `03-progress/tracker.md`
