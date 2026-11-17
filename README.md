# Sales Skills for Rakazo

**A sales skills plugin made only for Rakazo.**

A skills-only [Rakazo](https://github.com/elie222/rakazo) plugin that turns a Rakazo bot into a sales assistant: lead research, scoring, outreach (email, LinkedIn, WhatsApp), follow-ups, reply handling, meetings, proposals, negotiation, closing, CRM hygiene, pipeline reviews, deliverability, compliance and daily automation routines.

29 skills + 3 slash commands. Instructions only — no scripts, no MCP server, no secrets.

## Install in Rakazo

1. Create a **public** GitHub repository (e.g. `sales-skills-for-rakazo`) and upload every file and folder from this kit to the repository root (`plugin.json` must be at the root).
2. In Rakazo open **Integrations → + → From GitHub**.
3. Paste your repository URL, e.g. `https://github.com/<your-username>/sales-skills-for-rakazo`, and choose **Preview**.
4. Check the preview lists the skills and commands, then choose **Add**.
5. Open a bot and type `/sales-setup` to start.

Rakazo installs from public GitHub repositories only (not local folders or private repos). Installs are pinned to a commit: after changing files, remove the plugin and add it again.

## Start here

| Command | What it does |
|---|---|
| `/sales-setup` | Saves your business context and ICP, checks connected apps, proposes routines |
| `/sales-today` | Runs today's sales work and sends you one approval batch |
| `/sales-campaign <segment and goal>` | Plans a full outbound campaign |

Or just talk to the bot — `sales-assistant` routes any sales request to the right skill.

## Skills

**Foundation**
- `sales-assistant` — router for all sales requests
- `sales-context` — business, offer, proof, language, CRM facts (used by every skill)
- `sales-icp-builder` — ideal customer profile and personas

**Prospecting**
- `sales-lead-research` — research a prospect or build a lead list
- `sales-lead-scoring` — fit + intent scoring, BANT / MEDDIC / SPICED
- `sales-trigger-events` — buying signals on named accounts

**Outreach**
- `sales-cold-email` — first-touch emails that get replies
- `sales-outreach-sequence` — multi-channel cadences with stop/branch rules
- `sales-linkedin-outreach` — social selling
- `sales-whatsapp-outreach` — WhatsApp/SMS enquiry-to-sale with opt-in rules
- `sales-follow-up` — follow-ups and ghost recovery
- `sales-reply-handling` — classify and answer replies
- `sales-ab-testing` — test outreach variants

**Conversations and deals**
- `sales-objection-handling`
- `sales-discovery-call`
- `sales-meeting-booking`
- `sales-call-notes-to-crm`
- `sales-proposal-writer`
- `sales-negotiation`
- `sales-closing`
- `sales-battlecard`
- `sales-upsell-referrals`

**Operations and automation**
- `sales-pipeline-review`
- `sales-crm-hygiene`
- `sales-win-loss`
- `sales-deliverability`
- `sales-outreach-compliance`
- `sales-human-handoff`
- `sales-daily-routine`

## Connect these apps for full automation
In Rakazo **Integrations**: your mailbox (Gmail/Outlook), calendar, and CRM or Google Sheets (HubSpot, Zoho, Pipedrive, Salesforce…). LinkedIn and WhatsApp Web can be used through the bot's computer with your own login.

## Safety defaults
Every skill drafts first. Sending messages, booking meetings, quoting prices and changing CRM records need your approval unless you explicitly allow auto-approval for a specific routine. Opt-outs are honoured across all channels.

## Credits
Original text written for Rakazo. Skill coverage was inspired by these open-source collections — see them for deeper or tool-specific playbooks:
`sales-skills/sales`, `louisblythe/sales-skills`, `zapier/gtm-cheat-codes`, `gtmagents/gtm-agents`, `chadboyda/agent-gtm-skills`, `coreyhaines31/marketingskills`, `thecraighewitt/sales-skills`, `zubair-trabzada/ai-sales-team-claude`, `growthenginenowoslawski/coldoutboundskills`.

## License
MIT
