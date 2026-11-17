---
name: sales-crm-hygiene
description: Clean and maintain CRM or lead-sheet data — duplicates, missing fields, wrong stages, bad emails, unassigned leads, lead routing and enrichment. Use when the user says "clean my CRM", "dedupe contacts", "fix my lead sheet", "assign leads", "enrich these leads", or sets up a data-quality routine.
---

# CRM hygiene and lead routing

## Audit (read-only first)
Report counts and examples for:
- Duplicate contacts/companies (same email, phone, or domain + name).
- Missing required fields: owner, source, stage, next step, phone/email.
- Invalid data: bounced or malformed emails, phone numbers without country code, "test" records.
- Stale records: open deals untouched 30+ days, leads never contacted.
- Opt-outs not flagged.

## Fix plan
Propose fixes as a table (record → change → reason). Group by type. Apply only after user approval, in small batches, and keep a change log (`crm-changes-{date}.csv`) so changes can be reversed.

Merge rules: keep the record with the most activity; copy missing fields from the other; never delete activity history.

## Enrichment
Fill company size, industry, website, LinkedIn URL, city from public sources or a connected enrichment tool. Mark source and date.

## Lead routing (new leads)
1. Check duplicates first.
2. Score (`sales-lead-scoring`).
3. Assign owner by rule: territory/region, industry, deal size, or round-robin.
4. Set first-touch SLA: Hot → within 1 hour, Warm → same day, Nurture → this week.
5. Notify the owner.

## Rules
- Never bulk-delete. Archive or tag instead, and only with explicit approval.
- Respect opt-outs across all records of the same person.
