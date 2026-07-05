# Balloutt Trades LLC — Link Hub

A custom link-in-bio page for **@BallouttTradesLLC** — a nicer, faster,
fully-owned alternative to Linktree.

- Single static `index.html` — no build step, no dependencies, no tracking.
- On-brand aesthetic pulled from his own art: his purple-flame background photo,
  violet + ember palette, live ticker tape, glowing avatar, hover sparklines.
- Built-in **QR code** (`assets/qr.png`) linking back to this page — scan, save, share.
- Hosted free on **GitHub Pages**.

## Regenerate the QR code

If the live URL ever changes (e.g. a custom domain), regenerate `assets/qr.png`:

```bash
pip install qrcode pillow
python -c "import qrcode; qrcode.make('https://YOUR-URL/').save('assets/qr.png')"
```

## Edit your links

Open `index.html` and find the `<a class="link" ...>` blocks. Each one has a
`href` (where it goes), a title, and a subtitle. Add, remove, or reorder them —
that's it. Social icons live in the `<nav class="socials">` block near the bottom.

Swap `assets/profile.jpg` for a new logo (square works best).

## Deploy

Any push to `main` auto-publishes via GitHub Pages. Live URL is shown under
**Settings → Pages** in the repo.

---
Built for the community. Educational content only — not financial advice.
