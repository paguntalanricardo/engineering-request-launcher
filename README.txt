ENGINEERING REQUEST SYSTEM — PWA LAUNCHER (BETA 1.0)
=====================================================

WHAT THIS PACKAGE DOES
- Provides a branded installable launcher for Windows, iOS, and Android.
- The OPEN APPLICATION button opens your existing Google Apps Script web app.
- It does not copy, replace, or contain your Apps Script backend or database.
- It does not cache the Apps Script login page, user records, or request data.

YOUR APPLICATION URL
https://script.google.com/macros/s/AKfycbyLXw_m3TFQXUYpK99keKuNycMN2iBL-iXawreo4_fqGTfVsSh-mUBlCHBCAwoFSBfw/exec

IMPORTANT HOSTING REQUIREMENT
This package must be uploaded to an HTTPS static website host before it can be
installed as a PWA. Do not open index.html directly from a file:// location and
do not distribute the ZIP as though it were already an installed app.

Suggested hosting options:
- GitHub Pages (free static hosting)
- Netlify (free static hosting)

After hosting, test the HTTPS launcher URL on each device.

INSTALLATION
Windows PC (Chrome or Edge):
1. Open the hosted HTTPS launcher URL.
2. Use the browser's Install app option, if offered, or create a shortcut.
3. Launch the shortcut. Select OPEN APPLICATION.

Android:
1. Open the hosted HTTPS launcher URL in Chrome.
2. Choose Install app or Add to Home screen.
3. Launch the icon and tap OPEN APPLICATION.

iPhone / iPad:
1. Open the hosted HTTPS launcher URL in Safari.
2. Tap Share.
3. Choose Add to Home Screen.
4. If shown, enable Open as Web App, then tap Add.
5. Launch the icon and tap OPEN APPLICATION.

DEPLOYMENT / SECURITY NOTES
- Keep the Google Apps Script deployment access settings appropriate for your users.
- Users still need whatever Google account access your Apps Script deployment requires.
- The launcher requires internet access to reach the Apps Script application.
- This PWA is a launcher only; it does not make the Apps Script system work offline.
- The service worker caches only the static launcher shell, never the actual app or
  any private application data.
- Anyone who obtains the launcher can see the public web app URL. Access control
  must remain enforced by Apps Script, not by hiding the URL.
- If you later change the Apps Script deployment URL, update APP_URL in index.html,
  then upload the revised package contents to the hosting service.
