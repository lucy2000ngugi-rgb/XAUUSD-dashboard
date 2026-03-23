# XAUUSD Signal Hub (Phone-Ready PWA)

This package gives you a mobile-friendly XAUUSD signal dashboard that can be hosted and opened on your phone like an app.

## What it does
- 1H bias + 15M structure + 5M execution
- multiple signal cards
- Entry, SL, TP1, TP2, confidence
- auto refresh
- browser alerts on changed signals
- optional Telegram alerts
- installable as a PWA after hosting

## Fastest way to use it on your phone
### Option A: Netlify Drop
1. Unzip the package.
2. Go to Netlify Drop in your phone or laptop browser.
3. Drag or upload the whole folder.
4. Open the generated URL on your phone.
5. Add to Home Screen.

### Option B: GitHub Pages
1. Create a new public repo.
2. Upload the files from this folder.
3. In repo settings, turn on GitHub Pages from the main branch.
4. Open the site URL on your phone.

## Setup
1. Open the hosted site.
2. Paste your Twelve Data API key.
3. Choose your mode and auto-refresh.
4. Tap Enable Alerts.
5. Optional: paste your Telegram bot token and chat ID.

## Important security note
Telegram in this build is client-side. That means your bot token is stored locally on your device and used by the browser. Use a personal bot token only. The safer upgrade is a tiny backend relay.

## Safer next upgrade
If you want, the next step is a small backend (Cloudflare Worker / Netlify Function / Vercel Function) so:
- your Telegram token is not stored in the browser
- the dashboard can run alert checks server-side
- you can get alerts without keeping the page open

## Limitations
- It still approximates ICT/SMC concepts algorithmically.
- Browser notifications work best on hosted HTTPS pages.
- For always-on alerts, a serverless backend is better than a pure client app.
