# MwangiTrade Matrix — Official Website

A responsive React + TypeScript + Tailwind CSS website for the MwangiTrade Matrix Windows desktop trading terminal.

## Included
- Product landing page and feature overview
- Official GitHub Releases download centre
- Searchable trading glossary with category filters
- Trading guides, project information and risk disclosure
- Responsive dark trading-terminal visual system
- SEO title/description, Open Graph metadata, SoftwareApplication structured data, robots.txt and sitemap.xml
- Firebase Hosting configuration with SPA rewrites and static asset caching

## Stack
- React 18, TypeScript, Vite
- Tailwind CSS 3
- React Router
- Lucide icons
- Firebase Hosting

## Run locally

Requirements: Node.js 20 or later and npm.

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
npm run preview
```

The production build is written to `dist/`.

## Firebase Hosting deployment

1. Create or select the Firebase project in the Firebase Console.
2. Install the Firebase CLI: `npm install -g firebase-tools`.
3. Sign in: `firebase login`.
4. From this project folder, run `firebase use --add` and select your Firebase project. This creates the local `.firebaserc` file; do not commit a project selection until you intend to share it.
5. Run `npm run build`.
6. Run `firebase deploy --only hosting`.

The repository includes `firebase.json`; it serves the Vite production build from `dist/` and routes client-side paths to `index.html`.

## Configure the final public domain before launch

The Firebase project ID and public domain have not yet been supplied. Before launch, replace the temporary domain in:
- `index.html` — canonical URL (if using a canonical URL)
- `public/robots.txt` — sitemap URL
- `public/sitemap.xml` — all page URLs

Use your actual Firebase Hosting domain, usually `https://YOUR_PROJECT_ID.web.app`, or your verified custom domain.

## Downloads

The Download page points to the official release channel:
https://github.com/Anto-cmyk/MT-Matrix-Releases/releases/latest

Keep installer binaries and release metadata in that repository's GitHub Releases, not in this website source repository.

## Important

The site describes product capabilities at a high level. Actual functionality, supported Windows versions, MT5 connectivity and system requirements must match the current desktop release notes. Do not publish unverified performance claims, guaranteed-profit claims or financial advice.
