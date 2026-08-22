# Oswin - Ply Udaan — Dynamic QR

A single QR code that redirects users to the correct app store based on their device.

- **Scan URL / QR target:** https://clubcurvedynamicqr.dpdns.org
- **iOS →** https://apps.apple.com/in/app/oswin-ply-udaan/id6780872581
- **Android →** https://play.google.com/store/apps/details?id=com.varient.oswin&pcampaignid=web_share

## How it works

1. The QR code encodes a single URL: `https://clubcurvedynamicqr.dpdns.org`
2. `index.html` detects the device from the user agent (iOS vs Android).
3. It redirects to the App Store on iPhone/iPad and Google Play on Android.

## Files

- `index.html` — the device-detecting redirect page (served at the root domain).
- `index2.html` — an in-browser QR code generator + download for the URL above.
- `CNAME` — custom domain for GitHub Pages.

Because the QR always encodes the same URL, any printed QR keeps working even if the
store links change — only `index.html` needs updating.
