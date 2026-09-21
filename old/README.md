# old/ — assets from the original WebHealer site

Fetched 2026-09-21 from https://meerashahcounselling.com/ with curl.

| Path | What |
|---|---|
| `index.html` | Raw homepage source (all CSS is inline in `<head>`) |
| `pages/*.html` | Raw source of every page in the sitemap |
| `images/` | Every image the site references, renamed (original UUID names in the HTML) |
| `content.md` | All copy, per page, verbatim, with slugs/titles/meta |
| `design-tokens.css` | Colour / type / spacing tokens as CSS custom properties |

## Image map

| New name | Original | Size | Reuse? |
|---|---|---|---|
| `meera-portrait-300x451.jpg` | 9B1DC68D-…jpg | 300×451 | Yes — but only ~150px wide at 2×. Ask for a hi-res headshot. |
| `bacp-psa-badges-255x100.jpg` | 69530025-…jpg | 255×100 | Yes (low-res; PSA/BACP supply SVG/PNG badges on request) |
| `header-stepping-stones-772x276.jpg` | 09DA9CF4-…jpg | 772×276 | Reference only — photo + gradient + wave baked into one fixed-width raster |
| `footer-wave-772x202.jpg` | 2061B250-…jpg | 772×202 | Reference only — rebuild wave as CSS/SVG |
| `page-background-blur-1200x800.jpg` | 0D10167D-…jpg | 1200×800 | Reference only — fixed full-viewport blurred backdrop |
