# Medexs UK 0.235

Offline Android tablet tools for UCV service, AHU service, pressure tests, equipment records and CAD viewing.

[Download the APK](https://github.com/DangerousKitty666/Medexs/releases/download/v0.235/Medexs-0.235.apk) · [Release notes and full Android Studio project](https://github.com/DangerousKitty666/Medexs/releases/tag/v0.235)

## Stability fixes

Fixes the reproduced startup crash affecting both CAD viewers, PDF compatibility with older Android WebView versions, and viewer rotation handling. Adds recovery after WebView renderer failure and damaged report-index data, corrects future update version handling, and improves PDF section spacing. Cloud sync remains deferred to 0.24.

## Installation and storage

Android 8.0+. Version code 6 uses the existing signing certificate. Installing over the existing app retains records. If uninstalling, save any required reports first: uninstalling removes private app records.

Reports are copied to **Internal storage / Download / Medexs / Reports** on Android 10+, with private copies in the app. Use Save a copy for another folder or Android 8–9.

## Source and validation

Download **Medexs-0.235-Android-Studio.zip** from release assets for the complete source. GitHub automatic Source code archives contain repository documentation only. Private signing keys and user reports are excluded. Open the extracted Medexs project with Java 17 or 21 and Android SDK 35.

The installed APK was tested on Android 13 and Android 16 tablet emulators: CAD file loading, repeated viewer opening, model retention, measurement menus, rotation, equipment records and PDF generation/viewing for all four job types. A fresh-data Android 13 run also passed. Build, lint, signature, workflow and calculation checks passed. Physical Samsung hardware has not been tested. Pressure-test acceptance limits must be entered and confirmed for the project.
