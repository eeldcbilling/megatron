# Week 7 (28 Dec–3 Jan): Pricing, volatility and the Greeks

*Draft. Tuned at the month-1 review.*

**Why this week exists:** you said you have "tried to understand Black-Scholes". This week you build it. Once you have written the pricer yourself, the Greeks stop being vocabulary and become things you can compute and check.

**Real money:** swing system only.

## Outcomes

- Explain what an option's price is: the cost of hedging it, driven mainly by volatility.
- Implement Black-Scholes for calls and puts and derive the Greeks numerically.
- Compute implied volatility from a market price.
- Explain delta, gamma, theta and vega as risks, with numbers for a real position.
- Understand realised versus implied volatility, India VIX, and the volatility smile.

## Study

| Days | Topic | Source |
|---|---|---|
| Mon | Volatility: daily and annualised, the square-root-of-time rule, normal distribution of returns and where it fails | Varsity Module 5, volatility chapters. Natenberg, chapter on volatility |
| Tue | Black-Scholes: inputs, intuition, assumptions | Varsity Module 5, Black-Scholes chapter. MIT OCW 18.S096 lecture on Black-Scholes for the rigorous version. Khan Academy: "Black-Scholes formula" |
| Wed | Delta and gamma | Varsity Module 5, delta and gamma chapters. projectfinance: "option delta explained", "gamma explained" |
| Thu | Theta and vega; how Greeks interact near expiry | Varsity Module 5, theta and vega chapters. Natenberg, chapter on risk measurement |
| Fri | Implied volatility, IV percentile, skew, India VIX, event volatility | Sensibull IV charts. Search "volatility smile explained" |

## Practical

- Each day at 2:30, record India VIX and the at-the-money straddle price for the nearest Nifty weekly. Convert the straddle price to an expected move in points and in percent. On expiry, compare with what happened.
- For one paper position, write its delta, gamma, theta and vega each day and predict tomorrow's P&L for a ±100 point move. Check the next day.

## Lab 7: build the pricer

Folder: `05-labs/lab07/`

1. Compute 20-day realised volatility of Nifty from daily returns, annualised. Plot it over five years.
2. Implement Black-Scholes for European calls and puts. No library pricing functions; `math` and `scipy.stats.norm` are allowed.
3. Greeks two ways: closed-form, and by bumping inputs (finite differences). They should agree.
4. Implied volatility solver using bisection or Newton's method.
5. Take a live Nifty option chain (typed in by hand is fine): compute IV per strike, plot the smile.
6. Reprice the chain with your IVs and confirm you recover market prices.
7. Plot theta against days to expiry for an at-the-money option. Plot gamma against spot for 1 day and for 20 days to expiry.

## Concept questions

Answers in `06-answers/week-07.md`.

1. Of the Black-Scholes inputs, which one is not observable, and what follows from that?
2. India VIX is 14. What daily move does that imply, roughly, and how do you get there?
3. An at-the-money option has a delta near 0.5. Give two different interpretations of that number.
4. Why is gamma largest for at-the-money options close to expiry, and why does that frighten option sellers on expiry day?
5. Theta is the seller's income. What is the seller being paid to bear?
6. You buy a call before results. The stock rises 2% and your call falls. Explain with vega.
7. Realised volatility over the last month is 10% and implied is 15%. Who has been making money, buyers or sellers? What could change that overnight?
8. What does the volatility smile say about the Black-Scholes assumption of normally distributed returns?
9. Your finite-difference delta and closed-form delta differ in the fourth decimal. Why, and does it matter?
10. A short at-the-money straddle has near-zero delta. Is it therefore low risk? Answer using gamma and vega.

## Checkpoint

- [ ] VIX and straddle table for 5 days, with expected versus actual move
- [ ] Daily Greeks prediction log for one paper position
- [ ] Lab 7 pushed; pricer matches market within reason
- [ ] Answers pushed
