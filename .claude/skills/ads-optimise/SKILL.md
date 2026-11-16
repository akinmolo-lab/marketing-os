---
name: ads-optimise
description: Weekly check of a live paid ads campaign: compare spend, clicks, leads and cost per lead against the plan, then recommend what to pause, keep, scale or test next. Use when asked how ads are doing, to optimise a campaign, review ad spend, or for a weekly ads check.
---

# Weekly ads check

Work in the campaign folder. Read `brief.md`, `ads-plan.md` (targets and test rules) and `optimisation-log.md` (past changes).

## Steps

1. **Data.** Find the latest export in `06-measurement/data/` (or a connected ads platform; check it exists first). If there's no data, stop and ask a person to export: date range, spend, impressions, clicks, conversions, by campaign, ad set and ad. Name the file to save it as: `YYYY-MM-DD-<short-name>-ads.csv`.
2. **Numbers.** Per ad set and ad: spend, impressions, CTR, cost per click, conversions, conversion rate, CPL. Total spend vs budget so far and pace to the end date. Every figure names its source file.
3. **Judge with the test rules in `ads-plan.md`.** Only judge ads that have passed the threshold; mark the rest "too early".
   - **Pause:** spent 2× target CPL with no lead, or CPL well above target after the threshold.
   - **Keep:** near target, still learning.
   - **Scale:** CPL below target with enough leads to trust it. Suggest raising budget by no more than 20–30% at a time.
   - **Test next:** one new variable (angle, audience or landing page), never several at once.
4. **Check the funnel.** High CTR but few leads points at the landing page or tracking; low CTR points at the ad or audience. Say which.
5. **Lead quality.** Ask whether leads were good (a person knows; the data doesn't). Note the answer.

## Write

- Add a dated entry to `optimisation-log.md`: numbers summary, decisions, and the exact changes for a person to make in the ad platform (setting, from, to).
- Any test worth keeping goes into `06-measurement/experiments/experiments-log.md`.

## Output (under 250 words)

| Section | Content |
|---|---|
| **Headline** | On track / behind / ahead, in one line |
| **Numbers** | Spend vs budget, leads, CPL vs target |
| **Changes for a person** | Pause / scale / test, each with exact setting |
| **Next check** | Date |

## Rules

Real numbers only, each with its source. Never make changes in an ad account. Small numbers are noisy: say when a difference is too small to act on. No personal data from lead lists in any file.
