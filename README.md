# Ntunes-web

Landing page for **NTunes** — an ad-free, cross-platform music player built with Flutter (YouTube Music streaming, synced lyrics, offline downloads, playlist export).

## Downloads

Grab the latest build from the [Releases page](https://github.com/txngerine/Ntunes-web/releases/latest):

| Platform | Asset | Notes |
| --- | --- | --- |
| Android | `app-release.apk` | Sideload required (Android 7.0+) |
| macOS | `Ntunes.app.zip` | Unzip, drag to Applications. Unsigned: right-click → Open on first launch |

The site links to these via `releases/latest/download/<asset>`, so new releases need no site change as long as the asset names stay the same.

## Site

A single static page (`index.html`) with screenshots in `screenshots/` and assets in `assets/`. Deployed on Vercel (`vercel.json`).

To preview locally:

```sh
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

## Updating the download links

The URLs live near the top of the script in `index.html`:

- `ANDROID_APK_URL`
- `MACOS_ZIP_URL`
