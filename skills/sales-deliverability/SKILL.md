---
name: sales-deliverability
description: Keep sales emails out of spam — domain and DNS setup (SPF, DKIM, DMARC), separate sending domains, warm-up, daily volume limits, list verification, bounce and complaint handling. Use when the user asks "why are my emails going to spam", "set up cold email domain", "how many emails per day", "check SPF/DKIM", or before launching an outbound campaign.
---

# Email deliverability

## Setup checklist
1. **Separate sending domain** for cold outreach (e.g. `getbrand.com` alongside `brand.com`) so the main domain's reputation is protected. Redirect it to the main website.
2. **SPF**: one TXT record listing the mail provider (e.g. Google Workspace, Microsoft 365).
3. **DKIM**: enabled in the mail provider and published in DNS.
4. **DMARC**: start with `p=none` and a reporting address, move to `quarantine` once stable.
5. **Custom tracking domain** if open/click tracking is used; consider turning tracking off for first touches.
6. Real sender name, profile photo, and signature; mailbox can receive replies.

Check records with public DNS lookup tools in the browser; report pass/fail for each.

## Warm-up and volume
- New mailbox: start at ~10–20 emails/day, increase gradually over 3–4 weeks.
- Steady state: keep cold volume modest per mailbox (often ≤ 30–50/day); add mailboxes rather than pushing one.
- Spread sends across business hours; avoid identical bursts.

## List quality
- Verify emails before sending; remove invalid, role-based (info@, admin@) unless intended, and catch-all risks.
- Keep bounce rate < 2% and spam complaints near 0. Pause if bounces rise.

## Content
Plain text, one link max, no attachments in first touch, personalised first line, clear opt-out.

## Monitoring (weekly routine)
Bounce rate, reply rate, spam placement tests, blacklist checks, DMARC reports. If reply rate drops sharply, pause and investigate before sending more.

## Rules
DNS changes affect all company email — prepare the exact records and let the user (or their IT) apply them, or apply only after explicit approval.
