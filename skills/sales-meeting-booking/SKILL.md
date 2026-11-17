---
name: sales-meeting-booking
description: Book sales meetings and demos, send confirmations and reminders, handle reschedules, and reduce no-shows. Use when a prospect agrees to talk, when the user says "book a meeting", "schedule a demo", "send calendar invite", "they didn't show up", or wants automated meeting reminders.
---

# Meeting booking and no-show reduction

## Booking
1. Offer two specific slots in the prospect's time zone plus the booking link from `sales-context.md`.
   > "Would Tue 11:00 or Wed 16:00 IST work? Or pick any slot here: {link}"
2. When they choose, create the calendar event through the connected calendar app (after user approval) with:
   - Clear title: `{Company} x {Our company} — {purpose}`
   - Agenda (3 bullets) and video link or address.
   - All attendees they named.
3. Log the meeting in the CRM with stage `Meeting booked`.

## Confirmation and reminders
- Immediately: short confirmation with agenda and one question to prepare ("What would make this call useful for you?").
- 24 hours before: reminder with value ("I'll bring the example from {similar customer}").
- 1–2 hours before: brief reminder with the link (WhatsApp/SMS only if they opted in).

## Reschedules and no-shows
- Reschedule request → reply quickly, offer two new slots, no friction.
- No-show (wait 10 min) → friendly message: "Looks like today got busy — want to grab another slot?" with link. One more attempt after 2 days, then move to follow-up.

## Rules
- Always state time zone. Avoid lunch hours and local holidays where you know them.
- Never create events or send invites without user approval.
- Track show rate; if under 70%, check targeting, reminder copy, and time gap between booking and meeting.
