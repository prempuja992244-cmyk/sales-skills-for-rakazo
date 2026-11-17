---
name: sales-pipeline-review
description: Review the sales pipeline — stage definitions, stalled deals, forecast, coverage, conversion rates and the week's priorities. Use when the user asks "review my pipeline", "sales forecast", "which deals are stuck", "weekly sales report", "how much will we close this month", or sets up a weekly pipeline routine.
---

# Pipeline review and forecast

## Stage definitions (use the user's own if they exist)
| Stage | Exit criteria (must be true to move on) | Default probability |
|---|---|---|
| Lead | Fits ICP | 5% |
| Contacted | Two-way conversation started | 10% |
| Qualified | Pain + decision maker + timeline known | 25% |
| Meeting/Demo done | Prospect confirmed solution fits | 40% |
| Proposal sent | Proposal reviewed with buyer | 60% |
| Negotiation | Verbal yes, terms being agreed | 80% |
| Won / Lost | Signed & paid / closed with reason | 100% / 0% |

## Weekly review steps
1. Pull open deals from the CRM/sheet (connected app) — read-only.
2. Flag issues:
   - No next step or next-step date in the past.
   - No activity in 14+ days.
   - Close date in the past.
   - Stage doesn't match exit criteria.
   - Missing amount or decision maker.
3. Forecast:
   - **Weighted** = Σ amount × stage probability.
   - **Commit** = deals the user is confident will close this period.
   - **Coverage** = open pipeline ÷ target (aim 3× for B2B).
4. Metrics: new deals created, win rate, average deal size, average cycle length, stage-to-stage conversion.
5. Priorities: top 5 deals to push this week with the single next action for each.

## Output
A short report: headline numbers, risk list, top 5 actions, and suggested CRM corrections (applied only after approval). Suitable for a weekly Rakazo routine (e.g. Monday 9:00).

## Rules
Use only CRM data and user input; label any estimate. Don't change deal stages or amounts without approval.
