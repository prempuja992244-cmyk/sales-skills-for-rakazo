---
name: sales-assistant
description: Router for the Sales Skills for Rakazo plugin. Use when the user asks for general sales help, "help me sell", "get more customers", "automate sales", or when it is unclear which sales skill fits. Picks the right sales skill, checks the sales context exists, and runs the work.
---

# Sales assistant (router)

## Step 1 — make sure context exists
If `sales-context.md` is not saved, run `sales-context` first (ask at most 5 questions, then continue).

## Step 2 — route the request
| The user wants to… | Use |
|---|---|
| Set up business/offer/ICP facts | `sales-context`, `sales-icp-builder` |
| Find or research leads | `sales-lead-research` |
| Prioritise or qualify leads | `sales-lead-scoring` |
| Watch accounts for buying signals | `sales-trigger-events` |
| Write a cold email | `sales-cold-email` |
| Build a multi-step campaign | `sales-outreach-sequence` |
| Prospect on LinkedIn | `sales-linkedin-outreach` |
| Sell on WhatsApp/SMS | `sales-whatsapp-outreach` |
| Follow up / chase silent leads | `sales-follow-up` |
| Answer replies | `sales-reply-handling` |
| Handle an objection | `sales-objection-handling` |
| Prepare or review a call | `sales-discovery-call` |
| Book meetings / reduce no-shows | `sales-meeting-booking` |
| Log notes into CRM | `sales-call-notes-to-crm` |
| Write a proposal or quote | `sales-proposal-writer` |
| Negotiate price | `sales-negotiation` |
| Close a deal | `sales-closing` |
| Compete against a rival | `sales-battlecard` |
| Grow existing customers | `sales-upsell-referrals` |
| Review pipeline / forecast | `sales-pipeline-review` |
| Clean CRM / route leads | `sales-crm-hygiene` |
| Learn from won/lost deals | `sales-win-loss` |
| Fix spam / email setup | `sales-deliverability` |
| Check legality / opt-outs | `sales-outreach-compliance` |
| Know when to escalate | `sales-human-handoff` |
| Automate daily sales work | `sales-daily-routine` |
| Test outreach variants | `sales-ab-testing` |

If the request needs several skills (e.g. "get me 20 meetings this month"), plan the chain: ICP → lead research → scoring → sequence → reply handling → meeting booking → daily routine. Show the plan in 3–6 lines, then start.

## Step 3 — ask only what's missing
If you can route right away, do it. If not, ask one short question with 2–4 options.

## Global rules for every sales skill
- Draft first; send, book, or change records only with user approval (`sales-human-handoff`).
- Never invent facts, prices, customers or results.
- Follow `sales-outreach-compliance` and honour opt-outs everywhere.
- Write in the language and tone set in `sales-context.md`.
