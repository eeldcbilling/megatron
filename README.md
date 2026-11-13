# Megatron — 12-week trading foundation

A structured, practical course to go from "EMAs and support/resistance by feel" to a tested swing system, a working understanding of futures and options, and a first reading of order flow. Everything lives in this repo as markdown so it can be picked up on any machine.

- **Start date:** Monday 16 Nov 2026
- **End date:** Sunday 7 Feb 2027
- **Time budget:** 2–3 hours a day, 5–6 days a week
- **Live screen window:** 2:30–3:30 pm (the open is not available yet)

## Resume on any machine

```bash
git pull
```

Then open, in this order:

1. [`03-progress/STATUS.md`](03-progress/STATUS.md) — where you are and what is due next
2. The current week file in [`02-curriculum/`](02-curriculum/)
3. [`00-context/rules.md`](00-context/rules.md) — read before placing any trade

When working with Claude on a new machine or a new chat, say: *"Megatron: pull and resume."* The word **Megatron** is the trigger; a chat that does not mention it is not logged or pushed. The mentor instructions are in [`CLAUDE.md`](CLAUDE.md).

## Which Claude model to use

| Session | Model |
|---|---|
| Daily work: a concept, grading answers, lab code review, checking a trade plan, logging | Opus 5.5, medium effort |
| Gate exams, monthly reviews, debugging a suspicious backtest, the week-12 decision | Fable, or Opus at higher effort |

If a session grades shallowly or agrees too easily, switch up for that session. Whatever the model, start with "Megatron: pull and resume".

## Saving work

Claude saves and pushes after every reply (the continuity rule in [`CLAUDE.md`](CLAUDE.md)). For your own work (answers, labs, journal):

```bash
git add -A && git commit -m "Week N day D: <what you did>" && git push
```

Pull before you start and push when you stop, on every machine, so two machines never hold different versions.

## Map of the repo

| Folder | What it holds |
|---|---|
| [`00-context/`](00-context/) | Who the learner is, the mentor's charter, the risk rules, decisions made and questions still open |
| [`01-roadmap/`](01-roadmap/) | The 12-week plan, milestones, gates, daily and weekly rhythm |
| [`02-curriculum/`](02-curriculum/) | One file per week: study, practical work, Python lab, concept questions, checkpoint |
| [`03-progress/`](03-progress/) | Status, tracker, weekly reviews |
| [`04-journal/`](04-journal/) | Trade journal, daily prediction log, templates |
| [`05-labs/`](05-labs/) | Your Python code, one folder per lab |
| [`06-answers/`](06-answers/) | Your written answers to concept questions, with the mentor's evaluation |
| [`07-logs/`](07-logs/) | Every prompt and every chat, in chronological order |
| [`resources.md`](resources.md) | Books, video sources, tools and their costs |
| [`tools/`](tools/) | Small scripts that maintain the repo |

## The three-month shape

| Month | Weeks | Theme | You finish with |
|---|---|---|---|
| 1 | 1–4 | Market mechanics, price structure, risk | A written swing system, backtested, traded at tiny size |
| 2 | 5–8 | Futures and options | Black-Scholes built by hand, strategies paper-traded with a log |
| 3 | 9–12 | Auction theory, order flow, systematic work | A personal playbook and a decision on your specialisation |

Details: [`01-roadmap/roadmap.md`](01-roadmap/roadmap.md).
