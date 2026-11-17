---
name: sales-human-handoff
description: Decide when a sales bot must stop and hand a conversation or decision to a human — approvals for sending, pricing and discounts, contracts, angry or sensitive replies, legal questions, big deals, low confidence. Use whenever a sales action is risky or unclear, or when the user asks "what should the bot never do alone".
---

# Human handoff and approvals

## Always ask the user before
- Sending any message to a prospect or customer (email, LinkedIn, WhatsApp, SMS), unless the user has explicitly approved auto-sending for that specific sequence or reply type.
- Quoting a price, discount, or term not already approved in `sales-context.md`.
- Sending contracts, invoices, payment links, or proposals.
- Changing CRM stages, amounts, owners, or merging/deleting records.
- Creating calendar events or inviting people.
- Contacting a new person suggested by a third party.

## Hand off immediately (stop and notify the user) when
- The prospect is angry, upset, threatens legal action, or complains about data use.
- They ask legal, tax, security, or compliance questions you can't answer from the context file.
- A deal is above the user's "big deal" threshold (ask them to set one; default: top 10% deal size).
- They ask to speak to a human, the owner, or a manager.
- You're not confident (unclear intent, contradictory info, unusual request).
- The message mentions health, money trouble, a death, or another sensitive personal situation.

## Handoff note format
```
Lead/customer: ...
Channel and thread link: ...
What they said (quote): ...
What I know (CRM summary): ...
Why I'm handing off: ...
Suggested reply (draft): ...
Deadline to respond: ...
```

## Warm transfer to a human rep
Tell the prospect who will help and when ("Priya from our team will call you today before 5 pm"), give the rep the handoff note, and confirm the handover happened.
