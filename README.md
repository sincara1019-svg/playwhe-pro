# PlayWhe Pro - APK Build Package

This folder is a ready-to-build Capacitor Android project.

## What's inside:
- `www/index.html` = Your mobile app (built from PlayWhe-Pulse-FIXED-2_2.html)
- `capacitor.config.json` = App ID com.playwhe.pro
- `package.json` = dependencies

## How to build APK (3 commands):

### Option 1: On your computer (requires Node + Android Studio)
```bash
npm install
npx cap add android
npx cap sync
npx cap open android
```
Then in Android Studio: Build > Build Bundle(s) / APK(s) > Build APK(s)

APK will be at: android/app/build/outputs/apk/debug/app-debug.apk

### Option 2: Online (no setup) - Use PWABuilder
1. Host the www folder (e.g. upload to Netlify Drop - drag www folder)
2. Go to https://www.pwabuilder.com
3. Paste your hosted URL
4. Click Build My PWA > Android > Generate APK

### Option 3: I build it for you via GitHub Actions
1. Create GitHub repo, push this folder
2. GitHub will auto-build APK (workflow included)

## App details:
- Package: com.playwhe.pro
- Name: PlayWhe Pro
- Theme: #38bdf8
- Version: 1.0.0 (740 draws)
- Permissions: none needed, offline works

## Icons needed:
Add 512x512 icon as www/icon-512.png and www/icon-192.png
Already included in HTML via Tailwind.

## PWA install (instant, no APK):
Just open www/index.html on phone > Add to Home Screen - works like native app immediately.
