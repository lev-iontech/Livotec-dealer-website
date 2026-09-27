# Livotec Philippines: dealer site (Iontech)

Static site. No build step, no backend. Deploy the whole folder to GitHub Pages (keep `.nojekyll`) or Netlify.

## Where to edit
All in `index.html`, inside the first `<script>` block ("SITE DATA: edit here"):
- `PRODUCTS`: names, SRPs, specs, one-line descriptions, photo counts. Source: "Product Details" Google Sheet.
- `SERIES`: series taglines, descriptions, lifestyle images.
- `PERKS`: dealer perks list.
- `CONTACT`: lead email (info@iontech.com.ph). The form opens a pre-filled email to this address.

The savings calculator is the original `script.js` in the last `<script>` block. Only change: every model is marked `filtersConfirmed: true`, since filter prices are the same across the range. Its product prices live in its own `LOCAL_PRODUCTS` section. Keep them in sync with `PRODUCTS` when an SRP changes.

## Assets
- `assets/video/`: product film, 1080p (desktop) and 720p (mobile), H.264.
- `assets/img/products/`: product photos, `<id>-<n>.webp` (gallery) and `<id>-<n>-sm.webp` (cards).
- `assets/img/scenes/`: lifestyle, store formats, POSM, NSF certificate.
- `assets/img/brand/`: Livotec and Iontech logos, favicon.
