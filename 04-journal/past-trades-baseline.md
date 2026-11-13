# Past trades: the baseline (March 2023 – November 2026)

Computed on 13 Nov 2026 from the broker trade files he supplied (three accounts). The raw files are not in this repo. Rupee amounts and account identifiers are left out; figures are counts, percentages and multiples. This is the "before" picture to compare the course journal against in February 2027.

Method: orders were combined per account and stock; same-day buys and sells were paired first as intraday trades, the rest matched first-in-first-out as delivery trades. Brokerage, taxes and charges are not in the files and are not deducted. One auction settlement (the short that locked in circuit) is also not in the files.

## The two kinds of trading he did

| | Delivery (held overnight or longer) | Intraday |
|---|---|---|
| Round trips | 91 | 81 |
| Win rate | 56% | 40% |
| Average winner | +21.6% | +1.1% |
| Average loser | −8.6% | −1.5% |
| Result before costs | Profitable | Loss-making |
| Share of all turnover | 18% | 82% |

All of the profit came from delivery trades. Intraday trading produced a loss before costs and generated more than four-fifths of the turnover, so it also paid most of the costs.

## Findings

1. **The delivery record has a workable shape.** Winners averaged about 2.5 times the size of losers with a win rate above half. That is what a swing system is supposed to look like, and it happened without a system.
2. **It is concentrated.** The best 3 trades made 59% of the delivery profit and the best 5 made 86%. Defence stocks were 38 of the 91 trades, won 66% of the time and made about 84% of the delivery profit. The other 53 trades won 49% of the time and made the rest. Take away one sector's bull run and the record is roughly flat.
3. **Losses were not cut.** 16 of 40 losing delivery trades were held more than 60 days. 12 lost more than 10%; the worst was held 359 days to −37.5%. Winners and losers were held for about the same time (median 25 and 30 days). There is no trace of a stop-loss anywhere in the record.
4. **Winners were often sold early.** 17 of 51 winning trades were closed within a week.
5. **Position size had no rule.** Delivery positions were modest. Intraday positions averaged about five times the delivery size, and the largest were five to six times the capital he says he had.
6. **Intraday was a 2023–24 habit that mostly stopped.** 72 of the 81 intraday trades were in the first year, with one month carrying more than half of that year's turnover. Since January 2025 there have been two.
7. **The big short was not a one-off.** The same stock was shorted intraday in size three times: a small win (October 2024), a loss of 6.4% on the position (January 2025), and then the circuit lock (January 2026) as the largest of the three by value, the morning after closing a small winning long in the same stock. On the long side this was his most profitable stock.
8. **Leverage came back after the big loss.** Four months later, on the morning a 6.7% loss in a large-cap was closed, an intraday position of more than three times his stated capital was opened in another stock and closed the same day for a small gain.
9. **One losing year.** Of the three full financial years, the middle one was a net loss on both delivery and intraday.

## What this changes in the course

- The swing style chosen for real money is the one that worked for him. Intraday and shorting stay out, now with his own numbers as the reason.
- Rule R2 (size from the stop) and R3 (stop placed as an order) address findings 3 and 5 directly. Finding 3 is the one to watch: the record shows he can hold a loser for a year.
- Finding 8 means the urge to "make it back" after a loss is live, not historical. The circuit breaker after two losing trades in a week exists for this.
- Week 4's backtest should include a version without defence stocks, to see whether System v1 depends on the same sector he did.
- In February, compare: win rate, average winner and loser, longest-held loser, largest position as a multiple of capital, number of trades without a written stop (target: zero).
