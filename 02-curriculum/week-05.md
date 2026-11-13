# Week 5 (14–20 Dec): Futures

*Draft. Day-level detail is tuned at the month-1 review, based on how weeks 1–4 went.*

**Why this week exists:** futures are the simplest derivative and the cleanest lesson in leverage. Options make no sense without them.

**Real money:** swing system only; 1% risk if journal compliance is 90% or better, otherwise stay at 0.5%. Futures on paper only.

## Outcomes

- Explain a futures contract: lot, expiry, margin, mark-to-market, settlement.
- Compute P&L, leverage and margin for any position by hand.
- Explain basis, cost of carry, premium and discount, rollover.
- See why one Nifty lot is too large for ₹1 lakh of capital under your rules.

## Study

| Days | Topic | Source |
|---|---|---|
| Mon–Tue | Forwards to futures, contract specifications, margin and mark-to-market | Varsity Module 4, chapters 1–6. Khan Academy: "futures margin mechanics" |
| Wed | Leverage and payoff, shorting with futures | Varsity Module 4, leverage and shorting chapters |
| Thu | Pricing: spot, cost of carry, basis, convergence at expiry | Varsity Module 4, futures pricing chapter |
| Fri | Open interest, rollover, hedging a portfolio with index futures | Varsity Module 4, open interest and hedging chapters |

Reading for the month: Natenberg, the opening chapters on contract basics and elementary strategies. Twenty minutes on three days.

## Practical

- Each day at 2:30, record Nifty spot, the near-month future and the next-month future. Compute the basis. Watch it over the week.
- Use a broker margin calculator to find the margin for 1 lot of Nifty futures and for one stock future. Write both as a percentage of your trading capital.
- Paper trade: one long and one short Nifty futures position held for 2–3 days, with entry, stop and daily mark-to-market written in the journal.

## Lab 5: futures arithmetic

Folder: `05-labs/lab05/`

1. A function that takes entry, exit, lot size and lots, and returns P&L, notional value and leverage on a given margin.
2. Simulate daily mark-to-market for a 10-day position on real Nifty data: starting margin, daily gains and losses, the day a margin call would arrive.
3. Fair value: F = S × (1 + r × t) minus expected dividends. Compare with the actual futures price for three dates.
4. Hedge exercise: a ₹5 lakh portfolio with beta 1.1. How many Nifty lots hedge it, and why is the answer awkward at lot size 65?

## Concept questions

Answers in `06-answers/week-05.md`.

1. Nifty future bought at 25,000, lot 65. It closes 300 points lower the next day. What is the mark-to-market loss, and as a percentage of ₹1 lakh?
2. Why does a futures price usually sit above spot, and when can it sit below?
3. What happens to the basis as expiry approaches, and why must it?
4. Margin is about 12% of contract value. What is the leverage, and what index move wipes out the margin?
5. How is shorting a future different from shorting a stock in the cash market, mechanically and in risk?
6. Price is rising and open interest is rising. Price is rising and open interest is falling. What does each suggest, and how sure can you be?
7. What is rollover and what does it cost?
8. Under your rule R1 (1% risk on ₹1 lakh), how many Nifty points of adverse move could you tolerate on one lot? Is that a workable stop?
9. Why can a correct view on direction still lose money in a leveraged position?
10. What is the difference between hedging and speculating with the same instrument?

## Checkpoint

- [ ] Basis table for 5 days
- [ ] Margin percentages written
- [ ] 2 paper futures trades journaled
- [ ] Lab 5 and answers pushed
- [ ] Swing journal up to date
