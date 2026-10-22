# VIOLAB · ویلب

Coming-soon page for **violab.ir**. We Play The Taste.

Static site: `index.html` plus its images and fonts. It has no build step.

## Deploy (ParsPack VPS, nginx root `/var/www/violab`)

```
scp -r "D:\Claude Data\Cool Comp\violab" root@188.212.97.60:/var/www/
```

ArvanCloud sits in front (CDN + HTTPS). Purge its cache after an update.

## Routing coordinates

`LOCATION` in `index.html` holds the café's coordinates (35.7944806, 51.4735148). The Neshan, Balad, Google Maps and Waze buttons build their routing links from it.
