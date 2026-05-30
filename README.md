# Zichen Zhu Academic Site

This is a GitHub Pages site with two parts:

- an academic homepage at `/`
- a blog archive at `/blog/`

## Edit The Homepage

Update `index.html` with your real introduction, links, research interests, news,
and selected work.

Replace these placeholders:

- `your.email@example.com`
- the research-interest sentence
- the selected-work example
- `/files/cv.pdf`, if you want to publish a CV
- `/assets/images/profile.jpg`, after adding a profile photo

## Add A Blog Post

Create a Markdown file in `_posts` with this filename format:

```text
YYYY-MM-DD-post-title.md
```

Example:

```text
_posts/2026-06-01-reading-notes.md
```

Use this front matter:

```markdown
---
layout: post
title: "Reading Notes"
date: 2026-06-01
description: "Optional short summary."
---

Write your post here.
```

The blog page updates automatically.

## Publish

```bash
git add .
git commit -m "Initial academic site with blog"
git push
```

GitHub Pages will serve the site at:

```text
https://zichenzhu.github.io/
```
