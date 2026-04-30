# NursePartners Card Scanner — PWA Setup Guide

## What's in this folder

| File | Purpose |
|------|---------|
| `index.html` | The full app (all-in-one) |
| `manifest.json` | Makes it installable on phones |
| `sw.js` | Service worker — enables offline use |
| `icon-192.png` | App icon (Android home screen) |
| `icon-512.png` | App icon (splash screen) |

---

## Step 1 — Host the files (free, takes 5 minutes)

### Option A: Netlify Drop (Easiest — no account needed)

1. Go to **https://app.netlify.com/drop**
2. Drag the entire `np-pwa` folder onto the page
3. Netlify gives you a live URL like `https://random-name-123.netlify.app`
4. Share that URL with your team

### Option B: Netlify with a custom URL

1. Create a free account at **https://netlify.com**
2. Go to Sites → "Add new site" → "Deploy manually"
3. Drag the folder to upload
4. In Site Settings → Domain Management, set a custom name like `nursepartners-scanner.netlify.app`

### Option C: GitHub Pages (slightly more technical)

1. Create a free GitHub account at **https://github.com**
2. Create a new repository (public)
3. Upload all 5 files to the repository
4. Go to Settings → Pages → Source: Deploy from branch → `main` / `root`
5. Your app is live at `https://yourusername.github.io/your-repo-name`

---

## Step 2 — Install on iPhone

1. Open **Safari** on the iPhone (must be Safari, not Chrome)
2. Go to the app URL
3. Tap the **Share** button (box with arrow pointing up) at the bottom
4. Scroll down and tap **"Add to Home Screen"**
5. Tap **"Add"** in the top right
6. The NursePartners icon appears on the home screen — tap it to open like any app

> ⚠️ **iPhone tip:** The install prompt only appears in Safari. If the user opens the link in Chrome or another browser, they need to switch to Safari first.

---

## Step 3 — Install on Android (Samsung, Google Pixel, etc.)

1. Open **Chrome** on the Android phone
2. Go to the app URL
3. A banner will appear at the bottom saying **"Add NP Scanner to Home screen"** — tap it
4. Or tap the **3-dot menu** (top right) → **"Add to Home screen"** or **"Install app"**
5. Tap **"Install"**
6. The app icon appears on the home screen

> ✅ Android users may also see an automatic install popup appear after visiting the app for a few seconds.

---

## How to share the app with users

Just send them the link via:
- **Text message**
- **Email**
- **WhatsApp**

Example message to send:
> "Here's the NursePartners Card Scanner app: [YOUR URL HERE]
> Open the link in your phone browser, then follow the prompts to install it on your home screen. Works on iPhone and Android!"

---

## Features

- 📷 **Business card camera** — point at a card, AI extracts all contact fields
- 🎙️ **Voice notes** — record a memo per contact, saved with the entry
- 📝 **Manual form** — fill in or edit any field
- 👥 **Contact list** — tap any contact to see full details with tappable links
- 📤 **Export** — download CSV or email to peterabraldes@nursepartners.net
- ⏱️ **4-hour session** — auto-sends the report when time expires
- 📴 **Works offline** — once installed, the app works without internet (AI extraction requires connection)

---

## Troubleshooting

| Issue | Fix |
|-------|-----|
| App won't install on iPhone | Must use Safari, not Chrome |
| Camera won't open | Allow camera permission when prompted |
| Mic won't record | Allow microphone permission when prompted |
| AI extraction fails | Check internet connection; fill fields manually |
| Install banner doesn't appear on Android | Tap Chrome menu → "Add to Home Screen" manually |
