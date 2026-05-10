# Woodshed

Marketing and support site for the Woodshed iOS app — a tune recorder for old time and bluegrass musicians.

Hosted on GitHub Pages at **https://sararussert.github.io/woodshedIOS/**

## Pages

| File | Purpose |
|------|---------|
| `index.html` | Marketing / landing page |
| `support.html` | Support and FAQ |
| `privacy.html` | Privacy policy |

## Before launch

Search for `TODO` across the HTML files — there are a few things to fill in:

1. **App Store ID** — replace `idPLACEHOLDER` with your real App Store ID in `index.html`
2. **Support email** — replace `woodshed@youremail.com` with your real address in `support.html` and `privacy.html`
3. **Smart App Banner** — uncomment the `apple-itunes-app` meta tag in `index.html` once the app is live
4. **Install banner** — remove the early `return` in the banner script in `index.html` once the App Store link is ready

## Custom domain (when ready)

Add a `CNAME` file in the root of this repo containing your domain, e.g.:

```
woodshed.yourdomain.com
```

Then configure your DNS to point that subdomain to `sararussert.github.io`.

## Assets

| Path | Contents |
|------|----------|
| `assets/site.css` | All styles |
| `assets/app-icon.png` | Full-size app icon (1254×1254) |
| `assets/app-icon-256.png` | Icon for Apple touch icon |
| `assets/favicon-128.png` | Browser favicon |
| `assets/screenshots/` | App screenshots |
