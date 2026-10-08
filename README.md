# safatash.com

Personal site of Safa Damouzehtash, built with [Astro](https://astro.build).

## Run locally

```
npm install
npm run dev
```

## Write a blog post

Add a Markdown file to `src/content/blog/`:

```md
---
title: Post title
description: One-sentence summary shown on cards and in search results.
tag: Security
pubDate: 2026-10-20
draft: false
---

Post body in Markdown.
```

Set `draft: true` to keep a post off the live site. When an idea in
`src/data/upcoming.ts` gets published, remove it from that list.

## Deploy

The site is static and deploys on Vercel. Every push to `main` triggers a new deployment.
