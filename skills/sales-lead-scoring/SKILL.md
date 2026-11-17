---
name: sales-lead-scoring
description: Score, qualify, and prioritize leads using fit and intent, plus BANT, MEDDIC or SPICED qualification. Use when the user asks "which leads should I call first", "score my leads", "qualify this lead", "is this deal real", or wants a hot/warm/cold list from a CRM or sheet.
---

# Lead scoring and qualification

## 1. Fit score (0–50) — is this our kind of customer?
Score against `icp.md`:
- Industry match: 0–15
- Size / budget match: 0–15
- Location / serviceable: 0–10
- Role of contact (decision maker 10, influencer 6, user 3, unknown 0)
Any disqualifier → score 0 and mark `Disqualified` with reason.

## 2. Intent score (0–50) — are they likely to buy now?
- Replied positively or asked for price/demo: +20
- Visited pricing page / opened emails 3+ times (if tracking is connected): +10
- Trigger event in last 90 days (funding, hiring for related role, new branch, compliance deadline): +10
- Uses a competitor or a tool we integrate with: +5
- Referred by a customer: +5
- No response after full sequence: −10
- Explicit "not interested": set intent 0

## 3. Grade
- 75–100 **Hot**: contact today, personal outreach, offer a meeting.
- 50–74 **Warm**: sequence + personalised touch this week.
- 25–49 **Nurture**: monthly value content.
- <25 **Cold/Drop**.

## 4. Qualify active deals
For leads in conversation, fill one framework (default BANT for small deals, MEDDIC for large B2B):
- **BANT**: Budget, Authority, Need, Timeline.
- **MEDDIC**: Metrics, Economic buyer, Decision criteria, Decision process, Identified pain, Champion.
- **SPICED**: Situation, Pain, Impact, Critical event, Decision.
Mark each item `Confirmed`, `Assumed`, or `Unknown`. Every `Unknown` becomes a question for the next call.

## Output
Sorted table: Lead | Fit | Intent | Total | Grade | Next action | Owner. Write scores back to the CRM/sheet if a connected app allows, after the user approves the column changes.

## Rules
- Show the reason for each score; never present a score without evidence.
- Recalculate weekly or when new activity arrives.
