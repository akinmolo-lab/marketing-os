# CLAUDE.md: Marketing OS for <Company Name>

This file is the standing context for every Claude Code session in this repo. Read it first, then the latest file in `logs/`, before doing anything else.

> **Template.** Everything in `<angle brackets>` is a placeholder. Fill in section 1 and the `01-foundation/` files first: every agent depends on them.

---

## 1. The company

- **Company:** `<Company Name>`
- **What we sell:** `<one line>`
- **Who we sell to:** `<one line; detail in 01-foundation/ideal-customer.md>`
- **Market:** `<e.g. UK small businesses>`
- **Marketing team:** `<names and roles, or "one marketer">`
- **This year's main goal:** `<e.g. 200 qualified leads by December>`

## 2. How to work

- **Library first.** Before writing, planning or analysing, read the relevant files in `library/` and `01-foundation/`. Real customer data beats assumptions.
- **Be decisive.** Give a recommendation, not a list of options.
- **Verify facts.** Every statistic, tool claim or company detail is checked by web search, with the source noted. Never invent a number, quote or result. If it can't be confirmed, flag it with `[CHECK]`.
- **Drafts only.** Agents write drafts. People publish, send, book and pay. Never send an email, post to social media, book a venue or spend money.
- **Propose before moving or deleting.** Show a plan and wait for a yes before moving, merging, overwriting or deleting files.
- **Skimmable output.** Short sections, tables, UK English, no filler.

## 3. Privacy

- Customer names, emails and phone numbers go only in `library/customers/raw/` and `06-measurement/data/` exports. Both are blocked from GitHub by `.gitignore`.
- Everything else uses anonymised data: "Customer A, salon owner, Leeds", never a real name.
- Never paste personal data into a file outside those folders.

## 4. Folder map

| Folder | Job |
|---|---|
| `library/` | What the company already knows: customer and ICP data, past blogs, past campaigns and posters, brand assets, competitors |
| `01-foundation/` | Who we are: company profile, ideal customer, positioning, brand voice, competitors summary, offers |
| `02-strategy/` | Yearly plan, quarterly goals and KPIs, budget |
| `03-campaigns/` | One folder per live campaign; `events/` has one folder per monthly event |
| `04-content/` | Content pillars, calendar, `drafts/` and `published/` |
| `05-channels/` | How each channel works for us: SEO and AEO, email, social, paid, events |
| `06-measurement/` | KPI definitions, `data/` exports, monthly `reports/`, `experiments/` log |
| `07-operations/` | Playbooks, templates, tool stack, decisions log |
| `inbox/` | Raw notes waiting to be sorted by `/raw` |
| `logs/` | Daily session logs, `YYYY-MM-DD.md` |

**Naming:** campaigns `03-campaigns/YYYY-MM-<short-name>/`, events `03-campaigns/events/YYYY-MM-<short-name>/`, drafts `04-content/drafts/YYYY-MM-DD-<short-title>.md`, reports `06-measurement/reports/YYYY-MM.md`.

## 5. Agents

| Agent | Job | Commands |
|---|---|---|
| `content-manager` | Content that ranks on Google and gets quoted by AI answer engines (SEO + AEO) | `/content-plan`, `/content-brief`, `/refresh`, `/sync-blogs` |
| `event-organiser` | Plans and runs one event a month, from idea to follow-up | `/new-event`, `/event-status` |
| `marketing-analyst` | Turns numbers into decisions; never invents data | `/report`, `/analyse`, `/update-icp` |

They hand work to each other through files: the event organiser leaves a content request in the event folder, the content manager writes it, the analyst reports on both.

**Monthly rhythm:**
1. Week 1: `marketing-analyst` writes last month's report with 3 recommendations.
2. Week 1: `content-manager` plans next month's content; `event-organiser` confirms next month's event and starts promotion.
3. Weeks 2 to 4: content gets written; the event runs and is followed up.
4. Month end: `marketing-analyst` reports on the event and content, and the loop restarts.

## 6. Commands

| Command | What it does |
|---|---|
| `/morning-brief` | Today's priorities: live campaigns, content due, next event, open tasks |
| `/shutdown` | Logs the day in `logs/` and routes tasks into campaign files |
| `/week-recap` | Weekly review: what shipped, numbers, next week |
| `/brief [topic]` | Context before a meeting on a campaign, channel, customer type or person |
| `/raw` | Sorts `inbox/` notes into the right folders (proposes first) |
| `/lint` | Health check: empty foundation files, stale plans, campaigns without results |
| `/tactics` | Suggests tactics that fit the strategy, audience and budget |
| `/new-campaign` | Creates a campaign folder from the template |
| `/add-campaign` | Files a finished campaign in the library: brief, poster, results, lessons |
| `/sync-blogs` | Copies published blog posts from the website into `library/content/past-blogs/` |
| `/update-icp` | Updates `01-foundation/ideal-customer.md` from ICP data and interviews |
| `/content-plan` | Next month's content plan (content-manager) |
| `/content-brief [topic]` | SEO + AEO brief for one piece (content-manager) |
| `/refresh [page]` | Refreshes an old post for accuracy, SEO and AEO (content-manager) |
| `/new-event` | Plans the next monthly event (event-organiser) |
| `/event-status` | What's due this week for the next event (event-organiser) |
| `/report [month]` | Monthly marketing report (marketing-analyst) |
| `/analyse [campaign or event]` | Results of one campaign or event (marketing-analyst) |

## 7. Connectors

`<List what is connected, e.g. Google Analytics, Search Console, email platform, Apify.>` Don't assume an integration exists: check before relying on one. Without connectors, the analyst works from CSV exports in `06-measurement/data/`.

---

*Update this file as the company's conventions become clear.*
