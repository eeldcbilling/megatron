# Week 9 (11–17 Jan): Auction market theory, volume profile, VWAP

*Draft. Tuned at the month-2 review.*

**Why this week exists:** order flow without context is noise. Auction theory supplies the context: where the market found fair value, where it rejected price, and who is likely trapped. Volume profile is the picture of that.

**Real money:** swing system only.

## Outcomes

- Describe the market as a two-way auction that moves between balance and imbalance.
- Read a volume profile: point of control, value area, high- and low-volume nodes.
- Use VWAP as the day's fair-price reference.
- Classify a day's shape (trend day, balanced day, double distribution) after the fact.

## Study

| Days | Topic | Source |
|---|---|---|
| Mon | The auction idea: price advertises, time regulates, volume confirms | Dalton, *Mind Over Markets*, opening chapters on the auction and the profile |
| Tue | Volume profile: POC, value area, nodes | Trader Dale: "volume profile". GoCharting education: market profile and volume profile lessons |
| Wed | Day types and the opening | Dalton, chapter on day types |
| Thu | VWAP and anchored VWAP | Search "VWAP explained institutional". Rayner Teo or The Chart Guys on VWAP |
| Fri | Tying it to your swing levels: do your support zones line up with high-volume nodes? | Your own charts |

## Practical

- Turn on volume profile (session and fixed-range) and VWAP in your charting tool.
- For 5 sessions, after the close: mark POC, value area high and low, VWAP. Label the day type. Write what the 2:30–3:30 hour did relative to value.
- For 5 of your swing-system stocks, draw a 6-month fixed-range profile. Compare its nodes with the S&R zones you drew in week 2.

## Lab 9: build a volume profile

Folder: `05-labs/lab09/`

1. Get 1-minute or 5-minute Nifty futures data for 10 sessions through the Fyers API (free data) or your charting tool's export.
2. Build a volume-at-price histogram per session. Compute the POC and the 70% value area.
3. Compute VWAP through the day and plot price, VWAP and the profile together.
4. Test one simple claim on your 10 days: how often does price, opening inside yesterday's value area, stay inside it all day? Ten days proves nothing; note that, and say how many you would need.

## Concept questions

Answers in `06-answers/week-09.md`.

1. What does it mean to say the market is "in balance", and what ends a balance?
2. What is the point of control, and why might price return to it?
3. Why does price tend to move quickly through a low-volume node and slowly through a high-volume one?
4. Price is above VWAP all day and VWAP is rising. Who is in control, and who is in pain?
5. What distinguishes a trend day from a balanced day by 11:00, and why does it matter for someone who only watches from 2:30?
6. How is a volume profile different from the volume bars under a chart?
7. Your week-2 support zone sits on a 6-month high-volume node. Does that strengthen it? Argue both sides.
8. Why is volume-at-price built from 5-minute bars only an approximation?
9. An opening outside yesterday's value that is quickly pulled back inside suggests what?
10. Which idea from this week could become a testable rule in your swing system?

## Checkpoint

- [ ] 5 sessions profiled by hand
- [ ] 5 stock profiles compared with week-2 zones
- [ ] Lab 9 and answers pushed
