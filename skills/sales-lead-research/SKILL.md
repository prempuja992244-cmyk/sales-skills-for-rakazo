---
name: sales-lead-research
description: Research a prospect company or person before outreach or a meeting, and build a lead list from public sources. Use when the user says "research this lead/company", "find leads", "build a prospect list", "who should I contact at X", or gives a company name, website, or LinkedIn URL to prepare outreach.
---

# Lead research

## A. Research one prospect
Use the browser and web search on the bot's computer. Spend no more than ~10 minutes per lead.

Collect:
1. **Company**: what they do, size, location, recent news (funding, hiring, launches, expansion, awards), tools they use (job posts often reveal this).
2. **Person**: role, time in role, recent posts or talks, shared connections or interests.
3. **Fit**: match against `icp.md` → Fit / Maybe / No, with the reason.
4. **Hook**: one specific, true observation that links their situation to our offer.
5. **Contact path**: public business email pattern, LinkedIn, company phone, WhatsApp Business number if published.

Save a lead card:
```
Company | Website | Person | Role | Fit | Hook | Source links | Date researched
```

## B. Build a lead list
1. Confirm the ICP filters with the user (industry, region, size, role).
2. Find companies through public sources: Google Maps, industry directories, LinkedIn search, marketplaces, event exhibitor lists, startup databases, job boards.
3. For each company, find the right role (decision maker first, then a user/champion).
4. Write rows to the user's tracker (Google Sheet / CRM via connected app) or to `leads.csv`.
5. Deduplicate against existing CRM contacts before adding.

## Rules
- Use only public, business-related information. Do not collect personal data such as home addresses, family details, or personal phone numbers.
- Respect site terms; do not log in to other people's accounts or bypass paywalls or CAPTCHAs.
- Always store the source link for every fact used in a hook.
- Mark guessed email addresses as `unverified`.
