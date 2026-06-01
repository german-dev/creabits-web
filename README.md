# CREABITS | Technical Architecture

The official repository for CREABITS. A premium digital studio, shared knowledge system, and performance laboratory engineered for extreme scalability, speed, and zero-frictional workflow.

## 🚀 Tech Stack

- **Framework:** [Astro 6](https://astro.build/) — Island Architecture (Zero-JS by default)
- **Styling:** [Tailwind CSS v4](https://tailwindcss.com/) — Next-gen utility-first CSS driven by Lightning CSS
- **Language:** TypeScript (Strict Mode Enabled)
- **Infrastructure:** [Cloudflare Pages](https://pages.cloudflare.com/) — Globally distributed Edge Network
- **Content:** MDX + Astro Content Collections (Strictly typed with Zod)

## 📦 Repository Structure

```text
creabits/
├── src/
│   ├── assets/       # Optimized global static assets and local fonts
│   ├── components/   # Atomic UI system (core components & compound blocks)
│   ├── content/      # Content Collections (Blog, Technical Wiki, Labs)
│   ├── layouts/      # Master templates (Base, Post, Documentation)
│   ├── pages/        # File-based routing engine
│   └── styles/       # Global CSS entry point for Tailwind v4
└── astro.config.mjs  # Astro configuration & Cloudflare SSR integration
