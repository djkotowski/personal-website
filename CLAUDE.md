# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

This project uses **pnpm** — pinned via `packageManager` in `package.json` (enable it with `corepack enable`). Use `pnpm`, not `npm` or `yarn`.

- `pnpm dev` — start the Vite dev server
- `pnpm build` — production build to `dist/`
- `pnpm preview` — serve the production build locally
- `pnpm check` — type-check with `svelte-check` (the only "lint"/CI gate; there is no ESLint/Prettier and no test suite)

`pnpm check` runs automatically on `git commit` via the Husky `pre-commit` hook, and on every PR / push to `main` via the `ci-test` workflow. There are no unit tests, so `pnpm check` is the check to run before considering a change done.

## Architecture

A single-page, statically-generated personal résumé site — no router, no backend, no data fetching. Everything is hardcoded content in Svelte components.

- **Entry:** `src/main.ts` mounts `App.svelte` into `#app` (see `index.html`) using Svelte 5's `mount()`.
- **Composition:** `App.svelte` stacks four page **sections** from `src/lib/`: `HeaderSection`, `SkillsSection`, `ExpSection`, `ContactSection`. Adding/reordering page content happens here.
- **Reusable primitives** live in `src/lib/components/` (`Header`, `Hero`, `Link`) and `src/lib/icons/`. Sections compose these; primitives hold no page-specific content.
- Résumé text (skills, experience, contact info) is written inline in the section components — edit the relevant `*Section.svelte` file to change site content.

## Conventions

- **Svelte 5 runes syntax** throughout: props via `let { ... } = $props()`, slots via `{@render children?.()}`. Do not use legacy `export let` / `<slot>`.
- Prefer `<script lang="ts">` with a typed props object for new components (see `components/Link.svelte`, `components/Hero.svelte`). Some older section files use plain `<script>` — match the file you are editing.
- **Tailwind CSS v4** with **no config file**. It is enabled via the `@tailwindcss/vite` plugin and `@import "tailwindcss"` in `src/app.css`; customize through CSS, not a `tailwind.config.js`. `tailwind-merge` is available for conditional class composition.
- Styling is Tailwind utility classes in markup; the dark theme base (`bg-gray-950 text-white`) is set on `<body>` in `index.html`.
- `checkJs` is on and `.js`/`.svelte` files are type-checked — keep JSDoc/types valid so `pnpm check` passes.

## Deploy

Pushing to `main` triggers the `deploy` workflow: `pnpm build` → upload `dist/` → GitHub Pages (https://dankotowski.dev). CI reads its Node version from `.tool-versions` (pinned to 22.14.0), matching local dev — pnpm 11 requires Node >=22.13.
