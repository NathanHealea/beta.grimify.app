<div align="center">

# Color Wheel

**An interactive color wheel for miniature paints.**

Visualize, compare, and explore 190+ hobby paints across major brands — mapped by hue and lightness on a single interactive canvas.

[![Status](https://img.shields.io/badge/status-beta-orange)](#beta-notice)
[![Version](https://img.shields.io/badge/version-0.13.2-blue)](./package.json)
[![Next.js](https://img.shields.io/badge/Next.js-16-black)](https://nextjs.org)
[![React](https://img.shields.io/badge/React-19-61dafb)](https://react.dev)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178c6)](https://www.typescriptlang.org)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-4-38bdf8)](https://tailwindcss.com)
[![DaisyUI](https://img.shields.io/badge/DaisyUI-5-5a0ef8)](https://daisyui.com)

</div>

---

## Beta Notice

This is the **beta release** of Color Wheel. Features, data, and UI are evolving rapidly — expect breaking changes between releases. Feedback and bug reports are welcome.

## About

Color Wheel is built for miniature painters who want to make smarter color choices. It maps 190+ paints from **Vallejo**, **Green Stuff World**, **Citadel**, **Army Painter**, and **AK Interactive** onto an SVG-based circular visualization, with paints positioned by **hue** (angle) and **lightness** (radius).

It helps hobbyists:

- **Visualize** their paint collection on an interactive color wheel
- **Compare** paints across brands to find duplicates and alternatives
- **Explore** color relationships using complementary, split-complementary, and analogous schemes
- **Search** paints by name, hex code, or brand
- **Track** their owned paints with a personal collection layer

## Features

| Area                          | Highlights                                                                              |
| ----------------------------- | --------------------------------------------------------------------------------------- |
| **Color Wheel Visualization** | Interactive SVG wheel with zoom, pan, reset; paint selection, hover, overlap indicators |
| **Multiple Views**            | Wheel, Grid, and List modes for different browsing styles                               |
| **Brand Tools**               | Brand filtering, ring toggles, and legend for cross-brand comparison                    |
| **Color Analysis**            | Complementary, split-complementary, and analogous scheme modes                          |
| **Search**                    | Fast lookup by paint name, hex code, or brand                                           |
| **Paint Collection**          | Mark owned paints and filter the wheel by your collection (localStorage)                |
| **Detail Panel**              | Sidebar with full paint metadata for any selected color                                 |

## Tech Stack

| Layer             | Technology                              |
| ----------------- | --------------------------------------- |
| **Framework**     | Next.js (App Router), React, TypeScript |
| **Styling**       | Tailwind CSS, DaisyUI                   |
| **UI Components** | Headless UI, Heroicons                  |
| **State**         | Zustand                                 |

## Getting Started

### Prerequisites

- Node.js 20+ (or Bun)
- A package manager: `bun`, `pnpm`, `yarn`, or `npm`

### Install & Run

```bash
# install dependencies
bun install   # or: pnpm install / yarn / npm install

# start the dev server
bun dev       # or: pnpm dev / yarn dev / npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the app.

### Available Scripts

| Script         | Purpose                          |
| -------------- | -------------------------------- |
| `bun dev`      | Start the Next.js dev server     |
| `bun build`    | Create a production build        |
| `bun start`    | Run the production build locally |
| `bun lint`     | Run ESLint                       |

## Project Structure

```
src/
├── app/          # Next.js app router pages and layouts
├── components/   # UI components (wheel, sidebar, controls, etc.)
├── data/         # Paint datasets per brand (JSON)
└── lib/          # Color math, hooks, state (Zustand stores)

docs/             # Feature plans, epics, and implementation notes
```

## Roadmap

Color Wheel ships in epics. The full breakdown lives in [`docs/overview.md`](./docs/overview.md).

### Shipped

- Paint Database (190+ paints across 5 brands)
- Color Wheel Visualization (Wheel / Grid / List)
- Sidebar Layout & Header Stats
- Detail Panel
- Brand Filtering, Ring Toggle, Legend
- Color Scheme Modes & Search
- Owned Paint Collection

### In Progress / Planned

- **User Authentication** — Supabase-backed accounts, social login, profiles, role-based authorization
- **Recipes** — Step-by-step paint recipes, projects, tags, and community sharing
- **SEO & Branding** — Branding assets, metadata, sitemap

## Documentation

- [Project Overview](./docs/overview.md) — epics, status, and feature index
- Per-feature plans live under `docs/<epic>/<feature>.md`

## Contributing

This is a personal project in active beta development. If you find a bug, have a paint to add, or want to suggest a feature, open an issue.

## Acknowledgements

- Paint data curated from manufacturer ranges and community references including [PaintPad.app](https://paintpad.app)
- Bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app)
