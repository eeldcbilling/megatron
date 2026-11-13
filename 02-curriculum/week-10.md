# Week 10 (18–24 Jan): Order flow

*Draft. Tuned at the month-2 review.*

**Why this week exists:** you asked for order flow as a tool. This is an honest first pass: enough to read a footprint and the tape during the closing hour and to know what it can and cannot tell you. Fluency takes months of screen time beyond this course.

**Real money:** swing system only. Order flow is observation only.

**Tool decision this week:** a charting plan with footprint and cumulative delta (GoCharting's paid India plan was listed around ₹1,495 a month in November 2026). Take it for one month only, and only if weeks 1–9 are on track.

## Outcomes

- Explain the order book, market versus limit orders, and who "takes" and who "provides" liquidity.
- Read time and sales, a footprint chart, bid-ask imbalance, delta and cumulative delta.
- Recognise absorption, exhaustion and a failed auction on a replay.
- State clearly why order flow is a timing tool at a level you already care about, not a signal by itself.

## Study

| Days | Topic | Source |
|---|---|---|
| Mon | Market microstructure: the book, queue priority, aggressive and passive orders | Harris, *Trading and Exchanges*, chapters on orders and order-driven markets (reference reading). GoCharting free order flow course, first videos |
| Tue | Tape and footprint: volume at bid and at ask, imbalance | GoCharting course, footprint videos. Trader Dale: "order flow footprint" |
| Wed | Delta and cumulative delta; divergence between price and delta | Axia Futures: "cumulative delta", "footprint" |
| Thu | Absorption, exhaustion, stop runs, icebergs | Axia Futures: "absorption". Jigsaw Trading: "order flow basics" |
| Fri | Putting it together: level from profile, trigger from order flow | Your own replays |

## Practical

- Use bar replay on Nifty futures for the closing hour of 10 past sessions. For each, write: the level that mattered (from profile or VWAP), what the footprint showed there, what happened next.
- Live, 2:30–3:30, all five days: watch one instrument only. Write three observations per session. No trades, not even paper.
- Collect five screenshots of absorption and five of exhaustion, annotated.

## Lab 10: delta from ticks

Folder: `05-labs/lab10/`

1. Record live ticks for Nifty futures over a broker WebSocket (Fyers) for two closing hours: time, last price, quantity, best bid, best ask.
2. Classify each trade as buyer- or seller-initiated by comparing the trade price with the bid and ask at that moment.
3. Build delta per 5-minute bar and cumulative delta for the session. Plot against price.
4. Build a small footprint table for one 5-minute bar: volume at bid and at ask for each price.
5. Note in `notes.md` how the broker feed differs from true tick-by-tick data (snapshots several times a second, not every trade) and what that does to your delta.

## Concept questions

Answers in `06-answers/week-10.md`.

1. Every trade has a buyer and a seller. What, then, does "more buying than selling" mean in order flow?
2. What is delta for a bar? What is cumulative delta?
3. Price makes a new high but cumulative delta does not. Give two different explanations.
4. Describe absorption in terms of aggressive and passive orders. Why might it mark a turn, and why might it not?
5. What is a stop run, and how would it look on a footprint?
6. Why is order flow more reliable in index futures than in a mid-cap stock?
7. Your broker feed sends snapshots, not every trade. What kind of error does that introduce into your delta?
8. Why should order flow be read at a pre-chosen level and not continuously?
9. Large resting orders appear in the book and vanish as price approaches. What is this, and what does it teach about trusting the visible book?
10. After this week: would order flow improve your swing entries, or is it a different trade altogether? Give your honest view.

## Checkpoint

- [ ] 10 replay sessions written up
- [ ] 5 live observation sessions
- [ ] 10 annotated screenshots
- [ ] Lab 10 and answers pushed
