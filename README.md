# VIOLAB · ویلب

Coming-soon page for **violab.ir**. We Play The Taste.

Static site: `index.html` plus its images and fonts. It has no build step.

## Deploy (ParsPack VPS, nginx root `/var/www/violab`)

The server keeps `/var/www/violab` as a git clone and a cron job resets it to `origin/main` every 2 minutes, so merging a PR into `main` deploys it.

ArvanCloud sits in front (CDN + HTTPS). Purge its cache after an update.

## App icon (Add to Home Screen)

`manifest.json` names the app **VioLab** and points at the icons in `icons/` (192/512, plus maskable versions for Android). iOS uses `icons/apple-touch-icon.png` and the `apple-mobile-web-app-title` meta tag. All icons are generated from `logo.png` on the theme yellow `#FEF461`.

## Routing coordinates

`LOCATION` in `index.html` holds the café's coordinates (35.7944806, 51.4735148). The Neshan, Balad, Google Maps and Waze buttons build their routing links from it.
