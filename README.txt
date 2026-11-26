# EVE Time Converter — Hobart

A small installable Progressive Web App for Google Pixel / Android.

## Features
- Live EVE server clock (UTC) and Hobart clock
- EVE UTC date/time to Hobart conversion
- Automatic AEST/AEDT daylight-saving handling via `Australia/Hobart`
- 24-hour conversion table with previous/next-day labels
- Copy converted result
- Offline app shell after first successful load

## Install on your Pixel
A PWA must be served from HTTPS (or localhost) to be installable. It cannot be installed as a normal app by opening `index.html` from Downloads.

1. Put all four files (`index.html`, `manifest.webmanifest`, `sw.js`, `icon.svg`) in the same folder on an HTTPS static host.
2. Open that HTTPS address in Chrome on your Pixel.
3. Open Chrome's ⋮ menu and choose **Install app** or **Add to Home screen**.
4. Confirm. The EVE Time icon will appear on your home screen.

You can host the folder on GitHub Pages, Netlify, or another HTTPS static host. No account or server-side database is needed for the app itself.

## Notes
- EVE server time is UTC.
- The app uses the device's built-in IANA time-zone database for `Australia/Hobart`; daylight saving changes are automatic.
- Live clocks use the phone's current system clock. Ensure Android date/time is set automatically for best results.
- This is an unofficial fan-made utility and is not affiliated with CCP Games.
