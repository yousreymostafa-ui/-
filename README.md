# 🌙 نور — تطبيق متابعة العبادات اليومية

A Progressive Web App (PWA) for daily Islamic worship tracking — works fully offline and can be installed on iOS/Android home screen.

## ✨ Features

- 📿 Full morning & evening adhkar with reader mode and counter
- 🕌 Sunnah prayers tracker
- 🤲 Persistent daily duas (add your own)
- 📖 Quran daily reading & Qiyam al-Layl
- 📅 Calendar view with color-coded history
- 📊 Analytics — charts, streaks, per-task stats
- 🌙 Dark mode
- ⚡ Fully offline — works without internet after first visit

---

## 🚀 Deploy to GitHub Pages (5 minutes)

### Step 1 — Create a new GitHub repository

1. Go to [github.com/new](https://github.com/new)
2. Name it anything (e.g. `noor` or `noor-app`)
3. Set it to **Public**
4. Do **not** add README/gitignore (keep it empty)
5. Click **Create repository**

### Step 2 — Upload the files

**Option A — GitHub Web UI (no terminal needed):**
1. On your new repo page, click **"uploading an existing file"**
2. Drag and drop ALL files from this folder:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icons/` folder (all PNG files inside)
   - `.github/workflows/deploy.yml`
3. Commit message: `Initial commit`
4. Click **Commit changes**

**Option B — Terminal (git):**
```bash
cd noor-pwa
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages

1. Go to your repo → **Settings** → **Pages**
2. Under **Source**, select **GitHub Actions**
3. Wait ~1 minute for the workflow to run
4. Your app will be live at:
   ```
   https://YOUR_USERNAME.github.io/YOUR_REPO/
   ```

---

## 📱 Install on iPhone

1. Open the URL in **Safari** (must be Safari, not Chrome)
2. Tap the **Share** button (□↑)
3. Scroll down → tap **"Add to Home Screen"**
4. Name it **نور** → tap **Add**
5. The app icon appears on your home screen 🎉

## 📱 Install on Android

1. Open the URL in **Chrome**
2. Tap the **⋮** menu → **"Add to Home screen"**
   — or tap the install banner that appears automatically

---

## 🔄 Updating the app

After any changes, just push to `main` branch — GitHub Actions deploys automatically within ~1 minute.

---

## 📁 File Structure

```
noor-pwa/
├── index.html          ← The entire app (single file)
├── manifest.json       ← PWA manifest (name, icons, display mode)
├── sw.js               ← Service worker (offline caching)
├── icons/              ← App icons for all platforms
│   ├── icon-192x192.png
│   ├── icon-512x512.png
│   ├── icon-192-maskable.png
│   ├── icon-512-maskable.png
│   └── ... (other sizes)
└── .github/
    └── workflows/
        └── deploy.yml  ← Auto-deploy to GitHub Pages
```

---

## 🛠 Local Development

Just open `index.html` directly in your browser — no build step needed.

For Service Worker to work locally, use a simple server:
```bash
# Python
python3 -m http.server 8080

# Node
npx serve .
```
Then open `http://localhost:8080`

---

*بارك الله فيك — اللهم تقبل منا*
