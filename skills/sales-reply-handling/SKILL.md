---
name: sales-reply-handling
description: Triage and answer prospect replies from email, LinkedIn or WhatsApp — interested, question, objection, referral to someone else, not now, out of office, unsubscribe, angry. Use when the user says "handle my sales replies", "check the inbox for lead responses", "what should I reply", or when a routine processes new replies.
---

# Reply handling

## 1. Classify each reply
| Class | Signal | Action |
|---|---|---|
| Interested | asks price, demo, call, details | Reply within 1 hour, propose 2 time slots or booking link (`sales-meeting-booking`) |
| Question | asks about feature, fit, process | Answer briefly + ask one qualifying question |
| Objection | price, timing, competitor, "we do it in-house" | Use `sales-objection-handling` |
| Referral | "talk to X" | Thank, ask for intro or permission to mention them, contact X referencing the referral |
| Not now | "next quarter", "busy" | Agree, confirm a date, set reminder, move to nurture |
| Out of office | auto-reply | Pause sequence until return date + 2 days; note any alternate contact |
| Not interested | clear no | Thank, stop sequence, ask (optional) one-line reason |
| Unsubscribe / stop | opt-out words | Stop all outreach immediately, record opt-out, no reply needed beyond confirmation if required |
| Angry | complaint, hostility | Apologise briefly, remove from list, escalate to user (`sales-human-handoff`) |
| Wrong person / bounce | | Fix data, find correct contact |

## 2. Draft the reply
- Mirror their length and tone. Short reply → short answer.
- Answer exactly what they asked first, then one next step.
- Use only facts from `sales-context.md`; if unsure (custom pricing, legal terms), say you'll confirm and escalate.

## 3. Update records
Stop the sequence for that lead, update stage/status, log the reply summary and next action with a date.

## 4. Report
For a batch, give the user: counts per class, drafts awaiting approval (hot ones first), and any escalations.

## Rules
- Never argue with a prospect. Never send pricing that isn't approved in the context file.
- Every outgoing reply needs approval unless the user approved auto-replies for this class (e.g. out-of-office handling).
