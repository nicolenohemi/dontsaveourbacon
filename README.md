# Save Our Pigs 🐖

A one-page, mobile-first action site to **stop the Save Our Bacon Act** — built to get a visitor from "landing" to "talking to their senator" in as few taps as possible.

**Live:** https://saveourpigs.com

## How it works
- **Auto-locate** your state (browser GPS → U.S. Census geocoder), with a ZIP-code fallback.
- Shows your **two U.S. senators** — official photo, party, and DC office phone — from the public [`congress-legislators`](https://github.com/unitedstates/congress-legislators) dataset.
- One tap to **Call** (with a script), **Save** to your phone (vCard), or send a **pre-written email**.
- 4-step flow: contact → stay in the loop → learn more → share.
- Available in **English, Spanish, and Chinese**.

## Tech
Single static `index.html` — no build step, no backend. Vanilla JS. Deploy anywhere (Netlify, Vercel, GitHub Pages).

- Sign-ups (Step 2) post to **Netlify Forms** (form name `supporters`).
- Geolocation requires HTTPS — works on any real host, not `file://`.

## Develop
Open `index.html` in a browser, or serve the folder:
```bash
python3 -m http.server 8123
```

_Created by Joy Bardess._
