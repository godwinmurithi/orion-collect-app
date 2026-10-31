# Orion Collect

**Orion Collect** is the Android app for filling in [OrionForms](https://orionterrametrics.com/product/orion-forms) in the field, online or offline. Sign in with your OrionGIS account and your forms are on the phone; submissions go straight back to OrionGIS, where they appear on your maps and dashboards.

- Product page: https://orionterrametrics.com/product/orion-collect
- User guide: https://orionterrametrics.com/docs/forms/orion-collect
- Download: [latest release](https://github.com/godwinmurithi/orion-collect-app/releases/latest)

> **Early access.** The current build (0.1.0-test2) is an Android test build, signed with a debug key. It is not yet on Google Play. Please report problems through [Issues](https://github.com/godwinmurithi/orion-collect-app/issues) or info@orionterrametrics.com.

## What it does

- Works offline: download forms once, fill them in without signal, send when you are back online.
- GPS points, photos, audio, barcodes, dates, choice lists, repeats and skip logic: everything OrionForms (XLSForm/ODK XForms) supports.
- Signs in with OrionGIS and sets up your projects for you: no server URLs or QR codes to type.
- Available in many languages.

## Requirements

- Android 8.0 or newer.
- An OrionGIS account (the free plan includes 2 forms and 250 submissions a month; see [pricing](https://orionterrametrics.com/#pricing)) with at least one OrionForms project you own.

## Install

1. On your Android phone, download `orion-collect-0.1.0-test2.apk` from the [latest release](https://github.com/godwinmurithi/orion-collect-app/releases/latest) or from https://orionterrametrics.com/product/orion-collect.
2. Open the file. If Android asks, allow your browser or file manager to **install unknown apps** (Settings → Apps → Special access → Install unknown apps).
3. Tap **Install**, then **Open**.

If you installed an earlier test build and the install fails, uninstall the old version first.

Optional: check the download. The SHA-256 of `orion-collect-0.1.0-test2.apk` is

```
6bc5a1539ba2ad7e1e71e460c636f76d98d365bedb21245ef3fe7dbac2217a41
```

## Sign in and collect

1. Open Orion Collect and tap **Sign in with OrionGIS**.
2. Enter your OrionGIS **username** and **password**. If you normally sign in with Google or Microsoft, first set a password on the OrionGIS website with **Forgot password**.
3. Orion Collect adds one project for each OrionForms project you own and downloads its forms.
4. Tap **Start new form**, fill it in and save it as **finalized**.
5. Tap **Send finalized forms** (or let it send automatically when you are online).
6. In OrionGIS, open the form to see the submission, on a map if the form has a GPS question.

Your password is used once to sign in and is not stored on the phone; the app keeps a device key per project instead.

## Privacy

Orion Collect sends form data only to OrionGIS (`orionterrametrics.com`). It has no advertising or third-party analytics; the upstream Firebase analytics and crash reporting are disabled in this build.

## Licence

Apache License 2.0. Orion Collect is based on ODK Collect; see `NOTICE.md`.
