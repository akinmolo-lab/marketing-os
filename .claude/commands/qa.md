---
description: QA a draft before it goes out: facts, voice, SEO/AEO, privacy, links (qa-reviewer).
argument-hint: [draft file path]
---

Use the `qa-reviewer` agent to review: $ARGUMENTS

If no file is given, list the drafts in `04-content/drafts/` and the event folders that have no `-qa.md` report yet, and ask which one to review.

It runs its `qa-check` skill, saves the report next to the draft as `<draft-name>-qa.md`, gives a verdict, and only edits the draft after a yes.
