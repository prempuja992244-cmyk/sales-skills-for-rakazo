---
name: sales-outreach-sequence
description: Design a multi-step, multi-channel outreach cadence (email, LinkedIn, WhatsApp, phone) with timing, copy for every step, and stop rules. Use when the user asks for a "sequence", "cadence", "drip", "follow-up campaign", "outbound campaign", or wants to automate outreach over several days.
---

# Outreach sequence

## Default B2B cadence (14–21 days, 6–8 touches)
| Day | Channel | Purpose |
|---|---|---|
| 1 | Email | First touch with specific hook (`sales-cold-email`) |
| 2 | LinkedIn | Profile view + connection request, no pitch (`sales-linkedin-outreach`) |
| 4 | Email | Reply in same thread: new angle or short proof |
| 6 | Phone / WhatsApp* | Short call or message referencing the email |
| 9 | Email | Useful resource: case study, checklist, 2-min video |
| 12 | LinkedIn | Comment or message adding value |
| 16 | Email | Different pain or persona angle |
| 21 | Email | Polite break-up: "Should I close your file?" |

*WhatsApp only with prior opt-in or an existing relationship — see `sales-whatsapp-outreach`.

For B2C or local businesses, shorten to 5 touches over 10 days and lead with WhatsApp/phone if the customer contacted you first.

## Build steps
1. Confirm audience segment, goal (meeting/reply/demo), channels allowed, and sender.
2. Write every step's copy. Each step must add something new: a fact, proof, resource, or question. Never "just bumping this".
3. Add personalisation fields: `{first_name}`, `{company}`, `{hook}`, `{proof}`.
4. Define **stop rules**: stop on any reply, meeting booked, bounce, unsubscribe, or "not interested".
5. Define **branch rules**: opened 3+ times with no reply → phone step earlier; positive reply → `sales-reply-handling`; out-of-office → pause until return date.
6. Save as `sequences/<name>.md` and, if a sequencing tool (HubSpot, Apollo, Lemlist, Instantly, etc.) is connected, prepare the steps there as drafts.

## Running it with a Rakazo routine
- Daily routine: find leads due for a step, draft messages, ask for approval in one batch, send approved ones, log activity.
- Respect sending limits (`sales-deliverability`) and local business hours (`sales-daily-routine`).

## Rules
- Never send without approval unless the user has explicitly set up auto-approval for this sequence.
- Max one touch per channel per day per lead; never message the same lead on 3 channels the same day.
