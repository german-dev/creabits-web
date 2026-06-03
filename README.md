# CREABITS · web

### *Cada bit cuenta*

![version](https://img.shields.io/badge/version-0000.0001-FFEBC2?style=flat-square&labelColor=1B2C36)
![uptime](https://img.shields.io/badge/uptime-experimentando-F2C879?style=flat-square&labelColor=1B2C36)
![built](https://img.shields.io/badge/built-in_the_open-99D1FF?style=flat-square&labelColor=1B2C36)

The website for CREABITS — a lab, a public wiki, a playground and a portfolio, built by two people in the open. This repo *is* the site: unfinished on purpose, documented as it goes. You're looking at the work while it happens, not at a finished product.

We're not experts and don't pretend to be. We're amateurs in the old sense of the word — *from the Latin* amator*: those who do it for love.* Expect things in progress, things that broke, and notes on what we learned fixing them.

## Stack

- **Framework** — [Astro](https://astro.build/): island architecture, zero-JS by default.
- **Styling** — [Tailwind CSS v4](https://tailwindcss.com/): CSS-first config, no `tailwind.config.js`.
- **Language** — TypeScript (strict mode).
- **Content** — MDX + Astro Content Collections, typed with Zod.
- **Hosting** — [Cloudflare Pages](https://pages.cloudflare.com/): deployed on the edge.

> Versions are pinned in `package.json` — that's the source of truth, not this list.

## Structure

```text
creabits/
├── src/
│   ├── assets/       # static assets + self-hosted fonts (Roboto Serif, Martian Mono)
│   ├── components/   # UI system — core components & compound blocks
│   ├── content/      # content collections (wiki, labs, notes)
│   ├── layouts/      # base, post, documentation templates
│   ├── pages/        # file-based routing
│   └── styles/       # global.css — design tokens + Tailwind v4 entry
└── astro.config.mjs  # Astro + Cloudflare config
```

## Running locally

```bash
npm install
npm run dev      # local dev server
npm run build    # production build
npm run preview  # preview the build
```

## Design system

The visual language (two typographic voices, color tokens, the five states, the dot motif) lives in `src/styles/global.css` and is documented in the brand system. Two rules to keep it coherent:

- **Two voices, never three.** Serif (Roboto Serif) = a person speaking. Mono (Martian Mono) = the machine speaking.
- **Colors only from tokens.** If a color isn't in `@theme`, it doesn't go in the UI.

## A note on state

Every page and section declares its state: `aprendiendo`, `experimentando`, `documentando`, `iterando`, `depurando`. It's not decoration — it tells the reader how finished a thing is, honestly. `depurando` only shows up when something is actually broken.

## What you won't find here

Promises of completeness. This is a learning space; the structure is solid, the content keeps moving. If you leave with more questions than answers, it worked.

---

*Built in the open · uptime: experimentando*
**P.D. Sitio siempre en construcción.**
