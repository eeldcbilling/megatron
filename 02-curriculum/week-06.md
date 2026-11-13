# Week 6 (21–27 Dec): Options foundations

*Draft. Tuned at the month-1 review.*

**Why this week exists:** you have watched videos on calls, puts and Greeks. This week replaces "I have seen this" with "I can compute this", starting from payoffs and building upward without any formula you cannot derive.

**Real money:** swing system only. Options on paper only.

## Outcomes

- Draw the expiry payoff of any single option and any two-leg combination from memory.
- Separate an option's price into intrinsic value and time value.
- Explain moneyness, and why out-of-the-money options are cheap and usually expire worthless.
- State put-call parity and use it to spot a mispricing.
- Read an option chain: strikes, premiums, open interest, implied volatility.

## Study

| Days | Topic | Source |
|---|---|---|
| Mon | Call and put, buyer and seller, the four basic positions | Varsity Module 5, chapters 1–6. projectfinance: "options trading for beginners" |
| Tue | Moneyness, intrinsic and time value | Varsity Module 5, moneyness chapter. Natenberg, chapters on contract specifications and expiration profit and loss |
| Wed | Put-call parity and synthetic positions | Khan Academy: "put call parity". Natenberg's section on synthetics |
| Thu | The option chain; European index options, cash settlement, physical settlement of stock options, expiry-day mechanics | NSE option chain page; Sensibull option chain. Zerodha support articles on physical settlement |
| Fri | Why option buyers usually lose and what the seller is paid for | Varsity Module 5, summary chapters on buying versus selling |

## Practical

- Each day at 2:30, record the at-the-money Nifty call and put premium for the nearest weekly expiry. Watch what happens to them through the week with the index roughly where it was.
- Pick one out-of-the-money call on Monday. Track its price daily to expiry (Tuesday). Write what happened and why.
- Paper trade on Sensibull virtual trading: buy one call, buy one put, on different days, with a written thesis and exit rule.

## Lab 6: payoff plotter

Folder: `05-labs/lab06/`

1. A `Leg` class: type (call, put, future), side (buy, sell), strike, premium, lots.
2. A function that plots the expiry payoff of any list of legs, marks break-even points, maximum profit and maximum loss.
3. Plot: long call, short put, long straddle, bull call spread, short strangle. Print max loss for each. For which is it unbounded?
4. Check put-call parity on live Nifty prices for three strikes: C − P against F − K (discounted). How large is the gap, and is it tradable after costs?

## Concept questions

Answers in `06-answers/week-06.md`.

1. Nifty at 25,000. A 25,200 call costs ₹80. What are the intrinsic value, time value, break-even at expiry, and the maximum loss for one lot of 65?
2. Why does the seller of that call need margin while the buyer does not?
3. Draw (describe) the payoff of buying a call and selling a put at the same strike. What is it equivalent to?
4. State put-call parity in words. What would you do if a call were too expensive relative to the put?
5. Why are index options in India settled in cash while stock options are settled by delivery, and what danger does that create for a small account holding a stock option into expiry?
6. An option is ₹5 on expiry morning, 150 points out of the money. People call it "cheap". Why is that the wrong word?
7. What does high open interest at a strike tell you, and what does it not tell you?
8. Your tracked out-of-the-money call: the index moved in your favour and the option still lost value. How?
9. Who is on the other side when a retail trader buys a far out-of-the-money weekly option, and why are they happy to sell it?
10. Which of the five payoffs you plotted has the highest probability of profit, and which has the worst worst-case? Is that a coincidence?

## Checkpoint

- [ ] 5 days of at-the-money premiums recorded
- [ ] Tracked option written up
- [ ] 2 paper option trades journaled
- [ ] Lab 6 and answers pushed
