# ONCHART app 3.22.3 — verified distribution, 25 October 2026

The desktop APP is published as [v3.22.3](https://github.com/RicoHQ/onchart-releases/releases/tag/v3.22.3).
The separate launcher-v3.22.3 tag remains available. The live signed V3 app-update
feed now selects 3.22.3; V2 still selects 2.7.12. The existing update database
contains the identical immutable signed 3.22.3 envelope, with prior rows retained.

- [Installer / launcher](https://github.com/RicoHQ/onchart-releases/releases/download/v3.22.3/ONCHART.Setup.exe)
- [Full V3 portable ZIP](https://github.com/RicoHQ/onchart-releases/releases/download/v3.22.3/ONCHART_v3.22.3-portable.zip)
- [Signed Android Remote 1.1.1](https://github.com/RicoHQ/onchart-releases/releases/download/v3.22.3/ONCHART.Remote.apk)
- [Signed V3 metadata](https://raw.githubusercontent.com/RicoHQ/onchart-releases/main/channels/v3.json)

The ZIP is 269872656 bytes; SHA-256:
`c5c8c48eaf758af33ede562d8f2e4b6bbcbec6490ab48d733c82cec1dc86c392`.
Its executable reports ONCHART 3.22.3. The coherent Release build and all 16
native suites passed; all 217 frozen build inputs matched. System-only-PATH
startup, 26 Qt SDK library hashes, ZIP integrity and source/key exclusion passed.
GitHub verified the server size/SHA-256 of all nine published assets.

The actual published launcher engine verified the original-key signature and
public download, installed a fresh isolated 3.21.2 baseline, updated it to 3.22.3,
matched the installed executable to the final build, reopened saved state and
rolled back. Rollback disabled automatic updates as intended. The real launcher
then fetched the live V3 feed, verified its RSA signature and matched the exact
3.22.3 envelope. The V2 signed feed separately verified as 2.7.12. The normal user
installation, shortcuts/registry and game processes were not changed by the test.

Signing used the original trusted DPAPI signer account. Uploads used the existing
RicoHQ Git sign-in in the normal Windows account. No key copy, new credential,
public application source or persistent publishing workflow was introduced.
Earlier archives and the rejected mixed candidate remain preserved privately.

The website repository's five launcher links target the dedicated setup asset.
Its updated source commit a5f477afebb633c750257bd469799dbdd12967fd passed
Cloudflare's Workers Builds: onchart check. The live site URL/buttons have not
yet been verified; source/deployment success is not a live-button test.

Limits: optional native live-integration checks remain skipped where fixtures
were absent. No physical-phone, USB, native-iOS, real microphone latency/false
activation or live-game crash-freedom result is claimed. Instant wake activation
is not guaranteed, and full guided mobile parity remains planned. Runtime ZIPs
remain byte-for-byte unchanged; this report supplements their assembly-time docs.
