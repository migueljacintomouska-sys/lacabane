# La Cabane — website prototype

Static site: `index.html` + `menu.pdf`. No build step, no dependencies.

## Publish on GitHub Pages
1. Create a new repository on GitHub (e.g. `la-cabane-site`).
2. Upload `index.html`, `menu.pdf` and this `README.md` to the root of the repository.
3. Repository → Settings → Pages → Source: "Deploy from a branch", Branch: `main`, folder `/ (root)` → Save.
4. After a minute the site is live at `https://<your-username>.github.io/la-cabane-site/`.

## What works out of the box
- "Reserve" / "Call to reserve" / the phone button open the dialer with +351 289 313 819.
- "Open the full menu (PDF)" opens `menu.pdf` in a new tab (keep it next to `index.html`).
- EN / PT / FR switcher, review filters, dish slideshow — all plain HTML/CSS/JS.
- Fonts load from Google Fonts; everything else is embedded in the file.

## Updating
- New menu: replace `menu.pdf` (same name).
- Dish photos: in `index.html`, each `<article class="dish">` has a `<div class="ph">` — replace its contents with `<img src="photos/your-photo.jpg" alt="...">`.
