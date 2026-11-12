# Memory One UI — Android APK

This repository wraps the existing web app in a native Android shell using Capacitor.

## Project layout

- `www/index.html` — original web app (copy the supplied `memory_one_ui_9_5_galaxy_ai.html` here and rename it to `index.html`).
- `capacitor.config.json` — Capacitor configuration.
- `.github/workflows/android-apk.yml` — builds a debug APK on GitHub Actions.

## Build

The workflow runs on **Actions → Build Android APK → Run workflow** (or on pushes to `main`). It installs dependencies, adds/synchronizes Android, builds a debug APK, and uploads it as an artifact named `memory-one-ui-debug-apk`.

Download the artifact from the completed workflow run. This is a debug APK for testing, not a Play Store release-signed APK.

The app may require internet access for remote assets referenced by the original HTML.
