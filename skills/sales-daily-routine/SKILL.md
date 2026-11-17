---
name: sales-daily-routine
description: Run or set up the daily and weekly sales automation routines for a Rakazo bot — morning sales brief, new-lead processing, replies, due follow-ups, approval batch, end-of-day log, weekly pipeline and win-loss reviews. Use when the user says "automate my sales", "daily sales routine", "set up a sales bot", "what should the bot do every day", or wants a recurring sales schedule.
---

# Daily and weekly sales routines

## Setup (once)
1. Confirm `sales-context.md` exists (`sales-context`).
2. Confirm connected apps: mailbox, calendar, CRM or Google Sheet, and optionally WhatsApp/LinkedIn access on the bot's computer. If missing, ask the user to connect them in Integrations.
3. Ask for: working days and hours, time zone, daily send limits, which actions may run without approval (default: none).
4. Create the routines below in Rakazo (or ask the bot to "add this to a routine").

## Daily routine — morning (e.g. 9:00 local time)
1. **New leads**: dedupe, enrich, score, assign (`sales-crm-hygiene`, `sales-lead-scoring`).
2. **Replies since yesterday**: classify and draft answers (`sales-reply-handling`).
3. **Follow-ups due today**: draft them (`sales-follow-up`, `sales-outreach-sequence`).
4. **Today's meetings**: prep briefs (`sales-discovery-call`) and send reminders (`sales-meeting-booking`).
5. **Approval batch**: send the user ONE message with everything to approve, hottest first:
   ```
   🔥 Hot replies (n) · 📅 Meetings today (n) · ✉️ Follow-ups ready (n) · 🆕 New hot leads (n)
   ```
6. Send approved items within working hours and sending limits; log every action in the CRM.

## Daily routine — end of day (e.g. 18:00)
- Log the day: messages sent, replies, meetings booked, deals moved.
- List anything waiting on the user.

## Weekly (e.g. Monday morning)
- Pipeline review and forecast (`sales-pipeline-review`).
- Trigger events for named accounts (`sales-trigger-events`).
- Deliverability check (`sales-deliverability`).

## Monthly
- Win-loss analysis (`sales-win-loss`), objection library update, A/B test results (`sales-ab-testing`).

## Rules
- Never message outside the prospect's local business hours or on major local holidays.
- If a connected app fails, report it in the brief instead of retrying endlessly.
- Respect every rule in `sales-human-handoff` and `sales-outreach-compliance`.
