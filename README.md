# LVNG Nexus — Android starter

Cloud-build-ready Android project. No Android Studio is needed on the user's device.

## Build APK in GitHub Actions
1. Create a GitHub repository and upload the contents of this folder to its `main` branch.
2. Open the repository's **Actions** tab.
3. Select **Build LVNG Nexus APK** and press **Run workflow** (or wait for the first push build).
4. Open the completed run and download the `LVNG-Nexus-debug-APK` artifact.
5. Extract the downloaded artifact ZIP; install the APK on an Android device.

## Targets
- `minSdk 26`
- `targetSdk 35`
- `compileSdk 36`
- Intended testing range: Android 14–16, across manufacturers.

## Included in this starter
- Dashboard UI
- Floating overlay panel
- Accessibility gesture macro editor with coordinate taps and delays

## Current limitations
This is an early prototype, not a finished commercial app. Macro steps are not yet persisted and there is no touch recorder or swipe editor. Coordinate taps depend on display dimensions and game UI. Some manufacturers may restrict overlays or background services. Only enable Accessibility for features you understand and use macros where the game permits them.

The cloud workflow creates a debug APK for testing. A signed release build requires a private signing key; keep that key and its passwords private.
