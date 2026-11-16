---
description: Copies published blog posts from the company website into the library.
---

Use the `content-manager` agent to sync the blog.

1. Read `library/content/website.md` for the blog URL and sitemap. If they're still placeholders, ask me for the URL and stop.
2. Fetch the sitemap (or the blog index if there's no sitemap) and list every blog post URL.
3. For each post not already in `library/content/past-blogs/`, fetch it and save it as `YYYY-MM-DD-<slug>.md` with frontmatter: `title`, `url`, `published`, `last_updated`, `word_count`. Keep the text and headings; drop navigation, footers and scripts.
4. Update `library/content/past-blogs/index.md`: one row per post (date, title, URL, main topic, pillar).
5. Set "Last synced" in `website.md`.

Report: new posts added, posts already there, any that failed.
