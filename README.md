# Zichen Zhu Academic Site

This is a GitHub Pages site with two parts:

- an academic homepage at `/`
- a blog archive at `/blog/`

## Edit The Homepage

`index.html` holds the introduction, links, research interests, news, selected work,
experience, education, and skills. Keep it in sync with the CV at
`files/ZichenZhu_Resume.pdf`, and replace `assets/images/profile.jpg` to change the
profile photo.

## Add A Blog Post

Create a Markdown file in `_posts` named `YYYY-MM-DD-post-title.md`. Keep the
**filename in ASCII** even for a Chinese post — the filename becomes the URL, and
Chinese characters get percent-encoded into unreadable links. The Chinese title goes
in the front matter.

```markdown
---
title: "星集可达性入门"
date: 2026-09-01
lang: zh
category: technical
tags: [verification, spiking-networks]
description: "Optional one-line summary, shown on the blog index."
---

Write your post here.
```

Three fields carry the taxonomy:

- `lang` — `en` or `zh`. Not a topic, but a property of the post: it sets
  `<html lang>` for correct CJK line-breaking and font fallback, and it drives the
  language filter on `/blog/`. Defaults to `en`.
- `category` — `technical` or `notes` (personal, travel, reading, reflections).
  Exactly one per post. Defaults to `notes`.
- `tags` — free-form topics, as many as you like. Keep language and
  technical/notes out of here; the two fields above already cover them.

`layout: post` is applied automatically, so posts do not need to declare it. The
defaults live in `_config.yml`, and the blog index filters posts client-side, so no
Jekyll plugins are required.

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
