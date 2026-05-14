# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

Marketing and support site for the Woodshed iOS app — a tune recorder for old time and bluegrass musicians. Hosted on GitHub Pages at https://sarabeth-russert.github.io/woodshedIOS/.

No build step, no framework, no dependencies. Edit files and push; GitHub Pages deploys automatically.

## Pages

| File | Purpose |
|------|---------|
| `index.html` | Marketing / landing page |
| `support.html` | Support and FAQ |
| `privacy.html` | Privacy policy |
| `assets/site.css` | All styles (single shared stylesheet) |

## Before launch checklist

Search for `TODO` in the HTML files — a few things still need filling in:

- **App Store ID** — replace `idPLACEHOLDER` with the real App Store ID in `index.html` (currently live as `id6768061433`)
- **Support email** — replace `woodshed@youremail.com` with the real address in `support.html` and `privacy.html`
- **Smart App Banner** — uncomment the `apple-itunes-app` meta tag in `index.html` once the app is live
- **Install banner** — remove the early `return` in the banner script in `index.html` once the App Store link is ready

## Design system

CSS custom properties are declared in `:root` at the top of `site.css`:

- `--paper` / `--parchment` — cream background tones
- `--ink` / `--ink-soft` / `--muted` — text hierarchy
- `--amber` / `--amber-deep` — primary brand color (CTAs, highlights)
- `--dark-panel` — near-black used for the marketing page body background

`body.inner-page` (support, privacy) uses `--paper` as background. The main marketing page (`index.html`) uses `--dark-panel`.

## index.html structure

Sections in order:
1. Mobile install banner (shown on non-Safari iOS via JS)
2. Nav
3. Hero — three-device mockup (iPhone, iPad, MacBook built in CSS)
4. Problem section — camera roll illustration
5. Metadata section — iPad screenshot
6. Practice section — Mac screenshot
7. Cross-device section — three-device grid
8. Audience section — 6-card grid
9. FAQ accordion
10. Footer

## Screenshot naming conventions

| File | Device | View |
|------|--------|------|
| `01_library.jpg`, `02_player.jpg` | iPhone | Library, Player |
| `02_record.png` | iPhone | Record |
| `03_add.png` | iPhone | Add |
| `iPadLibraryGrid.png`, `iPadLibraryFull.png` | iPad | Library variants |
| `iPadMetadata.png` | iPad | Metadata edit |
| `iPadLooping.png` | iPad | Loop practice |
| `macPlayback.png`, `macCrossDevice.png` | Mac | Playback variants |

## Custom domain

Add a `CNAME` file at the repo root containing the domain (e.g. `woodshed.yourdomain.com`), then configure DNS to point to `sarabeth-russert.github.io`.
