# SBA Uber Driver P&L Report — iPhone PWA

A mobile-first Progressive Web App (PWA) for generating Uber driver income and expense reports. Built for SBA Small Business Accounting (NZ).

Supports both **IRD Mileage Rate** and **Actual Costs** methods. Works fully offline once installed.

---

## 📱 Deploy to iPhone in 4 Steps

### Step 1 — Create a GitHub Repository

1. Log in to [github.com](https://github.com)
2. Click **"New repository"**
3. Name it: `uber-pl-report` (or any name you like)
4. Set to **Public**
5. Click **"Create repository"**

---

### Step 2 — Upload the Files

Upload ALL these files to the repository root:

```
index.html
manifest.json
sw.js
icon.svg
icon-192.png
icon-512.png
README.md
```

You can drag-and-drop them in the GitHub web interface.

---

### Step 3 — Enable GitHub Pages

1. Go to your repository → **Settings** → **Pages** (left sidebar)
2. Under **"Source"** → select **"Deploy from a branch"**
3. Branch: **main** / Folder: **/ (root)**
4. Click **Save**
5. Wait ~1–2 minutes → GitHub shows your URL:
   ```
   https://YOUR-USERNAME.github.io/uber-pl-report/
   ```

---

### Step 4 — Add to iPhone Home Screen

1. Open **Safari** on your iPhone
2. Go to your GitHub Pages URL
3. Tap the **Share** button (box with arrow pointing up)
4. Scroll down → tap **"Add to Home Screen"**
5. Name it **"Uber P&L"** → tap **Add**

✅ The app now appears on your iPhone home screen and opens like a native app — full screen, no browser chrome.

---

## Features

| Feature | Detail |
|---|---|
| **Methods** | IRD Mileage Rate (83¢/14,000 km, then 31¢) or Actual Costs with business use % |
| **Income** | Month-by-month entry (Apr–Mar NZ tax year) |
| **Expenses** | Vehicle running costs + phone, accounting, bank fees, etc. |
| **GST** | Toggle for GST-registered clients (income GST breakdown) |
| **Report** | Full P&L summary with DRAFT watermark on print |
| **Print/PDF** | Print to PDF via iPhone Share → Print |
| **Offline** | Works without internet after first visit |
| **Data** | Auto-saved to device (localStorage) |
| **Branches** | New Brighton or Rolleston |

---

## Tax Year Support

- FY2023 (year ended 31 March 2023)
- FY2024 (year ended 31 March 2024)
- FY2025 (year ended 31 March 2025)
- FY2026 (year ended 31 March 2026)

---

## Updating the App

When you update files in GitHub, users will get the latest version automatically next time they open the app while connected to internet.

To force a cache refresh, increment the cache version in `sw.js`:
```js
const CACHE_NAME = 'sba-uber-pl-v2'; // bump the version number
```

---

## Notes

- **No server required** — runs entirely in the browser
- **No login** — data stays on the device
- **Privacy** — no data is sent anywhere; all stored locally
- Designed for NZ tax year (April–March)

---

*SBA Small Business Accounting — New Brighton & Rolleston*
