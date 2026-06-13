═══════════════════════════════════════════════════════
  PINTEREST PIN STUDIO — UPDATE (v2.1)
═══════════════════════════════════════════════════════
Built & verified: npm run build → Compiled successfully (0 errors)

WHAT'S FIXED IN THIS UPDATE
1. TEMPLATES no longer change every pin.
   - In CSV/Sitemap, click a pin card to select it, then in the
     orange panel click "Lock current template into this pin only".
   - Pick a Ready Template first, then lock it onto that one pin.
     Other pins are untouched.
2. BANNER TRANSPARENCY.
   - New "Banner opacity" slider (sidebar > Banner Size).
   - Lower it so the photos show through the banner — no blank gap.
   - Text automatically gets a shadow so it stays readable.
3. SITEMAP SCRAPER — more reliable.
   - Now tries 5 proxies including the allorigins JSON endpoint.
   - Already pulls title + OG image + URL from each page.
4. PINTEREST SCHEDULING CSV.
   - New blue "Pinterest CSV" button next to "Download all (ZIP)".
   - The ZIP also now contains pinterest-schedule.csv automatically.
   - Columns: Title, Media URL (matches image filenames), Board,
     Description, Link, Publish date, Keywords.
5. TEXT NEVER OVERFLOWS THE BANNER.
   - Headline auto-shrinks to fit inside the banner height.

───────────────────────────────────────────────────────
DEPLOY (your repo: plizyhost/hallopins, command line)
───────────────────────────────────────────────────────
cd /Users/mac/Downloads/hallopins
# copy these over the old files (keep folder layout):
#   package.json, public/index.html, src/App.jsx, src/index.js
git add .
git commit -m "v2.1: transparency, per-pin lock, pinterest csv, autofit"
git push

Then Vercel auto-redeploys. HARD REFRESH the page: Cmd + Shift + R
═══════════════════════════════════════════════════════
