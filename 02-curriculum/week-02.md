# Week 2 (23–29 Nov): Price structure

**Why this week exists:** you already draw EMAs and support/resistance, by your own account not well. This week strips charts back to the raw material, price and time, and rebuilds the reading from there. Indicators come in week 4.

**Real money:** no new trades this week.

## Outcomes

- Read a candle as a record of a fight, not as a named pattern.
- Mark swing highs and lows and classify a chart as uptrend, downtrend or range by a rule.
- Draw support and resistance as zones and explain why they exist.
- Use a higher timeframe for direction and a lower one for timing.

## Day by day

| Day | Study | Do |
|---|---|---|
| Mon | Varsity Module 2, chapters 1–4 (what TA is, chart types, candlesticks intro). Varsity TA video series, videos 1–5. | On 5 daily charts, cover the right half of the screen, describe each of the last 10 visible candles in words (who won, where, how decisively), then reveal. |
| Tue | Varsity Module 2, single and multiple candlestick patterns (chapters 5–10). Read them as examples of one idea: rejection or acceptance of a price. | Find 10 examples of a long-wick rejection on daily charts. For each, note what happened in the next 5 days. Count how often it "worked". |
| Wed | Trend and swings. Rayner Teo: search "market structure" and "how to identify trend". Murphy, chapter on trend basics (reference). | Mark swing highs and lows on 10 daily charts by hand using one rule: a swing high is a high with two lower highs on each side. Label each chart up, down or range. |
| Thu | Support and resistance. Varsity Module 2 chapter on S&R; Rayner Teo "support and resistance". | Mark S&R zones on the same 10 charts. Write for each zone why traders would act there (trapped buyers, prior breakout level, round number). |
| Fri | Multiple timeframes and Dow theory. Varsity Module 2, Dow theory chapters. | For 5 stocks: weekly chart gives the trend, daily chart gives the location. Write one line each: "Weekly is X, daily is at Y, so I would look for Z." |
| Sat | Lab 2. | Concept answers. |
| Sun | *Trading in the Zone*, continue. | Weekly review. 20 more chart mark-ups to reach 50 for the week. |

2:30 prediction log continues. From this week, add the reason in structural terms (trend, level, last hour's swings).

Holdings: on Saturday, do step 3 of `04-journal/holdings-review.md`, replacing the interim floors with levels from the weekly charts.

Paper picks: by Friday, write 3 paper swing ideas in the journal with entry, stop and target. They are graded on reasoning, not outcome.

## Lab 2: swings and trend by rule

Folder: `05-labs/lab02/`

1. Write a function that finds swing highs and swing lows in a daily series (N bars on each side, N as a parameter).
2. Write a function that labels each date as uptrend (higher highs and higher lows), downtrend, or range, from the last two swing highs and lows.
3. Plot price with swings marked and the background shaded by trend label.
4. Compare the script's labels with your hand labels on 5 charts. Where do they differ, and who is right?
5. Stretch: find horizontal levels touched by at least three swings within a tolerance.

The important catch to discover: a swing high is only confirmed N bars later. Note where your code might be using information that was not available on that day.

## Concept questions

Answers in `06-answers/week-02.md`.

1. What four prices make a candle, and what do the body and the wicks each say about the session?
2. Two candles close at the same price. One has a long lower wick, the other a long upper wick. What happened differently during those sessions?
3. Define an uptrend by rule. At what exact event do you stop calling it an uptrend?
4. Why is support better drawn as a zone than as a line?
5. Give two reasons, based on what traders are holding and feeling, why broken resistance often acts as support afterwards.
6. A stock is in a weekly uptrend and a daily downtrend. Describe the two ways this can resolve and what you would wait to see.
7. Your count of the long-wick rejection: how many of 10 "worked"? What does that number tell you about trading a pattern alone?
8. What is the difference between a breakout and a false breakout at the moment it happens? Can you know which it is?
9. In lab 2, a swing high is confirmed N bars late. Why does this matter for backtesting?
10. Why does a level that everyone can see sometimes fail precisely because everyone can see it?

## Checkpoint

- [ ] 50 charts marked up (screenshots or a list of symbols with labels in `04-journal/`)
- [ ] Lab 2 pushed
- [ ] 10 answers pushed
- [ ] 3 paper swing ideas written
- [ ] Holdings review step 3 done
- [ ] 5 predictions logged
- [ ] Weekly review written
