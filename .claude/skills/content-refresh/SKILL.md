---
name: content-refresh
description: Refresh an existing blog post: fix outdated facts, improve SEO and restructure for AI answer engines. Use when asked to update, refresh, revamp or check an old post, even if only a URL or file is given.
---

# Refresh a post

## Steps

1. **Get the post** from `library/content/past-blogs/` or fetch the URL. Never edit the original.
2. **Freshness audit** (web search for every item):
   - Statistics: still the latest? Find the current figure and source.
   - Tools and features: still exist, same name, same price?
   - Dates, years, "this year" wording.
   - Links: still working, still pointing to the right page.
   - Claims that no longer hold.
3. **AEO audit** against the checklist in `05-channels/seo-aeo.md`: answer first, question headings, quotable paragraphs, FAQ, sources, author and date.
4. **Rewrite** to `04-content/drafts/YYYY-MM-DD-refresh-<slug>.md`: the full updated post, keeping what works and the original URL.
5. **Change log** at the top of the draft: a table of every change (what, why, source).
6. Add or update the row in `04-content/content-calendar.md` with format `refresh`.

## Output

The draft path, the number of facts fixed, and the 3 biggest improvements.
