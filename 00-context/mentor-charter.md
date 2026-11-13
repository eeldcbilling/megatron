# Mentor charter

The positions the mentor took at the start, with reasons. These are the mentor's views, not the learner's. Where he has agreed, it is recorded in [`decisions.md`](decisions.md).

## 1. Twelve weeks buys a foundation, not mastery

Three months is enough to understand market mechanics, build and test one swing system, understand derivatives properly and read order flow at a beginner level. It is not enough to be good at all of swing, intraday, options selling, algo trading and order flow. The course goes wide on understanding and narrow on real-money practice: **one style with real money (swing, cash equities), everything else on paper.**

## 2. The biggest risk is already known

The worst loss so far came from one trade: a leveraged short in a stock that could lock in circuit. That is 30% of capital gone on a single position. The lesson is about structure, not about stock picking:

- Position size was set by available margin instead of by the loss he could accept.
- The instrument could become impossible to exit.
- There was no point at which the trade was automatically over.

Every rule in [`rules.md`](rules.md) exists to make that kind of loss impossible. A course that teaches chart reading without fixing this would be teaching the wrong thing.

## 3. A 20% loss limit is too wide for a learner

He said a losing streak up to 20% of capital would not shake him. The mentor's position: during the learning phase, real trading stops at **10%**. The reason is practical. At 1% risk per trade, losing 10% takes ten full losses with no winners. If that happens, the system or the execution is broken and more trades will not fix it.

## 4. No real-money F&O in these twelve weeks

With the Nifty lot at 65, one futures lot carries roughly ₹16–17 lakh of exposure and needs margin close to the entire trading capital. Even a 50-point defined-risk option spread can lose about ₹3,000, which is 3% of ₹1 lakh. Neither fits a 1% risk rule. So futures and options are studied in depth and traded on paper with a full log. Real F&O is a decision for the week-12 review.

"Low-risk profit" from short straddles and strangles needs correcting early: they win often and lose big. High win rate and low risk are different properties. Weeks 7–8 make this concrete with numbers.

## 5. His edge is testing, not prediction

A computer science background does not predict prices better. It lets him check an idea against data before paying for it, measure his own behaviour from a journal, and automate the boring parts (scans, alerts, position sizing). So every week has a Python lab, and no setup is traded with real money until it has been tested.

## 6. The schedule decides the style

He can watch 2:30–3:30 pm and study at flexible times, but not the open. That fits end-of-day swing trading and rules out serious intraday work for now. Order flow in weeks 9–10 will be studied on the closing hour and on replay.

## 7. No leave yet

Earned leave is worth more later, for a focused block of live trading with a tested setup. For now, steady daily hours matter more than long days. (He agreed.)

## 8. Order flow comes last

It only means something once market structure and auction logic are understood. It is placed in month three. (He agreed.)

## 9. What the mentor will not do

- Give trade tips or approve a trade without hearing the thesis first.
- Relax a risk rule in the middle of a trade or a losing streak.
- Pretend progress is better than the journal shows.
