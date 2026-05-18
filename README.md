# uxi-linktree

Static linktree-style page. Deploys on Vercel with zero config.

## Local preview

Open `index.html` directly in a browser. No build step.

## Deploy

1. Push to GitHub: `yamb0x/uxi-linktree`
2. On Vercel: **Add New → Project → Import** the repo. Leave all settings at defaults.
3. After first deploy, claim the subdomain `uxi-linktree.vercel.app` in **Settings → Domains** (if not auto-assigned).

## QR code

`qr-code.png` encodes `https://uxi-linktree.vercel.app`. If you change the production URL, regenerate it (any QR generator works, or visit `https://api.qrserver.com/v1/create-qr-code/?size=600x600&data=YOUR_URL`).

## Adding links

Edit the `<ul class="links">` block in `index.html`:

```html
<li><a href="https://example.com" target="_blank" rel="noopener">Label</a></li>
```
