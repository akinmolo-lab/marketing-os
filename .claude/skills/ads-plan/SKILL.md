---
name: ads-plan
description: Plan a paid ads campaign on Google Ads, Meta (Facebook and Instagram) or LinkedIn: platform choice, audience, campaign structure, budget split, conversion tracking and launch checklist. Use when asked to plan, set up or restructure a paid campaign, choose an ad platform, or split an ads budget.
---

# Plan a paid ads campaign

## Steps

1. **Brief.** If no campaign folder exists, create one: copy `03-campaigns/_campaign-template/` to `03-campaigns/YYYY-MM-<short-name>/` and fill in `brief.md`. Ask (in one message) for anything you can't infer: goal, offer, budget, dates, landing page.
2. **Goal and maths.** Turn the goal into numbers: target leads, the highest cost per lead (CPL) the business can afford (from offer price and close rate in `offers.md` or past campaigns), and the budget that implies. If budget and goal don't fit, say so now.
3. **Platform.** Recommend one main platform (two at most for small budgets) and say why:
   - **Google Search:** people already searching for the service. Best for high intent.
   - **Meta (Facebook / Instagram):** local consumers and small business owners, visual offers, retargeting.
   - **LinkedIn:** reaching specific job titles or industries in B2B. Higher cost per click; needs a higher-value offer.
4. **Audience.** From `ideal-customer.md`: keywords (Google) or targeting (location, interests, job titles, industries, company size), exclusions, and retargeting audiences. Customer-list audiences are described, never listed.
5. **Structure.** Campaign → ad sets / ad groups → ads. Keep it simple: 1 campaign, 2–3 ad sets testing one variable (audience or angle), 2–3 ads each.
6. **Budget.** Daily budget per ad set, test period (default 2 weeks), and the rule for judging a test (e.g. "at least 1,000 impressions and 2× target CPL spent per ad before pausing it"). Total must stay inside the paid ads line in `02-strategy/budget.md`.
7. **Tracking.** Conversion event, pixel or tag needed, UTM convention (`utm_source`, `utm_medium=paid`, `utm_campaign=<folder short-name>`), and where results are exported to (`06-measurement/data/`).
8. **Benchmarks.** If useful, find current benchmark CTR and CPL for the platform and industry by web search. Label them as benchmarks with the source and date; never as our numbers.

## Write `ads-plan.md` in the campaign folder

| Section | Content |
|---|---|
| Goal and maths | Target leads, max CPL, budget, the calculation |
| Platform | Choice and why |
| Audience | Targeting, keywords, exclusions, retargeting |
| Structure | Table: campaign, ad set / ad group, audience, daily budget, ads |
| Test rules | Test period, when to judge, when to pause, when to scale |
| Tracking | Conversion, pixel / tag, UTMs, data export |
| Launch checklist | See below |

## Launch checklist (for a person)

- [ ] Offer and landing page live, and checked with `/qa`
- [ ] Conversion tracking installed and tested with a real test conversion
- [ ] UTMs on every ad URL
- [ ] Ad copy approved after `/qa`
- [ ] Budgets and end date set exactly as in `ads-plan.md`
- [ ] Payment method and spend limit set by a person
- [ ] Ads turned on by a person; date added to `brief.md`
- [ ] First check booked for 3 days after launch (`/ads-check`)

## Output

The folder path, the plan summary, the budget maths, and the tasks a person must do with dates. Then suggest running the `ad-copy` skill.
