# 🌴 Weekend Vibes — Task App

A beautiful weekend task manager, installable on iPhone without the App Store.

---

## 📱 How to Install on iPhone

### Option A — Open directly in Safari (easiest)
1. Transfer `index.html` to your iPhone (AirDrop, email it to yourself, or upload to iCloud Drive)
2. Open it in **Safari** (must be Safari, not Chrome)
3. Tap the **Share** button (box with arrow at bottom of screen)
4. Scroll down and tap **"Add to Home Screen"**
5. Tap **Add** — the app icon appears on your home screen!

### Option B — Host locally on your Mac (best experience)
If you have a Mac on the same Wi-Fi as your iPhone:

1. Open Terminal on your Mac
2. Navigate to this folder:
   ```
   cd path/to/weekend-vibes-app
   ```
3. Start a local server:
   ```
   python3 -m http.server 8080
   ```
4. Find your Mac's local IP address (System Settings → Wi-Fi → Details)
5. On your iPhone Safari, go to: `http://YOUR-MAC-IP:8080`
6. Tap Share → **Add to Home Screen**

### Option C — Free hosting (permanent URL)
Upload the entire folder to any free static host:
- **Netlify Drop**: drag the folder to [netlify.com/drop](https://netlify.com/drop)
- **GitHub Pages**: push to a repo and enable Pages
- **Vercel**: `npx vercel` in this folder

---

## 📁 Files in this Package

| File | Purpose |
|------|---------|
| `index.html` | The full app |
| `manifest.json` | PWA metadata (name, icons, display mode) |
| `sw.js` | Service worker — enables offline use |
| `icon-192.png` | App icon (home screen) |
| `icon-512.png` | App icon (splash screen) |

---

## ✨ Features

- ✅ Add weekend tasks with due dates & priority
- 🔁 Recurring tasks (weekly, fortnightly, monthly, every weekend)
- ⚡ Due date reminders & overdue alerts
- 🎯 Filter by All / To Do / Completed / Due
- 📤 Export as Plain Text, CSV, or Markdown
- 💾 All data saved locally on your device
- 📴 Works fully offline once installed

---

## 🔧 Troubleshooting

**"Add to Home Screen" not showing?**
Make sure you're using Safari — Chrome and Firefox on iOS cannot install PWAs.

**App not loading offline?**
The service worker needs one online visit first to cache the app. Open it once on Wi-Fi, then it works offline.

**Data lost after update?**
Tasks are stored in your browser's localStorage. Clearing Safari's website data will erase them. Use the Export feature to back up regularly.
