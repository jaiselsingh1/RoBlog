---
title: "FAQ"
url: "/faq/"
summary: "Publishing notes for the site"
---

## How do I add a post?

Add a Markdown file or page bundle under `content/posts/`. The recommended structure is:

```text
content/posts/YYYY-MM-DD-topic-name/index.md
```

Set `draft: false` when the post is ready to publish.

## How do I add tags?

Add tags in the post front matter:

```yaml
tags:
  - reinforcement-learning
  - robotics
```

Hugo builds the tag pages automatically.

## How do co-authors work?

Add every post author in front matter:

```yaml
author:
  - Jaisel Singh
  - Ben Evans
```

Ben Evans is listed as an invited co-author for this site.

## How does publishing work?

Push to the `main` branch. The GitHub Actions workflow builds the Hugo site and deploys it to GitHub Pages.
