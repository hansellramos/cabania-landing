# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

CabanIA landing page — a marketing site for an AI-powered booking system for cabins/parcels (cabañas/parcelas). The product targets property owners, commission agents, and end users in Latin America.

## Architecture

This is a **single-file static site** (`index.html`). There is no build step, no bundler, no package manager, and no framework.

- **Styling**: Tailwind CSS via CDN (`cdn.tailwindcss.com`)
- **JavaScript**: Vanilla JS inline `<script>` at the bottom of the body (mobile menu toggle + dynamic year)
- **Language**: All UI copy is in **Spanish**

## Development

Open `index.html` directly in a browser or use any static file server:

```
open index.html
# or
python3 -m http.server 8000
```

There are no build, lint, or test commands.

## Page Sections

The page uses anchor-based navigation: `#beneficios`, `#ia`, `#demo`, `#modulos`, `#para-quien`, `#precios`, `#faq`, `#cta`.

## Key Conventions

- Design uses a dark theme (`bg-slate-950`) with emerald/sky gradient accents
- Layout width is constrained with `w-[min(1120px,calc(100%-40px))]`
- Cards use `rounded-2xl border border-white/15 bg-white/5` pattern consistently
- CTA buttons use `bg-gradient-to-br from-emerald-500 to-sky-500` with `text-slate-950`
- The CTA form is visual-only (no backend wired yet)
