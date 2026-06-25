# App-Site

A simple, free website to host your app for direct download — no Google Play Store required.

## What's here
```
index.html        The landing page (app name, description, download button, install steps)
styles.css        Styling
render.yaml        Render deploy config (static site, forces .apk to download)
downloads/         Put your .apk file here (name it myapp.apk)
assets/            Put your app icon here (icon.png) — optional
```

## Customize it
1. Edit `index.html` — change "My App", the tagline, version, size, and features.
2. Add your app icon at `assets/icon.png` (square, ~512×512 looks great).
3. Add your installer at `downloads/myapp.apk` (see `downloads/README.md` for size limits).

## Run locally
Just open `index.html` in a browser, or serve the folder:
```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deploy on Render (free)
1. Push this repo to GitHub (already done if you're reading this there).
2. Go to https://dashboard.render.com → **New** → **Static Site**.
3. Connect this GitHub repo.
4. Settings: **Build Command** = empty, **Publish Directory** = `.`
   (Or just use the included `render.yaml` Blueprint and Render fills these in.)
5. Click **Create Static Site**. You'll get a live `https://...onrender.com` URL.
