# Medexs UK 0.25

Offline Android tablet tools for UCV re-verification, AHU service, pressure tests, equipment records and CAD viewing.

[Download APK](https://github.com/DangerousKitty666/Medexs/releases/download/v0.25/Medexs-0.25.apk) · [Release notes and complete source project](https://github.com/DangerousKitty666/Medexs/releases/tag/v0.25)

## New in 0.25

Re-verification starts with Job details, System description, Site survey and Balancing. The new 26-question survey provides calculated compliance and maintenance ratings, explicit assessment criteria and reasoned manual adjustments, all included in the PDF. System description offers reusable wording, Balancing uses spacious room cards and reading tables, section numbers include a dot, and the sidebar status is separated from the update button.

The assessment basis defaults to HTM 03-01 Part B (2021), Appendix 2; the supplied report's older Appendix B basis is separately selectable. Missing evidence never automatically receives Good. Ratings support engineer review and are not return-to-service authorisation.

## Install and storage

Android 8.0+, build 10, existing signing certificate. Install over the existing app to retain records. Uninstalling removes private jobs, equipment, photos and sign-in state. Reports normally copy to **Internal storage / Download / Medexs / Reports** on Android 10+, with a private app copy.

## Source and checks

Download **Medexs-0.25-Android-Studio.zip** from release assets for the complete project and tests. Automatic GitHub Source code archives contain repository documentation only. Keys, local settings and user records are excluded. Java 17/21 and Android SDK 35.

Survey, persistence, read-only, responsive layout, noise and calculation checks passed. Final installed APK passed Android 13 emulator checks for viewers, rotation, equipment and native PDFs for all four templates; survey PDF pages were visually inspected. Assembly/lint and signature verified. The known Windows SDK archive-close error occurred after Java classes were emitted; verified emitted classes were assembled and tested. Physical Samsung acceptance remains outstanding.

Manual company cloud sync is included from v0.24. Company sign-in and shared-folder read access were verified on 23 November 2026; live uploads and real cross-user equipment sync remain unverified.
