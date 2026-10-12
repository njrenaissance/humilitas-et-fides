# Humilitas et Fides

A personal blog by Jonathan Phillips, built with [Jekyll](https://jekyllrb.com/) and hosted on GitHub Pages.

**Live site:** https://njrenaissance.github.io/humilitas-et-fides/

## Structure

```
.
├── _config.yml      # Site settings (title, baseurl, theme, plugins)
├── _posts/          # Published posts: YYYY-MM-DD-title.md
├── drafts/          # Excluded from the build (still visible on GitHub; repo is public)
├── index.md         # Home page (lists posts)
├── about.md         # About page
└── README.md
```

## Writing a post

Create a file in `_posts/` named `YYYY-MM-DD-title-in-kebab-case.md` with this front matter:

```yaml
---
layout: post
title: "Post Title"
date: 2026-10-12 12:00:00 -0400
---
```

Write the body in Markdown below the front matter.

- Jekyll skips posts dated in the future, so a future date acts as a scheduled post.
- Pushing to `main` triggers a rebuild; changes go live in roughly 1 to 3 minutes.

## Workflow

Posts are drafted and edited in conversation with Claude, then committed to `_posts/` on `main` when approved for publication.

## Local preview (optional)

```bash
gem install bundler jekyll
jekyll serve
```

Then open http://localhost:4000/humilitas-et-fides/.

## Theme

[minima](https://github.com/jekyll/minima), the Jekyll default, with `jekyll-feed` and `jekyll-seo-tag`.
