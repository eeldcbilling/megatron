# Resources

Facts on this page were checked on **13 Nov 2026**. Prices, lot sizes and plan features change; re-check before relying on them.

## A note on video links

Only links that were verified are given as URLs. For other channels, the name and a search phrase are given instead of a guessed link. If a recommended video turns out weak or missing, tell the mentor and it gets replaced.

## Core free course: Zerodha Varsity

The spine of months 1 and 2. Free, India-specific, text plus video.

| Module | Link |
|---|---|
| All modules | https://zerodha.com/varsity/modules/ |
| Video modules | https://zerodha.com/varsity/video-modules/ |
| YouTube channel (English and Hindi videos) | https://www.youtube.com/@varsitybyzerodha |
| Technical analysis playlist | https://www.youtube.com/watch?v=yzRP-mA2eiE&list=PLX2SHiKfualH_xMbGM-3zWC47s9gUjGR_ |
| Module 1 Introduction to Stock Markets | https://zerodha.com/varsity/module/introduction-to-stock-markets/ |
| Module 2 Technical Analysis | https://zerodha.com/varsity/module/technical-analysis/ |
| Module 4 Futures Trading | https://zerodha.com/varsity/module/futures-trading/ |
| Module 5 Options Theory | https://zerodha.com/varsity/module/option-theory/ |
| Module 6 Option Strategies | https://zerodha.com/varsity/module/option-strategies/ |
| Module 9 Risk Management and Trading Psychology | https://zerodha.com/varsity/module/risk-management/ |
| Module 10 Trading Systems | https://zerodha.com/varsity/module/trading-systems/ |

If a module link has moved, start from the "All modules" page.

## Video channels by topic

Search the channel name on YouTube, then the phrase.

| Topic | Channel | Search phrase |
|---|---|---|
| Price action, swing trading | Rayner Teo | "price action trading course", "support and resistance" |
| Chart reading, plain technicals | The Chart Guys | "technical analysis basics" |
| Indian market basics (Hindi and English) | CA Rachana Ranade | "basics of stock market" |
| Trader interviews, Indian context | Elearnmarkets (Face2Face) | "Face2Face swing trading" |
| Options mechanics, very clear visuals | projectfinance | "options trading for beginners", "option greeks explained" |
| Options strategies and probabilities | Option Alpha, tastylive | "iron condor", "short strangle risk" |
| Options in the Indian market | Sensibull | "option strategies", "virtual trading" |
| Finance theory, short lessons | Khan Academy | "put call parity", "futures margin" |
| Black-Scholes and volatility, rigorous | MIT OpenCourseWare 18.S096 | "Topics in Mathematics with Applications in Finance" |
| Volume profile, order flow | Trader Dale | "volume profile", "order flow" |
| Order flow, professional tape reading | Axia Futures, Jigsaw Trading | "footprint", "price ladder", "absorption" |
| Order flow on the tool you may use | GoCharting | free order flow course on their education page |
| Python for trading | Part Time Larry | "backtesting python" |
| Python for trading, long course | freeCodeCamp | "Algorithmic Trading Using Python" |

Zerodha also runs a newsletter with a video series called *In The Money* (https://inthemoneybyzerodha.substack.com/), useful as weekly reading from month 2.

## Books

One per month is the reading plan. He is returning to books after a long gap, so portions are small: 20–30 minutes on the days marked in the week files.

| Month | Book | Why | How much |
|---|---|---|---|
| 1 | *Trading in the Zone*, Mark Douglas | Thinking in probabilities; the easiest read on this list | Whole book, about 15 pages a day |
| 2 | *Option Volatility and Pricing*, Sheldon Natenberg | The standard practitioner's book on options | Chapters named in weeks 6–8 only |
| 3 | *Mind Over Markets*, James Dalton | Auction market theory and market profile | Chapters named in weeks 9–10 only |

Reference shelf, to consult and not to read cover to cover:

- *Technical Analysis of the Financial Markets*, John Murphy. The encyclopedia for month 1.
- *Trade Your Way to Financial Freedom*, Van Tharp. Expectancy and position sizing.
- *Trading and Exchanges*, Larry Harris. Market microstructure; suits a CS mind.
- *Evidence-Based Technical Analysis*, David Aronson. Why most backtests lie.
- *Quantitative Trading*, Ernest Chan. A first book on systematic trading.

## Tools and what they cost

| Need | Tool | Cost (checked 13 Nov 2026) |
|---|---|---|
| Charts on PC | TradingView free plan, or Kite web | Free |
| Daily data for labs | `yfinance` Python package (NSE tickers end in `.NS`) | Free; fine for daily bars, not for anything precise intraday |
| Broker API with data | Fyers API | Free, including historical and live data |
| Broker API, Zerodha | Kite Connect | Personal plan free but has no market data; Connect plan ₹500 a month includes live and historical data |
| Broker API, Dhan | DhanHQ | Trading API free; data API ₹499 a month, or free with 25 trades in the previous 30 days |
| Options analysis and paper trading | Sensibull (virtual trading), through a broker login | Free tier, with paid plans for more |
| Order flow charts | GoCharting | Free plan for charts; footprint and CVD are on the paid India plan, listed around ₹1,495 a month |

Placing orders through any broker API needs a registered static IP under the retail algo rules. Not relevant until after this course; data access is unaffected.

## Contract facts (checked 13 Nov 2026)

| Item | Value |
|---|---|
| Nifty 50 lot size | 65 |
| Bank Nifty lot size | 30 |
| Nifty weekly expiry | Tuesday |
| NSE monthly expiry | Last Tuesday of the month |
| Bank Nifty, FinNifty, Midcap Nifty | Monthly expiry only, no weeklies |
| Sensex (BSE) | Weekly expiry on Thursday, lot 20 |

Always confirm on the NSE site or the broker terminal before sizing anything.
