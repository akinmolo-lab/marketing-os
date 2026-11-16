---
name: monthly-report
description: Write the monthly marketing report from real data, with 3 ranked recommendations. Use when asked for a monthly report, a marketing update, or "how did we do last month".
---

# Monthly marketing report

## Steps

1. **Data check first.** List the data available for the month (exports in `06-measurement/data/`, connectors) against every KPI in `06-measurement/kpis.md`. Show a table: KPI, available yes/no, source. If key data is missing, say what and ask whether to continue with gaps marked.
2. **KPIs.** For each KPI: this month, last month, change, target (from `02-strategy/quarterly-goals.md`), status (on track / at risk / behind).
3. **Content.** Top 3 and bottom 3 pieces by the main content KPI; any AI answer mentions (from the person's pasted checks).
4. **Campaigns and events.** One line each: goal, result, verdict. Link to their `results.md` or `report.md`.
5. **Experiments.** Results from `experiments-log.md` that finished this month.
6. **What it means.** 3–5 short insights. Say when a change is too small to read anything into.
7. **Recommendations.** Exactly 3, ranked: what, why (the evidence), owner, first step, KPI it should move.

## Output

Save to `06-measurement/reports/YYYY-MM.md`. Start with a 3-line summary: the headline, the biggest win, the biggest worry. Every figure has its source. No names or personal data.
