# Week 1 (16–22 Nov): Market mechanics

**Why this week exists:** your worst loss came from not knowing what the market could do to you mechanically (a circuit lock on a short). Before reading a single chart, you should know exactly how an order becomes a trade and what can stop you from getting out.

**Real money:** no new trades this week.

## Outcomes

By Sunday you can:

- Explain how a price is formed from bids and offers.
- Choose the right order type for a situation and say what can go wrong with each.
- Compute the full cost of a round-trip trade.
- Explain circuit limits, auctions and why short-selling in cash is intraday only.
- Pull daily price data in Python and plot it.

## Day by day

| Day | Study (60–75 min) | Do (30–45 min) |
|---|---|---|
| Mon | Varsity Module 1, chapters 1–5 (the market, regulators, intermediaries, IPO basics). Watch the matching videos in the Varsity "Introduction to Stock Market" video module. | Set up TradingView (or Kite web) on PC: one layout, daily and 15-minute charts, a watchlist of Nifty 50 index, Bank Nifty and 10 Nifty stocks you know. |
| Tue | Varsity Module 1, chapters 6–10 (the stock market, indices, commonly used jargon, the trading terminal, clearing and settlement). | Open the market depth window of a liquid stock and an illiquid one at 2:30. Write down bid, ask, spread and the top-5 quantities for both. |
| Wed | Order types: market, limit, stop-loss (SL and SL-M), GTT, bracket. Read Zerodha's support pages for each, then place nothing; just open each order window and read every field. | Write a one-page note: "Which order type when, and how each can hurt me." |
| Thu | Circuits, price bands, the short-delivery auction, T+1 settlement, why F&O stocks have no fixed band. Search: "NSE price bands", "short delivery auction penalty". | Rewrite the story of your worst trade as a sequence of mechanical events: what you did, what the exchange rules did, where exit became impossible. |
| Fri | Costs: brokerage, STT, exchange charges, GST, stamp duty, DP charges, slippage. Use any broker's brokerage calculator. | Compute the round-trip cost of a ₹20,000 delivery trade and a ₹20,000 intraday trade. Express both as a percentage. |
| Sat | Lab 1 (below). | Concept answers. |
| Sun | *Trading in the Zone*: start, 15 pages. | Weekly review. |

Every weekday at 2:30 pm: write one prediction for Nifty's 3:30 close relative to its 2:30 price (up, down, flat within 0.1%) and one sentence of reasoning. At 3:30 record the result. No chart knowledge is expected yet; the habit is the point.

## Lab 1: first data

Folder: `05-labs/lab01/`

1. Create a virtual environment and install `pandas`, `matplotlib`, `yfinance`.
2. Download five years of daily data for `^NSEI` (Nifty 50) and five Nifty stocks of your choice. Save each as CSV.
3. Plot closing prices. Then compute daily percentage returns and plot their histogram.
4. Print for each: average daily return, standard deviation of daily returns, the worst single day, the worst peak-to-trough fall (drawdown).
5. Write three sentences in `05-labs/lab01/notes.md` on anything that surprised you.

Rule for all labs: you may use AI to help write code, but you must be able to explain every line when asked.

## Concept questions

Write answers in `06-answers/week-01.md`. Two to six sentences each, in your own words.

1. A stock shows bid ₹499.80 × 200 and ask ₹500.20 × 150. You send a market order to buy 400 shares. Describe what happens and at what prices you might be filled.
2. What is the difference between an SL order and an SL-M order? Give one situation where each fails you.
3. Why can a stop-loss order not protect you in a stock locked in upper circuit when you are short?
4. You short a stock intraday and cannot buy it back by the close. Walk through what happens over the next days and who decides your loss.
5. Why do stocks in the F&O segment not have fixed 5%, 10% or 20% price bands, and what protects the market there instead?
6. Your round-trip cost on a swing trade is 0.25%. Your average winning trade makes 4% and your average loser loses 2%, with half your trades winning. What does cost do to your expectancy per trade?
7. What is slippage, and in which kind of stock and at which time of day is it worst?
8. A stock's average daily return is 0.05% and the standard deviation of daily returns is 1.8%. What does that tell you about how much of any single day's move is signal?
9. What does "liquidity" mean in practice for someone trading ₹20,000 positions, and for someone trading ₹2 crore?
10. In one paragraph: what rule, existing before the trade, would have prevented your worst loss?

## Checkpoint

- [ ] Charting set up on PC with a saved layout
- [ ] Order-type note written
- [ ] Cost calculation done
- [ ] Lab 1 pushed
- [ ] 10 answers pushed for evaluation
- [ ] 5 predictions logged
- [ ] Weekly review written
