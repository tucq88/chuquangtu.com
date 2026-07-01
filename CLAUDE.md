# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

The personal landing page for **Tu Chu** (tucq88), deployed at **chuquangtu.com**. It is a
single-page site that mirrors the content of the existing Carrd page at
https://chuquangtu.carrd.co — bio, profile image, and links out to social/writing profiles and a CV.

The site is being (re)built as **plain static HTML/CSS/JS** — no build step, no framework.
The page should be openable directly in a browser and hostable on any static host
(GitHub Pages / Netlify / Cloudflare Pages).

## Canonical content (source of truth)

The page content mirrors chuquangtu.carrd.co. When adding or editing content, keep it in sync:

- **Name:** Tu Chu
- **Tagline:** "A curious geek who diving in technology, entrepreneurship & leadership"
- **Links:**
  - Twitter — https://twitter.com/tucq88
  - GitHub — https://github.com/tucq88
  - LinkedIn — https://linkedin.com/in/tuchuquang
  - Medium (Writing) — https://medium.com/@tucq88
  - CV — Dropbox PDF (tucq.cv.YYYY.pdf)

## Structure

```
index.html            # the whole page — markup + content
assets/css/style.css  # all styling; light/dark via prefers-color-scheme; CSS vars at :root
assets/js/main.js     # tiny progressive enhancement (footer year); page works without JS
assets/images/        # avatar.jpg (rescued from the old Hugo site)
```

Social icons are inline SVG in `index.html` (no icon-font/CDN dependency). The former Hugo
site (goa theme) has been removed from the repo.

## Development

No toolchain or build step — open `index.html` in a browser, or serve the directory statically:

```
python3 -m http.server        # then visit http://localhost:8000
```
