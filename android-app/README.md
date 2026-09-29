# Android app

This folder turns the game into an Android APK. You don't need to touch it.

- The app opens the live game at thespectrumtechengine.com, so changes you
  push to the website show up in the app straight away.
- With no internet, the app falls back to a copy of the game built into the APK.
- Every push to `main` runs `.github/workflows/android-apk.yml`, which builds a
  signed APK and publishes it as a GitHub Release. The newest APK is always at:
  https://github.com/SpectrumTechEngine/Gravity-Trampoline-smiles/releases/latest/download/gravity-trampoline-smiles.apk

The signing key is NOT in this repo. It lives in GitHub secrets
(ANDROID_KEYSTORE_BASE64, ANDROID_KEYSTORE_PASSWORD) and in your backed-up
keys folder.
