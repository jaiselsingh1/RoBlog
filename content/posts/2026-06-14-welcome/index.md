---
title: "Welcome to the Notes"
date: 2026-06-14T18:35:00-07:00
draft: false
summary: "A starter post showing how Markdown entries become published blog posts."
tags:
  - meta
  - hugo
  - github-pages
categories:
  - site notes
author:
  - Jaisel Singh
  - Ben Evans
ShowToc: true
TocOpen: false
---

This repository is set up so each Markdown file in `content/posts/` becomes a blog post.

The pattern is intentionally close to Lilian Weng's public blog setup: Hugo generates the site, PaperMod provides the clean reading layout, and GitHub Pages serves the built files.

## Authoring loop

Create a new post with Hugo:

```bash
hugo new content posts/2026-06-14-my-topic/index.md
```

Then update the front matter, write the body in Markdown, set `draft: false`, and push to `main`.

## Co-authored posts

Use the `author` field when a post has multiple authors:

```yaml
author:
  - Jaisel Singh
  - Ben Evans
```

Both authors are included in the site metadata and linked from the Authors page.
