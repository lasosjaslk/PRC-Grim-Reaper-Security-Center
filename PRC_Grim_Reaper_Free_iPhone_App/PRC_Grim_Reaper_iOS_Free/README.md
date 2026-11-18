# PRC Grim Reaper Security Center — Free iPhone build

This is a free, installable, mobile-first web app (PWA). It can be hosted for free on GitHub Pages and added to an iPhone Home Screen from Safari. It does not require a paid domain, VPS, Apple Developer account, or Mac to use as a PWA.

## What's included
- PRC Grim Reaper dark/red mobile dashboard
- iPhone security guidance and links to Apple documentation
- Local-only chat preview with a basic client-side slur/link filter
- Community rules and future reporting explanation
- Hall of Fame preview
- Bitcoin donation section with no fabricated wallet address
- Offline app shell after first successful load

## Important limits — read before publishing
- Chat is local to one browser/device. It is NOT worldwide, live, or synced between people.
- The preview's simple filter is not AI moderation and cannot guarantee detection of hateful content. A real public community needs server-side moderation, human moderators, reporting queues, account controls, and abuse prevention.
- No VPN tunnel is implemented. The app explicitly reports that no VPN server is configured.
- This app does not scan all iPhone files, remove viruses, or replace iOS security protections.
- No Bitcoin address is configured. Do not send funds to an address unless the project owner verifies and publishes it.
- The included static app is a starting point, not a deployed service or App Store-signed native app.

## Free deployment with GitHub Pages (Windows)
1. Create or sign in to a GitHub account.
2. Create a **public** repository named `prc-grim-reaper`.
3. Extract this ZIP on Windows.
4. Upload the contents of the `PRC_Grim_Reaper_iOS_Free` folder to the repository root (so `index.html` is at the top level), then commit the files.
5. In the repository, open **Settings → Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
7. Wait for GitHub Pages to publish the site. The Pages URL will appear in Settings → Pages. This normally uses a free `github.io` address; no custom domain is needed.

## Install on iPhone
1. Open the published HTTPS GitHub Pages URL in **Safari** on the iPhone.
2. Tap **Share** (square with arrow).
3. Choose **Add to Home Screen**. If needed, scroll the share sheet to find it.
4. Name it `PRC Grim Reaper`, then tap **Add**.
5. Launch it from the new Home Screen icon. Open it online once first so the offline shell can cache.

If the site does not show the Add to Home Screen option, confirm you opened it in Safari and that the GitHub Pages site has finished publishing over HTTPS.

## Updating it
Edit the files in the GitHub repository and commit the changes. If an older cached version remains on the iPhone, close the app and reload the website in Safari; the service worker updates its cache on a later visit.

## Next stage when funding is available
A real multi-user chat and moderator system needs a backend and database. A real VPN needs a server and per-device WireGuard configuration. Native App Store distribution needs an Apple Developer account and a signed iOS build. Those are intentionally not represented as already working in this free build.
