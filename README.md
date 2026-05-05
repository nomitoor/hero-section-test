# The Atelier — Hero Section

A refined, editorial-style hero section built with [Astro](https://astro.build). Designed for a high-end coaching studio ("The Atelier"), the layout features a full-bleed background image, typographic hierarchy using Cormorant Garamond and Inter, staggered fade-up entrance animations, and a fully responsive layout.

## Preview

The hero renders a 16:9 full-bleed composition with:

- **Heading** — Cormorant Garamond, large serif display type
- **Body copy** — German-language coaching positioning text
- **Keyword strip** — spaced small-caps tags separated by a thin rule
- **CTA button** — gold-toned ("Erstgespräch buchen") with hover transition
- **Vignette overlay** — subtle radial gradient to anchor the composition
- **Staggered animations** — each element fades and rises in sequence on load

## Project Structure

```text
/
├── public/
│   ├── subject.png          # Hero background image
│   └── favicon.svg / .ico
├── src/
│   ├── pages/
│   │   └── index.astro      # Single-page hero layout
│   └── styles/
│       └── global.css       # Global resets / base styles
└── package.json
```

## Tech Stack

| Tool | Version |
| :--- | :------ |
| [Astro](https://astro.build) | ^6.2.2 |
| [Tailwind CSS](https://tailwindcss.com) | ^4.2.4 (via `@tailwindcss/vite`) |
| Node.js | >=22.12.0 |

Fonts loaded via Google Fonts: **Cormorant Garamond** (300, 400, italic) and **Inter** (300, 400).

## Getting Started

```sh
npm install
npm run dev
```

The dev server starts at `http://localhost:4321`.

## Commands

| Command | Action |
| :------------------------ | :----------------------------------------------- |
| `npm install` | Install dependencies |
| `npm run dev` | Start local dev server at `localhost:4321` |
| `npm run build` | Build production site to `./dist/` |
| `npm run preview` | Preview the production build locally |
| `npm run astro ...` | Run Astro CLI commands |

## Design Notes

- Background image is positioned at `60% center` on desktop, shifting to `68% center` on mobile to keep the subject visible.
- On screens narrower than 640 px the hero switches from a fixed 16:9 aspect ratio to full-viewport-height (`100svh`) and overlays a warm gradient behind the text for legibility.
- Color palette is anchored around deep espresso (`#1c1008`) and antique gold (`#8a7040`).
