# TruckLoyal — Marketing Site

The public landing page for **TruckLoyal**, a loyalty rewards program for food trucks.
It explains the product, shows pricing, and links customers/vendors to the app at
`https://truckloyal-api.onrender.com/app`.

## What's here
```
index.html     The full landing page (self-contained — all CSS is inline)
render.yaml     Render deploy config (free static site)
```

## Run locally
Open `index.html` in a browser, or serve the folder:
```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deploy on Render (free)
1. Merge this to `main`.
2. Go to https://dashboard.render.com → **New** → **Static Site**.
3. Connect this GitHub repo (`Samuel0205/App-Site`).
4. **Build Command** = empty, **Publish Directory** = `.`
   (Or just use the included `render.yaml` Blueprint — Render fills these in.)
5. **Create Static Site** → you get a live `https://...onrender.com` URL.
   Every push to `main` auto-redeploys.
