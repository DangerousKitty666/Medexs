# Medexs UK 0.23

Offline Android tablet tools for UCV service, AHU cleaning/service, pressure tests, equipment records and CAD viewing.

[Download the APK](https://github.com/DangerousKitty666/Medexs/releases/download/v0.23/Medexs-0.23.apk) · [Release notes and full Android Studio project](https://github.com/DangerousKitty666/Medexs/releases/tag/v0.23)

## Changes

Direct verified APK updates with Android installation confirmation; compact versioned update button; in-page CAD measurement menus; instrument selection without type categories; instrument photos, read-only viewing, separate edit/delete; matching UCV/AHU report styling; positive and negative pressure-test templates. Cloud sync is deferred to **0.24**.

## Installation and storage

Android 8.0+. Install over the existing app to retain records; do not uninstall first. Version code 5 retains the earlier signing certificate. Install 0.23 once from the APK; subsequent updates use the new direct-download updater.

Reports are copied to **Internal storage / Download / Medexs / Reports** on Android 10+, with private copies in the app. Use Save a copy for another folder or Android 8–9.

## Source and validation

Download **Medexs-0.23-Android-Studio.zip** from release assets for the complete source. GitHub automatic Source code archives contain repository documentation only. Private signing keys and reports are excluded. Open the extracted Medexs project with Java 17 or 21 and Android SDK 35.

Build/lint, APK signature and automated workflow/calculation/viewer checks passed. Physical-tablet testing remains necessary for native installation, system bars, camera/gallery and PDF appearance. Pressure-test acceptance limits must be entered and confirmed for the project.
