# arcticalm_webb

Static one-page landing site for the Arcticalm mobile app. Built with [Astro](https://astro.build/) for maximum SEO and Core Web Vitals.

## Develop

```bash
npm install
npm run dev      # http://localhost:4321
```

## Build

```bash
npm run build    # outputs to ./dist
npm run preview  # serve the built site locally
```

## Deploy

Pushes to `main` build and deploy to GitHub Pages via `.github/workflows/deploy.yml`.


## TODOs before launch

- Replace `#` hrefs in `src/components/StoreBadges.astro` with the real App Store and Google Play URLs.
- Replace placeholder `/privacy` and `/support` links in `src/components/Footer.astro` (or host these as separate pages).
- Replace `public/og-image.png` with a designed 1200×630 social-preview image (currently a copy of the app icon).
- Tweak hero copy in `src/components/Hero.astro` and `<title>`/`<meta description>` in `src/layouts/BaseLayout.astro`.

## SEO checklist baked in

- Pre-rendered static HTML (zero JS by default)
- `<title>`, meta description, canonical URL
- Open Graph + Twitter Card meta tags
- `MobileApplication` JSON-LD structured data (eligible for Google rich results)
- `sitemap-index.xml` via `@astrojs/sitemap`
- `robots.txt`
- `theme-color` and `apple-touch-icon`
- Reduced-motion CSS guard
