# BookieApp — PWA Setup Guide

A private betting app for you and your friends. You're the bookie — set events, set odds, settle results. Friends install it on their phone and place bets.

---

## Files

| File | Purpose |
|------|---------|
| `index.html` | The full app |
| `manifest.json` | Makes it installable as a PWA |
| `sw.js` | Service worker (offline support) |
| `icon-192.png` | App icon — add your own 192×192px PNG |
| `icon-512.png` | App icon — add your own 512×512px PNG |

---

## How to host it (free, 5 minutes)

### Option A — GitHub Pages (easiest)
1. Go to github.com and create a new **public** repository called `bookieapp`
2. Upload all files (`index.html`, `manifest.json`, `sw.js`, plus your icons)
3. Go to **Settings → Pages → Source: main / root**
4. Your app URL will be: `https://YOUR-USERNAME.github.io/bookieapp/`
5. Share that link with your friends

### Option B — Netlify (drag and drop)
1. Go to netlify.com and sign up (free)
2. Drag your whole project folder onto the Netlify dashboard
3. Netlify gives you a URL like `https://your-app.netlify.app`
4. Share that link

---

## How friends install it

### iPhone / Safari
1. Open the link in Safari
2. Tap the Share button (box with arrow)
3. Tap "Add to Home Screen"
4. Tap "Add" — it appears like a real app

### Android / Chrome
1. Open the link in Chrome
2. Tap the three-dot menu
3. Tap "Add to Home screen" or "Install app"
4. Done

---

## How it works

### You (the bookie)
- Tap the **Bookie** tab — enter your PIN (default: `1234`, change it in settings)
- **Create events** with any number of outcomes and decimal odds
- Events can be sports games, custom events, anything
- When the result is in, tap **Settle event**, pick the winning outcome
- All winning bets are automatically marked Won, losers marked Lost

### Your friends (bettors)
- Open the link, enter their name once
- See all open events on the **Events** tab
- Tap **Place bet**, pick outcome, enter stake
- Track their bets on **My bets**
- See who's up and who's down on **Standings**

---

## Add your own icons

Create two PNG images:
- `icon-192.png` — 192×192 pixels
- `icon-512.png` — 512×512 pixels

Use a dice, money bag, or any image you like. Free tools: Canva, GIMP, or any image editor.

Until you add icons, the app still works — it just won't have a custom icon when installed.

---

## Tips

- All data is stored locally in each person's browser — no server, no database
- The bookie PIN keeps the manage/settle screen private from friends
- Default PIN is `1234` — change it in Bookie → Settings before sharing
- Decimal odds: `2.0` = evens, `3.0` = 2/1, `1.5` = 1/2
- Money is tracked virtually — you settle up in real life

---

## Legal note

This app is for private, social use between friends. Check your local laws regarding informal betting before use.
