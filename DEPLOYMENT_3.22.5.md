# ONCHART 3.22.5 — verified distribution

ONCHART 3.22.5 adds guided phone forms for 94 registered desktop tools, with typed inputs, an in-page review and explicit Run/Cancel. Editing requires a fresh review. The phone validates its connection and shows why unavailable actions are disabled.

Recent desktop worker jobs now retain their latest 20 results on the phone, including success/failure, duration and request correlation. Signing out clears that session history. The five-tab navigation and returning tool/chat views are corrected. Blue remains the default.

- [Windows installer / launcher](https://github.com/RicoHQ/onchart-releases/releases/download/v3.22.5/ONCHART.Setup.exe)
- [Desktop portable ZIP](https://github.com/RicoHQ/onchart-releases/releases/download/v3.22.5/ONCHART_v3.22.5-portable.zip)
- [Android Remote 1.1.2](https://github.com/RicoHQ/onchart-releases/releases/download/v3.22.5/ONCHART.Remote.apk)

All 17 native suites passed, with 19 explicit optional integration skips. Mobile core 27 checks, all five Chromium/WebKit touch-layout regressions and native-fixture portrait/landscape review/export-result checks passed. Package startup, 26 Qt library hashes, ZIP integrity and source/key exclusion passed. Remote 1.1.2/build5 retains the original Android signing certificate and all 11 tested web assets.

The desktop ZIP is 269903323 bytes; SHA-256 `1302b147eb3df9e3621234e3eaa502e12e136ba0065afd5b3002f39301835842`.

The published launcher verified the original-key signature and public ZIP size/hash, installed an isolated 3.21.2 baseline, updated it to 3.22.5, reopened saved state and rolled back. The signed V3 feed and its database mirror now select the identical 3.22.5 envelope; V2 remains 2.7.12. The existing launcher remains version 3.22.3; it independently selects the desktop app from the signed feed. Prior releases and archives are preserved; application source and signing keys are excluded.

Limits: generic forms and a worker journal do not provide complete guided mobile parity. Scoped file selection, extension-aware availability and unified progress/cancellation remain planned. Physical Android/iPhone, USB, native iOS, live microphone responsiveness and live-game crash freedom are unverified. No new production wake or osu! crash fix is claimed.


The desktop package contains 348 runtime/documentation files.
All 238 frozen source inputs matched before/after packaging. The private source
backup remains local; it was excluded from the nine public release assets.
The APK SHA-256 is `53b0a69f81ce468c7415df6cbba9156b09bc013b76872ada6a9c671144cf0297`.

Evidence: `qa/3225/native-gate-20261025T084635Z/summary.json`,
`browser-current/check.json`, `forms-jobs-browser.json`, `portable-package.json`,
`signature-check.json`, `github-publication.json`, `android-build-check.json`,
`live-update-check.json`, `live-feed-check.json` and `registry-check.json`.

The first update-test harness failed during baseline extraction because its
workspace path exceeded .NET Framework path limits. That failure is preserved in
`live-update-deep-path-failure.json`; the successful run used a shorter isolated
workspace path. This does not verify arbitrary long installation paths. The
normal installation and games were not modified or launched by the check.

Published archives remain byte-for-byte sealed; this report records subsequent
public verification. The website's dedicated launcher URL remains compatible:
launcher 3.22.3 independently selects the current desktop app through its signed
feed. No application source, private key, new credential or publishing automation
was added to the public repository.

