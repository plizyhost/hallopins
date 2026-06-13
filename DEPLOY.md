# Pinterest Pin Studio v2 — Update on Vercel

This is the Create React App version, matching your existing repo structure
(public/index.html, src/App.jsx, src/index.js, package.json).

## How to update your live site

1. Go to your GitHub repo (plizyhost/pinmaker)
2. Replace these files with the new ones from this folder:
   - src/App.jsx        ← the big update (all new features)
   - package.json       ← now includes "jszip" dependency (needed for ZIP download)
   - public/index.html  ← loads all Google Fonts
   - src/index.js       ← unchanged, but included for completeness
3. Commit the changes
4. Vercel auto-redeploys in ~2 minutes

## IMPORTANT — package.json changed
The new "Download all (ZIP)" feature needs the `jszip` package.
Make sure you upload the new package.json (it adds jszip to dependencies),
or Vercel's build will fail with "Module not found: jszip".

## Application Preset on Vercel
Keep it set to: Create React App  (same as before)

## What's new in v2
- Download all pins as a ZIP (CSV + Sitemap tabs)
- Full color picker with 50+ colors + custom hex / color wheel
- 8 ready-made templates + save your own custom templates
- Image position controls: drag horizontal / vertical + zoom
- Per-pin custom styling (click a pin to override its colors/layout)
- Sitemap scraper with 4 proxy fallbacks + sitemap-index support
- Banner background and vertical centering fixed

## Build verified
This exact code was compiled with `npm run build` → "Compiled successfully."
