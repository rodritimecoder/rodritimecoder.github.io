---
layout: post
title: Hello, world
date: 2026-11-18
date_display: 2026-11-18 · boot
summary: First transmission. What this box is for, and what it is not.
---

The terminal is on. This is the first post in a blog built as a Jekyll site and dressed in the `glitch-console` look — a dark terminal that moves in discrete pixels.

## What this box is for

- Notes on code, tools, and the machine.
- Short write-ups that can be read in one sitting.
- An excuse to keep the design pack honest: every colour here comes from its token sheet.

## What it is not

A newsletter, a portfolio, or a place for long essays. If a thought does not fit in a few paragraphs, it stays in the notebook.

The gates run like this:

```sh
design-pack verify _site --json
design-pack check _site --json
```

One is a static token gate. The other watches the page across seven viewports. Both treat a failure as a build error, not a suggestion.

Try the [posts index]({{ site.baseurl }}/blog.html) — it is the same archive, counted.
