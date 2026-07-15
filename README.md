# MoHRE Digital DNA — 13 AI Agents

A static, self-contained snapshot of the Ministry of Human Resources and Emiratisation
(MoHRE) "Digital DNA — 13 AI Agents" showcase page, prepared for hosting on GitHub Pages.

## What this is

A single-page site (`index.html`) with all styles, fonts and images served locally from
`assets/`. It was adapted from a saved copy of the original published page so that it works
when hosted on any static host, with no cross-origin (CORS) errors and no broken images.

## Changes made for reliable hosting

- Renamed the asset folder (`… _files/`) to a URL-safe `assets/` and updated every reference.
- Renamed the Google-Fonts stylesheet (`css2`, no extension) to `assets/fonts.css` so it is
  served with the correct `text/css` MIME type.
- Removed dead `modulepreload` links and the analytics / web-vitals scripts
  (`events.js`, `_flock.js`) that phoned home to the original origin — the source of the
  CORS console errors.
- Fixed a stale absolute self-link so in-page navigation stays on this site.
- Added `.nojekyll` so GitHub Pages serves all files as-is.

Fonts load from Google Fonts (CORS-safe) with local fallbacks via `font-display: swap`.

## Local preview

```bash
python3 -m http.server 8000
# then open http://127.0.0.1:8000/
```
