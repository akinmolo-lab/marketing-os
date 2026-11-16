---
description: Health check of the marketing OS. Finds gaps, stale plans and missing results. Reports first.
---

Run a health check and report. Fix nothing until I confirm.

Check:
1. **Foundation gaps:** placeholders (`<...>`) still in `CLAUDE.md` section 1 or `01-foundation/`.
2. **Stale ICP:** `ideal-customer.md` not updated in 90 days, or new files in `library/customers/` since the last update.
3. **Campaigns:** status `live` past their end date; `finished` campaigns without `results.md` filled in; finished campaigns not filed in `library/campaigns/`.
4. **Events:** next month has no event folder; past events without `report.md`.
5. **Content:** calendar items overdue; drafts older than 30 days; blog not synced in 30 days (`library/content/website.md`).
6. **Measurement:** last month's report missing; KPIs in goals that aren't defined in `06-measurement/kpis.md`.
7. **Privacy:** any email address or phone number outside `library/customers/raw/` and `06-measurement/data/`.

Output a table: check, finding, file, suggested fix, severity (must / should / nice). Privacy findings are always "must".
