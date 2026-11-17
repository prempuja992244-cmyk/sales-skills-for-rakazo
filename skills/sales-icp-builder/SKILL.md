---
name: sales-icp-builder
description: Define or sharpen the ideal customer profile (ICP) and buyer personas. Use when the user asks "who should I sell to", "define my ICP", "build buyer personas", "which customers are best", or when lead scoring or outreach has no clear target.
---

# ICP and persona builder

## Inputs
- `sales-context.md` (run `sales-context` first if missing).
- Optional: a list of current or past customers (CRM export, sheet, or pasted list). Best customers are the strongest evidence.

## Steps
1. **Find the best customers.** If a customer list exists, rank customers by revenue, speed to close, retention, and ease of service. Take the top 20% as the model.
2. **Extract shared traits** of the top group:
   - Firmographics: industry, size (employees or revenue), location, years in business.
   - Technographics: tools they already use (e.g. Shopify, Tally, Salesforce).
   - Situation: growth stage, recent funding, hiring, new location, compliance deadline.
   - Pain and trigger: what made them buy now.
3. **Write the ICP** in this format:
   - Must-have (all required)
   - Nice-to-have (raise priority)
   - Disqualifiers (never pursue)
4. **Write 2–4 personas.** For each: title/role, goals, daily pains, objections, what proof convinces them, preferred channel, words they use.
5. **Anti-ICP.** List customer types that waste time (too small, wrong region, needs custom work).
6. **Save** as `icp.md` and add a short version to `sales-context.md`.

## Output
A one-page ICP plus persona cards. End with 3 example companies or people that fit, found through research only if the bot has web access, otherwise ask the user for examples.

## Rules
- Base traits on real customer data when available; label guesses as assumptions.
- Keep the ICP narrow enough that a stranger could say yes/no for any lead in under a minute.
