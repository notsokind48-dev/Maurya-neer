# Maurya Jal Manager — installable web app

This bundle keeps the deep-blue / teal / mint theme from the preview and adds PWA metadata plus offline app-shell caching.

## What works
- Customer profiles
- 20-litre jar deliveries and empty-jar returns
- Dated payment and security-deposit records
- Outstanding water-charge calculation
- Daily, weekly and monthly subscription tracking
- Dashboard and JSON export/import backup
- Installable PWA on supported Android browsers
- App shell can open offline after the first successful online load

## Important data limitation
Customer records are saved in this browser's local storage. This bundle does **not** include cloud account sign-in or automatic online data synchronisation. JSON export/import is the backup method until a secure cloud backend is configured. Browser storage can be cleared, so export backups regularly.

## Publish online (HTTPS required for install/offline features)
1. Extract this ZIP.
2. Upload the contents of this folder to a static HTTPS host, for example a GitHub Pages site or another static host.
3. Open the resulting HTTPS website on Android in Chrome.
4. Use Chrome's menu → **Install app** or **Add to Home screen**.
5. Open it once online, then test offline launch.

## APK
This bundle is a Progressive Web App (PWA), not a compiled APK. To produce an APK, first publish it at an HTTPS URL, then use PWABuilder (https://www.pwabuilder.com/) with that URL to generate an Android package. Review the package and signing options before installing. This environment cannot publish a public website or sign/build a production APK on your behalf.

## First-run checklist
- Set the correct jar price and deposit in Settings.
- Test with sample customers.
- Export a backup and verify restore before entering all real records.
