---
name: sales-context
description: Set up or update the business's sales context (what we sell, ideal customer, offer, proof, tone, language, sales channels, CRM). Use before any other sales skill when no sales context is saved yet, when the user says "set up my sales", "here is my business", "update my ICP/offer/pricing", or when another sales skill needs facts it does not have.
---

# Sales context

Every other skill in this kit depends on one shared, written sales context. Build it once, save it, and keep it current.

## 1. Check what already exists
- Look in your memory and workspace for a saved note or file named `sales-context.md`.
- If it exists, read it, show the user a short summary, and ask only what is missing or out of date.

## 2. Collect the facts (ask at most 5 questions at a time)
Business
- Company name, website, one-line description.
- Products or services sold, with price range or pricing model.
- Where you sell: country/cities, B2B or B2C, online or offline.

Customer
- Ideal customer: industry, company size, location, budget range (or person type for B2C).
- Buyer roles: who decides, who uses, who pays.
- Top 3 pains the customer has before buying.

Offer and proof
- Main promise in one sentence (outcome + timeframe).
- Proof: customer names you may mention, numbers, testimonials, case studies.
- Guarantee, free trial, demo, or other low-risk first step.

Selling
- Channels: email, LinkedIn, WhatsApp, phone, Instagram, walk-in, marketplaces.
- Outreach language: English, Hindi, Hinglish, or other. Tone: formal / friendly / casual.
- CRM or tracker: HubSpot, Zoho, Pipedrive, Salesforce, Google Sheets, Excel, none.
- Sender identity: name, role, signature, calendar booking link.
- Hard rules: words to avoid, claims not allowed, discounts limits, who must approve messages.

## 3. Save it
Write the answers to `sales-context.md` using these headings: Business, Offer, Ideal customer, Buyer roles, Pains, Proof, Channels, Language and tone, CRM, Sender, Rules. Also save a 5-line summary to memory so every bot can find it.

## 4. Confirm
Show the user the summary and ask: "Is anything wrong or missing?" Update on their reply.

## Rules
- Never invent customers, numbers, or testimonials. Leave a field as `UNKNOWN` instead.
- If the user gives pricing, record whether it can be shared with prospects.
- Re-run this skill whenever the offer, price, or target customer changes.
