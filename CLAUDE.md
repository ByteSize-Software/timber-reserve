# CLAUDE.md

Guidance for Claude Code when working in this repository.

## Commands
```bash
npm run dev      # Start dev server at localhost:4321
npm run build    # Production build to ./dist/
npm run preview  # Preview production build
```

No lint or test commands configured.

## Tech Stack

- Astro v6 — file-based routing, `.astro` components
- Tailwind CSS v4 — via `@import "tailwindcss"` in `src/styles/global.css`
- TypeScript strict mode
- Vercel adapter for edge deployment
- Node.js >=22.12.0

## Architecture

- Pages in `src/pages/` map to routes (`index.astro` → `/`)
- All pages extend `src/layouts/BaseLayout.astro` (HTML shell, nav, footer)
- Components go in `src/components/`

## Style Rules

- **Always use Tailwind utility classes** — no inline styles or custom CSS unless absolutely necessary