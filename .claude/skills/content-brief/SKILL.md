---
name: content-brief
description: Write an SEO and AEO content brief for one article. Use when asked for a brief, an outline, or "what should this post cover", even if only a topic or question is given.
---

# Content brief

## Steps

1. **Read** the content manager's required files, and check `library/content/past-blogs/` for overlap. If a close post exists, recommend a refresh instead and stop.
2. **Research** with web search:
   - The top 5 Google results for the main question: what they cover, what they miss.
   - Related questions ("People also ask", forums).
   - What AI answer engines currently say (search the question and note which sources get cited, if visible).
3. **Write the brief** to `04-content/drafts/YYYY-MM-DD-brief-<slug>.md`:

```
---
type: brief
status: brief
target_question: <main question>
pillar: <pillar>
persona: <persona>
---

# Brief: <working title>

| | |
|---|---|
| Main question | |
| Answer in one sentence | (goes in the first 2–3 sentences) |
| Search intent | learn / compare / buy |
| Related questions | (become H2s or FAQs) |
| Angle | what we say that the top results don't |
| Proof to include | customer stories, data (with sources) |
| Internal links | past posts to link to and from |
| Call to action | from offers.md |
| Length | (match the intent, not a word target) |

## Outline
H1, H2s as questions, FAQ section.

## Sources
```

4. Update the calendar row to status `brief`.
