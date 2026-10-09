# SolidStart Template

A starter template for [bolt.diy](https://github.com/stackblitz-labs/bolt.diy).

## Purpose

This template is designed for use with **<https://github.com/stackblitz-labs/bolt.diy>**. bolt.diy fetches
these files at runtime and imports them into a fresh WebContainer project when you ask for a Solid project,
so everything here needs to install and build with no extra setup.

Modified by [Dustin Loring](https://github.com/Dustinwloring1988) (Dustinwloring1988) in October 2026.

## Stack

| Package | Version |
| --- | --- |
| Vite | ^8.3.4 |
| Tailwind CSS | ^4.3.3 |
| TypeScript | ^6.0.3 |
| Solid JS | ^1.9.17 |

Node 20 or newer is required.

## Commands

```bash
npm install   # install dependencies
npm run dev   # vite — dev server
npm run build # vite build — production build
npm run serve # vite preview — local preview server
```

## About this template

A Vite + Solid starter with Tailwind CSS 4 configured. `vite-plugin-solid` provides the Solid integration
with Vite. `tailwind.config.ts` uses the new CSS-first `@theme` syntax. The `App` component is the root
Solid component rendered via Vite.

## Upgraded to Vite 8, Tailwind CSS 4, Solid 1.9.17 (October 2026)

Moved from Vite 5, Tailwind CSS 3, and Solid 1.8.x. Each step was verified with `npm install` and
`npm run build`:
- Vite: 5 → 6 → 7 → 8
- Tailwind CSS: 3.4.x → 4.3.3 (Vite 8 peer requires ^4.3.3)
- Solid: 1.8.x → 1.9.17 (latest stable 1.x)
- TypeScript: ~5.5.0 → ^6.0.3 (Vite 8 + TW 4 peer range)

Tailwind CSS 4's `@theme` syntax replaced the old `tailwind.config.js` with CSS imports, which required
updating `index.css` and `vite.config.ts`. The `typescript` was also updated to ^6.0.3 because Vite 8 +
Tailwind CSS 4's peer range is `>=6.0 <7.0`.

## Verification

- `npm install` and `npm run build` pass
- Confirmed the dev server starts and HMR works with Tailwind classes
- `npm run build` produces a production build with Tailwind styles extracted