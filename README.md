# MACHAA OS
Offline, local-only productivity app (PWA). No account, no servers.
## Install on Android (PWA)
1. Host this folder over HTTPS (GitHub Pages, Netlify Drop, Cloudflare Pages).
2. Open the URL in Chrome on your phone, wait a few seconds, then menu > "Install app" / "Add to Home screen".
3. It now opens full screen and works offline. Data lives in the phone's browser storage; use More > Export backup regularly.
## Build a real APK (needs internet + your own PC)
Option A (easiest): go to pwabuilder.com, enter your hosted URL, choose Android, download the APK/AAB.
Option B (Capacitor): `npm init -y && npm i @capacitor/core @capacitor/cli @capacitor/android`, `npx cap init "MACHAA OS" com.machaa.os --web-dir=.`, `npx cap add android`, `npx cap sync`, `npx cap open android`, then Build > Build APK in Android Studio.
