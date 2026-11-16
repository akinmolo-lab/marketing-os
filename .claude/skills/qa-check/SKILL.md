---
name: qa-check
description: Review a draft before it is published or sent: verify every fact by web search, check brand voice, SEO and AEO, privacy, offers and links, then give a verdict. Use when asked to QA, fact-check, proofread, review or sanity-check a draft, or before anything in 04-content/drafts/ or an event folder goes out.
---

# QA check

## Steps

1. **Identify the draft.** Its type (article, landing page, email, social post, event promo), its goal and its source brief. Read the whole draft before judging any part.
2. **Facts.** List every checkable claim: statistics, quotes, dates, prices, tool features, company details, research. Web-search each one. Record: claim, verdict (correct / wrong / can't confirm / outdated), source link, fix. Anything that can't be confirmed is a blocker until it's cut or sourced.
3. **Offers and events.** Prices, dates, times, links and what's included must match `01-foundation/offers.md` or the event's `event-plan.md` word for word.
4. **Privacy.** Search for real names, emails, phone numbers, company names of customers, and identifiable details. Any found outside the raw data folders is a blocker.
5. **Brand voice.** Check against `01-foundation/brand-voice.md`: tone, reading level, UK English, banned words. Quote the line and suggest the fix.
6. **SEO and AEO** (articles and pages only). Main question answered in the first 2–3 sentences; question-style headings; one clear idea per section; FAQ where useful; title and meta description present; internal links to past posts in `library/content/past-blogs/`; sources cited.
7. **Links and calls to action.** Every link has a real destination (no placeholders like `<link>`); the call to action matches the goal in the brief.
8. **Basics.** Spelling, grammar, repeated words, length against the brief or channel limit.

## Output

Save the report next to the draft as `<draft-name>-qa.md`:

```
# QA: <draft title>
Verdict: Ready | Ready after fixes | Not ready
Date: <today>

## Blockers
| # | Where | Problem | Fix | Source |

## Should fix
| # | Where | Problem | Fix |

## Nice to have
- ...

## Facts checked
| Claim | Verdict | Source |
```

Then ask which fixes to apply. On a yes, edit the draft, tick off each fix in the report, and never touch anything not approved.

## Rules

Never invent a source. Never publish or send. Don't rewrite the draft for taste: report problems, not preferences.
