# Medexs 0.21

Offline Android tablet tools for UCV service reporting, equipment records and CAD viewing.

[Download the installable APK and complete Android Studio source project](https://github.com/DangerousKitty666/Medexs/releases/latest).

Use **Medexs-0.21.apk** for installation, or **Medexs-0.21-Android-Studio.zip** for the full source with bundled offline viewers. Private signing keys and user records are excluded.

## Changes

Smaller icon artwork; HTM/DW reference library; PDF search and 70% default dimmer; compact dark CAD viewers with retained sessions; engineer dropdown; equipment register with calibration history and PDF certificates; instrument snapshots; square velocity grids; quadrant results; entrainment zones and target percentages; multiple filter photos included in PDFs; manual Check for updates.

## Installation and storage

Android 8.0+ with an up-to-date Android System WebView. Install over the existing Medexs tablet app to retain records; do not uninstall first.

On Android 10+, PDFs are copied to **Internal storage / Download / Medexs / Reports**. They also appear in **Saved PDFs** in the app. Use **Save a copy** to choose another location, including on Android 8–9.

## Android Studio

Open the extracted Medexs project root. Use Java 17 or 21 and Android SDK 35. For a tablet emulator: **Tools → Device Manager → + → Create Virtual Device → Tablet**, then select the device beside Run.

The release notes include build and test details. Physical-tablet acceptance testing remains necessary for native attachment selection and generated PDF output.
