# switchbase-web

The public-facing web presence for [Switchbase](https://github.com/iDrewn/switch-collection), a personal collection tracker for press-on nails. Hosted via GitHub Pages at **[idrewn.github.io/switchbase-web](https://idrewn.github.io/switchbase-web/)**.

This repo is intentionally separate from the app's source (which lives in a private repo) — it only needs to be public so GitHub Pages and app store review can reach it without a paid plan or repo access.

## What's here

| File | Purpose |
|---|---|
| `index.html` | Landing page — download links for the Android `.apk` and the iOS TestFlight beta |
| `privacy-policy.html` | The app's privacy policy (linked from Play Console / App Store Connect) |

## How the Android download stays current

The `.apk` isn't committed to this repo — it's attached as an asset on the [`latest` release](https://github.com/iDrewn/switchbase-web/releases/tag/latest). A GitHub Actions workflow in the app's repo rebuilds and re-uploads it there on every push to `master`, so the download link on the landing page never changes even as the app updates.
