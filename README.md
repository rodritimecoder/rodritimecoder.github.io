# The Terminal Notebook

A GitHub Pages blog built with Jekyll and the `glitch-console` design-pack look.

## Publish

1. Push to a GitHub repository under `rodritimecoder`.
2. Settings → Pages → Build and deployment → Source: **Deploy from a branch**,
   branch `main`, folder `/ (root)`.
3. Leave `baseurl: ""` for a user site (`username.github.io`). For a project site
   (`username.github.io/<repo>`), set `baseurl: "/<repo>"` in `_config.yml`.

## Write a post

Add `_posts/YYYY-MM-DD-slug.md` with frontmatter:

```yaml
---
layout: post
title: A title
date: 2026-11-18
date_display: 2026-11-18 · a short tag
summary: One line shown in the archive.
---
```

The index and post index pick posts up automatically from `site.posts`.

## Design gates

The design is not "close enough" — it is checked:

```sh
design-pack verify _site          # static token conformance (strict)
design-pack check  _site          # 7 viewports, overlap, clipping, keyboard, ≤100ms, ≥3:1
```

`tokens.css` is copied verbatim from the look. Do not edit it in this repo; add
site layout in `assets/css/blog.css` using `var(--token)` only.

## Local preview

GitHub Pages builds the Jekyll site on push. This machine has no Ruby, so a
temporary renderer was used during development to produce `_site/` for the gates;
it is not part of the repo. To preview locally with the real toolchain, install
Ruby + Bundler and run `bundle exec jekyll serve`.
