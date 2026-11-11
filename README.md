# Medexs UK 0.22

Offline Android tablet app for service jobs, PDF reports, equipment records and 2D/3D drawings.

[Download Medexs-0.22.apk](https://github.com/DangerousKitty666/Medexs/releases/download/v0.22/Medexs-0.22.apk) | [Release and complete Android Studio project](https://github.com/DangerousKitty666/Medexs/releases/tag/v0.22)

## Install

Android 8.0 or later. Install over the existing Medexs app to preserve jobs and equipment; do not uninstall first. Version 0.22 (code 4) retains the previous signing certificate. Keep Android System WebView up to date. Check for updates v-0.22 is at the bottom of the tool menu.

## Changes in 0.22

- Renamed Medexs UK, Service jobs and Recorded jobs; removed the introductory tagline; enlarged the logo within its existing background.
- + New job menu offers UCV Filter Change and Re-verification and AHU service. AHU jobs include filter changes, internal and coil cleaning, and photo sections.
- Gallery or camera attachments, multiple photos and editable captions. Action required service checks have individual notes.
- UCV filters are HEPA; AHU options are Pre-filter, Final filter (HEPA) and Recirculation filter (HEPA).
- Entrainment measurement rows can be added, deleted and reordered. Recorded points are highlighted on the grid.
- CAD viewers have black system bars, hidden navigation bars and immersive landscape, navigation controls enlarged by 20%, a standard-sized Back button and a larger 3D part information panel.
- PDF viewer defaults to 90% brightness, supports continuous vertical scrolling and pinch zoom, and adapts page columns to orientation.
- Generated PDF names follow Medexs - SR - Hospital - YYYY-MM-DD.pdf, with a suffix to prevent overwriting. Removed the outstanding-items list from generated reports.
- Jobs and saved reports can be deleted. Report deletion also removes its app-created Downloads copy where available; separately exported copies remain.

Shared company cloud synchronisation is deferred to version 0.23 pending IT setup. This release has no cloud sign-in, Sync button or cloud status indicators. All service work remains offline. Check for updates contacts GitHub only when pressed.

## Report storage

Android 10 and later: Internal storage / Download / Medexs / Reports (some file managers say Downloads). The app also retains a private internal copy under files/reports. Use Save a copy to choose another folder, including on Android 8-9 or if automatic copying fails. Jobs, equipment and photos are stored privately on the tablet. Uninstalling removes private app data.

## Android Studio source

Download the explicitly named Medexs-0.22-Android-Studio.zip release asset for the complete application; GitHub's automatic Source code archives contain the repository documentation only. Open the Medexs folder. Use Java 17 or 21, Android SDK 35, Gradle 8.9 and Android Gradle Plugin 8.7.3. Build using gradlew assembleDebug or gradlew assembleRelease. Initial builds need dependencies; the installed app bundles its offline assets.

To create a tablet emulator: Tools > Device Manager > + > Create Virtual Device > Tablet. Choose a profile and system image, then select it beside Run. Use the emulator rotation control to test landscape and portrait.

The release uses the existing local Android testing certificate for compatibility with earlier installations. Private signing files are excluded. A fresh source build uses your own local debug certificate and cannot update an APK signed by a different certificate. CAD/PDF bundles are included; Node is only needed to rebuild CAD assets. See VIEWER-ATTRIBUTION.txt and bundled dependency licences.

## Validation

Release assembly and lint, APK signature/version checks, calculation checks, browser job workflows and PDF scrolling/search/zoom/orientation checks were performed. This environment has not exercised installation, native camera/gallery, Android-generated PDF rendering or system-bar behaviour on a physical tablet; those need device acceptance testing.

Service results require engineer review. UCV final issue checks support the existing 2.8 m square canopy layout; other geometry needs a future template extension.
