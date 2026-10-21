# ONCHART downloads

[**Download ONCHART Launcher**](https://github.com/RicoHQ/onchart-releases/releases/latest/download/ONCHART.Setup.exe)

Run ONCHART.Setup.exe, choose **V2 Classic (2.7.12)** or **V3 Native (3.21.2)**, then install. Use **Installation folder → Change folder** to select another dedicated folder; existing versions and rollback history are copied and verified, and the old folder is kept as a backup. The launcher remembers your selection. Each family keeps its own installation, automatic update preference and previous version for rollback. V3 requires an active licensed account.

For offline installation, [download the complete installer ZIP](https://github.com/RicoHQ/onchart-releases/releases/download/v3.21.2/ONCHART_v3.21.2-installer.zip), extract the whole folder, and run ONCHART Setup.exe. Both families are bundled. No separate Python or Qt installation is required.

The installer includes the [complete changelog](https://github.com/RicoHQ/onchart-releases/releases/latest/download/CHANGELOG.html), searchable before installation. Updates are checked when the launcher opens and verified using the pinned release signature, SHA-256 and size. Close ONCHART before updating. Rollback turns automatic updates off until you enable them again.

- [Complete C++ version catalog](HISTORY.md)
- [All releases and version-specific changes](https://github.com/RicoHQ/onchart-releases/releases)
- [V2 portable package](https://github.com/RicoHQ/onchart-releases/releases/download/v2.7.12/ONCHART_v2.7.12-portable.zip)
- [V3 portable package](https://github.com/RicoHQ/onchart-releases/releases/download/v3.21.2/ONCHART_v3.21.2-portable.zip)

Historical packages retain their original bytes and curated version labels. Older binaries may show their pre-renumbering version text. Each historical release records its changes, original validation limitations and checksum; archive publication does not establish its original publication date or certify live game compatibility.

Private application source, backend credentials and signing keys are kept separately. Future versions require maintainer packaging, signing and publication; the launcher installs signed updates automatically when enabled. No background Windows service is installed.

This public repository contains compiled downloads, release notes and signed update metadata. Development source and release automation are private. GitHub-generated source ZIP/TAR links contain only this documentation and metadata.

## Phone remote

ONCHART 3.21.2 includes a paired local remote. [Download the Android app](https://github.com/RicoHQ/onchart-releases/releases/latest/download/ONCHART.Remote.apk). On iPhone, use Safari and Add to Home Screen. Enable Settings → Phone remote in ONCHART, then connect using the PC address and pairing code. [Connection and cable guide](MOBILE_REMOTE.md). No extra testing app is needed. Native iOS signing and physical phone/cable tests have not been performed.
