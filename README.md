# Events Workflow

Single-file web app (index.html) that installs on an iPhone as a home-screen app and works offline.

- `index.html` the whole app
- `manifest.webmanifest`, `sw.js`, `icons/` make it installable and offline
- `vendor/` the PDF maker and font used to create quotes and invoices, bundled so it works offline
- Data lives on the device (browser storage). Backups go to a separate PRIVATE repository from inside the app (Menu > Backup & restore > GitHub backup).

Never commit business data to this repository.

## Host it (pick one)
- GitHub Pages: Settings > Pages > Deploy from branch `main`, folder `/ (root)`. (Free accounts need a public repo for Pages. That is fine because this repo holds code only.)
- Or Cloudflare Pages / Netlify: connect this repo, no build command, publish directory `/`.

## Install on iPhone
1. Open the site address in Safari (not Chrome).
2. Share button > Add to Home Screen > Add.
3. Open it from the new icon. Restore your data once: Menu > Backup & restore.
