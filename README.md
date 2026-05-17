# ✦ ScholarWatch PWA — Deployment Guide

A mobile-first Progressive Web App for live academic paper discovery.
Works on iPhone, Android, and desktop. Installable to home screen.

---

## 📁 Files in this folder

```
scholarwatch-pwa/
├── index.html       ← The entire app (one file)
├── manifest.json    ← PWA metadata (name, icons, theme)
├── sw.js            ← Service worker (offline support)
├── icons/
│   ├── icon-192.png ← App icon (home screen)
│   └── icon-512.png ← App icon (splash screen)
└── README.md        ← This file
```

---

## 🚀 Deploy FREE to GitHub Pages (10 minutes)

### Step 1 — Create a GitHub account
Go to https://github.com and sign up (free).

### Step 2 — Create a new repository
1. Click the **+** button (top right) → **New repository**
2. Name it: `scholarwatch` (or anything you like)
3. Set to **Public**
4. Click **Create repository**

### Step 3 — Upload the files
1. On the new repo page, click **uploading an existing file**
2. Drag ALL files from this folder into the browser:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - The `icons/` folder (drag the whole folder)
3. Scroll down → click **Commit changes**

### Step 4 — Enable GitHub Pages
1. In your repo, click **Settings** (top menu)
2. Scroll to **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Branch: **main**, Folder: **/ (root)**
5. Click **Save**

### Step 5 — Get your URL
After ~2 minutes, your app is live at:
```
https://YOUR-USERNAME.github.io/scholarwatch/
```

**That's it!** Share this URL with anyone. Open it on your phone browser.

---

## 📱 Add to iPhone Home Screen

1. Open the URL in **Safari** (must be Safari on iPhone)
2. Tap the **Share** button (box with arrow ↑)
3. Scroll down → tap **Add to Home Screen**
4. Tap **Add**

ScholarWatch now appears on your home screen like a real app! ✦

---

## 📱 Add to Android Home Screen

1. Open the URL in **Chrome**
2. A banner may appear: **"Add ScholarWatch to home screen"** → tap it
3. Or: tap the **⋮ menu** → **Add to Home screen**

---

## 🔄 Updating the app

When you want to update:
1. Edit `index.html` on GitHub (click the file → pencil icon)
2. Commit the change
3. GitHub Pages auto-deploys in ~1 minute

---

## 🌐 Alternative: Deploy to Netlify (even easier)

1. Go to https://netlify.com → Sign up free
2. Drag the entire `scholarwatch-pwa` folder onto the Netlify dashboard
3. Done! You get a URL like `https://random-name.netlify.app`

To get a custom URL: Netlify Settings → Domain management → Add custom domain.

---

## 📡 How the data works

| Source | What | Free? |
|---|---|---|
| Semantic Scholar | Citations, abstracts, DOI links | ✅ No key needed |
| arXiv | Preprints, cutting-edge research | ✅ No key needed |

- **Daily**: papers from last 48 hours
- **Weekly**: papers from last 7 days
- **Monthly**: papers from last 31 days
- Auto-refreshes every **30 minutes**

---

## ❓ Troubleshooting

**"No papers found" on Daily**
→ Daily has fewer papers. Try Weekly or Monthly first.
→ Tap ↻ to force a refresh.

**App won't install on iPhone**
→ Must use Safari (not Chrome) on iPhone for PWA install.

**Data not loading**
→ Check internet connection. Both APIs are public and free.

---

Made with ✦ for curious minds everywhere.
