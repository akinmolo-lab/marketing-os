---
description: Weekly check of live paid ads: what to pause, keep, scale or test (campaign-manager).
argument-hint: [campaign folder, optional]
---

Use the `campaign-manager` agent to check: $ARGUMENTS (default: every campaign in `03-campaigns/` with `status: live` and an `ads-plan.md`).

It runs its `ads-optimise` skill, adds a dated entry to the campaign's `optimisation-log.md`, and lists the exact changes for a person to make in the ad platform.
