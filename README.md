# CREMA — The Art of Coffee

A responsive, English-language specialty coffee storefront built with Vite, React, TypeScript, Three.js, React Three Fiber and Drei. It is a static client-side demo: product data and cart are local, and no API, backend, or payment processing is used. The supplied Clifford GLB is used in the interactive hero, with a local image fallback if 3D loading fails.

## Requirements
- Node.js 18 or later
- npm

## Install and run
```sh
npm install
npm run dev
```

## Production build
```sh
npm run build
```
Vite writes the static site to `dist/`. Preview locally with `npm run preview`.

## Deploy to Cloudflare Pages
1. Push this project to a Git repository and create a Cloudflare Pages project connected to it (or build locally and upload `dist/`).
2. Framework preset: **Vite**. Build command: `npm run build`. Build output directory: `dist`.
3. Use Node.js 18+ for the build environment. No environment variables or server functions are required.

All model and image files are local under `public/assets` and are copied into `dist/assets` by Vite. The cart, deterministic coffee finder, filters, detail/journal dialogs, newsletter confirmation, and navigation run in the browser. Newsletter and checkout are explicitly demo interactions; no information is sent or payment collected.
