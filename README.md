# Red Sunset KP — Marketing Website

Single-page bilingual (EN/TH) marketing site for Red Sunset KP Co., Ltd.

- **Live**: https://redsunsetkp.com
- **GH Pages**: https://liam-kp.github.io/red-sunset-kp

## Stack

Static HTML + Tailwind CDN + vanilla JS. No build step.

## Local preview

```sh
python3 -m http.server 8000
# open http://localhost:8000
```

## Editing copy

- `i18n.js` — all user-facing strings (EN master + TH draft).
- `index.html` — structure / inline SVGs / styles.
- TH copy is marked `THAI DRAFT — pending Sirin Nekhamatcha review`. Do not unlock the TH toggle for production traffic until Sirin has reviewed.

## Updating leadership photos

Drop JPGs at:

- `assets/images/leadership/sirin-portrait.jpg`
- `assets/images/leadership/liran-portrait.jpg`

`onerror` fallback renders monogram circles (`SN` / `LM`) if either file is missing.

## Manual follow-ups (post-deploy)

1. Replace the `[to be inserted]` Company Registration No. in section 7 + footer with `0845567032172` (DBD-confirmed).
2. Sirin review of `i18n.js` Thai strings before TH toggle is unlocked publicly.
3. Domain WHOIS — move to Red Sunset KP Co., Ltd. or enable WHOIS Privacy.

## Deploy

Pushes to `main` deploy automatically via GitHub Pages.
