# GRC Engineering Club blog

The club's static blog, built with [Astro](https://astro.build/) and deployed through GitHub Pages.

## Run locally

You need Node.js 24 or newer.

```sh
npm install
npm run dev
```

Then open `http://localhost:4321/blog/`.

## Publish a post

Add a Markdown file to `src/content/posts/`. Start it with:

```yaml
---
title: Your post title
description: A one-sentence summary.
published: 2026-10-11
author: Your name
tags: [projects, robotics]
draft: false
---
```

Write the post below the second `---`. Commit and push to `main`; GitHub Actions builds and deploys it automatically.

## First-time GitHub Pages setup

In the repository on GitHub, open **Settings → Pages** and set **Source** to **GitHub Actions**. The included workflow will publish to `https://grcengclub.github.io/blog/` after the next push to `main`.

## Commands

| Command | Purpose |
| --- | --- |
| `npm run dev` | Start the local development server |
| `npm run check` | Check Astro and TypeScript files |
| `npm run build` | Build the production site into `dist/` |
| `npm run preview` | Preview the production build |
