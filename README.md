# uxi-linktree

Static linktree-style page. Deploys on Vercel with zero config.

## Local preview

Open `index.html` directly in a browser. No build step.

## Deploy

1. Push to GitHub: `yamb0x/uxi-linktree`
2. On Vercel: **Add New → Project → Import** the repo. Leave all settings at defaults.
3. After first deploy, claim the subdomain `uxi-linktree.vercel.app` in **Settings → Domains** (if not auto-assigned).

## QR code

Both files encode `https://uxi-linktree.vercel.app` with high error correction (~30% damage tolerance):

- **`qr-code.svg`** — vector, scales to any size with no pixelation. Use for print (posters, business cards, signage).
- **`qr-code.png`** — 1000×1000, use for screens, slides, or anywhere PNG is required.

If the production URL changes, regenerate both via `https://api.qrserver.com/v1/create-qr-code/?data=YOUR_URL&ecc=H&margin=20` (add `&format=svg` for the vector version, `&size=1000x1000` for the PNG).

## Adding links

Edit the `<ul class="links">` block in `index.html`:

```html
<li><a href="https://example.com" target="_blank" rel="noopener">Label</a></li>
```
