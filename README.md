# Marketing OS

A marketing operating system for a company, run with [Claude Code](https://claude.com/claude-code). Plain markdown folders hold what the company knows and what it's doing; three AI agents and 18 commands run the daily, weekly and monthly marketing work on top of them.

## What's inside

| Layer | Folder | What it holds |
|---|---|---|
| Library | `library/` | Customer and ICP data, past blogs, past campaigns and posters, brand assets, competitors |
| 1. Foundation | `01-foundation/` | Company profile, ideal customer, positioning, brand voice, offers |
| 2. Strategy | `02-strategy/` | Yearly plan, quarterly goals, budget |
| 3. Campaigns | `03-campaigns/` | One folder per campaign; `events/` for monthly events |
| 4. Content | `04-content/` | Pillars, calendar, drafts, published |
| 5. Channels | `05-channels/` | SEO and AEO, email, social, paid, events |
| 6. Measurement | `06-measurement/` | KPIs, data exports, monthly reports, experiments |
| 7. Operations | `07-operations/` | Playbooks, templates, tools, decisions |
| AI layer | `.claude/` | Agents, commands, skills |

## The agents

| Agent | Job |
|---|---|
| **Content Manager** | Plans, writes and refreshes content that ranks on Google and gets quoted by ChatGPT, Perplexity, Gemini and Google AI Overviews |
| **Event Organiser** | Plans and runs one event a month: theme, run-of-show, landing page, promotion, reminders, follow-up, report |
| **Marketing Analyst** | Monthly reports, campaign and event results, content performance, experiments; never invents a number |

## Getting started

1. **Make your own copy.** Click **Use this template** (top of this page) → **Create a new repository**, and set your copy to **Private**: it will hold your company's strategy and customer insights. Then clone your copy and open it in [Claude Code](https://claude.com/claude-code).
2. **Fill in the company:** section 1 of `CLAUDE.md`, then the six files in `01-foundation/`. Or ask Claude: *"Interview me to fill in the foundation files."*
3. **Load the library:**
   - Add the website and blog URL to `library/content/website.md`, then run `/sync-blogs`.
   - Put raw customer exports in `library/customers/raw/` (never uploaded), then run `/update-icp`.
   - File past campaigns with `/add-campaign`, including their posters.
4. **Set the strategy:** fill in `02-strategy/` with this year's goals.
5. **Start the loop:** `/morning-brief` each day, `/week-recap` each Friday, `/report` at the start of each month.

## Commands

| Daily and weekly | Campaigns and library | Agents |
|---|---|---|
| `/morning-brief` | `/new-campaign` | `/content-plan` |
| `/shutdown` | `/add-campaign` | `/content-brief [topic]` |
| `/week-recap` | `/sync-blogs` | `/refresh [page]` |
| `/brief [topic]` | `/update-icp` | `/new-event` |
| `/raw` | `/tactics` | `/event-status` |
| `/lint` | | `/report [month]`, `/analyse [name]` |

## Rules the system follows

- **Drafts only.** Agents never publish, send emails, book or pay. People do.
- **Facts are checked** by web search, with sources. Numbers come only from real data.
- **Privacy.** Raw customer data stays in `library/customers/raw/` and `06-measurement/data/`, which `.gitignore` keeps off GitHub. Everything committed is anonymised.
- **This template is public; your copy shouldn't be.** Once you fill it in with your company's details, keep your repository private.

Full operating rules: [CLAUDE.md](CLAUDE.md).
