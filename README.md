# Medexs UK 0.26

Offline Android tablet tools for UCV re-verification, AHU service, pressure tests, equipment records and CAD viewing.

[Download APK](https://github.com/DangerousKitty666/Medexs/releases/download/v0.26/Medexs-0.26.apk) · [Release notes and complete source project](https://github.com/DangerousKitty666/Medexs/releases/tag/v0.26)

## New in 0.26

Choose an AHU and plantroom survey (40 questions) or theatre suite survey (26 questions), checked against Sancta Maria, Prince Philip, Dumfries and Fortius reports. Each form retains its own answers. Scoring now uses the correct AHU question groups and theatre defect severity, with semantic answer colours, incomplete-evidence checks and reasoned manual adjustments. Both formats are included in native PDF generation.

Balancing uses one row per terminal or pressure measurement, side-by-side operating-mode columns and compact supply/extract room summaries. Select UCV, conventional or both; switching preserves readings and the PDF shows only the selected modes. The field-service line is removed and Company sync explicitly shows signed-in status separately from shared-folder verification.

The theatre assessment basis offers HTM 03-01 Part B (2021), Appendix 2 at 18 AC/h, or the supplied reports' Appendix B at 75% of design. AHU scoring follows Appendix A. Missing evidence never automatically receives Good. Ratings support engineer review, not return-to-service authorisation; full rules and interpretations are documented in the app and release attachments.

## Install and storage

Android 8.0+, build 11, existing signing certificate. Install over the existing app to retain records. Uninstalling removes private jobs, equipment, photos and sign-in state. Reports normally copy to **Internal storage / Download / Medexs / Reports** on Android 10+, with a private app copy.

## Source and checks

Download **Medexs-0.26-Android-Studio.zip** from release assets for the complete project and tests. Automatic GitHub Source code archives contain repository documentation only. Keys, local settings and user records are excluded. Java 17/21 and Android SDK 35.

Survey scoring/persistence, read-only views, responsive layouts, noise, calculations, account status and equipment interface checks passed. Android 13 emulator checks covered both CAD viewers, files, measurement menus, repeated reopening and rotation, plus native PDFs for all job templates and both survey formats. Generated PDF content and layouts were checked. Assembly/lint passed with zero lint errors; version and signature verified. The known Windows Java archive-close error occurred after classes were emitted; verified updated classes were assembled and tested in the installed APK. Physical Samsung acceptance remains outstanding.

Manual company cloud sync is included from v0.24. Company sign-in and shared-folder reads were verified on 23 November 2026; live uploads and real cross-user equipment sync remain unverified. Version 0.26 changes account-status display, not cloud permissions or upload behaviour.
