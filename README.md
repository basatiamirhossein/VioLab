# VIOLAB · ویلب

Coming-soon page for **violab.ir**. We Play The Taste.

Static site: `index.html` plus its images and fonts. It has no build step.

## Deploy (ParsPack VPS, nginx root `/var/www/violab`)

```
scp -r "D:\Claude Data\Cool Comp\violab" root@188.212.97.60:/var/www/
```

ArvanCloud sits in front (CDN + HTTPS). Purge its cache after an update.

## Routing coordinates

Set `LOCATION` in `index.html` to the café's lat/lng. Until then, every routing button opens the Google Maps link.
