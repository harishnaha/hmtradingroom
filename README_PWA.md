# HM Trading Journal — PWA V15

This package is based on the iPhone-ready V14 HM Trading Journal.

## Start on a computer

A PWA service worker needs a web origin. Do not rely on double-clicking `index.html` with `file://`.

If Python is installed:

```bash
cd HM_Trading_Journal_PWA_V15
python -m http.server 8000
```

Then open:

`http://localhost:8000/`

This is suitable for local testing.

## Put it online for iPhone

Upload the entire folder to an HTTPS static host. Keep this structure:

- index.html
- manifest.json
- service-worker.js
- icons/icon-192.png
- icons/icon-512.png
- icons/apple-touch-icon.png

Recommended simple hosts: GitHub Pages, Netlify, Cloudflare Pages, or Vercel.

## Install on iPhone

1. Open the HTTPS URL in Safari.
2. Tap Share.
3. Tap **Add to Home Screen**.
4. Keep the app name as **HM Journal** / **HM Trading Journal**.
5. Tap Add.
6. Open the new HM Journal icon from the Home Screen.

## Backup / Restore

Use the app's **System → Backup Full Journal (JSON)** before moving devices or making major changes.

On iPhone, save the JSON backup to Files or OneDrive. To restore, use **System → Restore Full Journal** and select the JSON backup.

## Important

The PWA shell caches the application so it can load offline. Your journal data continues to use the app's existing local storage/IndexedDB system. Keep regular JSON backups; the PWA cache is not a replacement for backups.
