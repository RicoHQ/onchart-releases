# ONCHART downloads

[**Download ONCHART Launcher**](https://github.com/RicoHQ/onchart-releases/releases/download/launcher-v3.22.3/ONCHART.Setup.exe)

Run ONCHART.Setup.exe, choose **V2 Classic (2.7.12)** or **V3 Native (3.22.8)**, then install. Use **Installation folder → Change folder** to select another dedicated folder; existing versions and rollback history are copied and verified, and the old folder is kept as a backup. The launcher remembers your selection. Each family keeps its own installation, automatic update preference and previous version for rollback. V3 requires an active licensed account.

For the preserved 3.21.2 offline bundle, [download the complete installer ZIP](https://github.com/RicoHQ/onchart-releases/releases/download/v3.21.2/ONCHART_v3.21.2-installer.zip), extract the whole folder, and run ONCHART Setup.exe. Both families are bundled; its V3 seed is 3.21.2 and online updates advance it to 3.22.8. For the latest V3 without a network connection, use the full V3 portable package below. No separate Python or Qt installation is required.

The installer includes the [complete changelog](https://github.com/RicoHQ/onchart-releases/releases/download/v3.22.8/CHANGELOG.html), searchable before installation. Updates are checked when the launcher opens and verified using the pinned release signature, SHA-256 and size. Close ONCHART before updating. Rollback turns automatic updates off until you enable them again.

- [Complete C++ version catalog](HISTORY.md)
- [All releases and version-specific changes](https://github.com/RicoHQ/onchart-releases/releases)
- [V2 portable package](https://github.com/RicoHQ/onchart-releases/releases/download/v2.7.12/ONCHART_v2.7.12-portable.zip)
- [V3 portable package](https://github.com/RicoHQ/onchart-releases/releases/download/v3.22.8/ONCHART_v3.22.8-portable.zip)

Historical packages retain their original bytes and curated version labels. Older binaries may show their pre-renumbering version text. Each historical release records its changes, original validation limitations and checksum; archive publication does not establish its original publication date or certify live game compatibility.

Private application source, backend credentials and signing keys are kept separately. Future versions require maintainer packaging, signing and publication; the launcher installs signed updates automatically when enabled. No background Windows service is installed.

This public repository contains compiled downloads, release notes and signed update metadata. Development source and release automation are private. GitHub-generated source ZIP/TAR links contain only this documentation and metadata.

## Phone remote

ONCHART 3.22.8 includes typed phone forms for 94 tools, recent desktop worker results and approved-file selection for 13 existing-file inputs. Session index, Preview skin and Extension link also support approved existing folders. Rate, BPM and Bulk Rate support explicit Write-approved destinations and fresh export subfolders. Bulk dry run needs no loaded chart or destination and creates no files or folders. Approvals cover paired phones for the current session and can be revoked on the PC; global command/assistant/indirect-resource path permissions and other output workflows remain unfinished.

The Android app is Remote 1.1.5/build 8 and retains the original signing certificate. [Download the Android app](https://github.com/RicoHQ/onchart-releases/releases/download/v3.22.8/ONCHART.Remote.apk). On iPhone, use Safari and Add to Home Screen. Enable **Settings → Phone remote**, then connect using the PC address and pairing code. [Connection and cable guide](MOBILE_REMOTE.md). No extra testing app is needed.

The [ONCHART 3.22.8 release](https://github.com/RicoHQ/onchart-releases/releases/tag/v3.22.8) is published and offered by the signed V3 feed. All 20 native suites passed with 19 optional skips, phone core passed 51 checks, and one clean 15-case browser run passed across portrait, landscape and iPhone WebKit. Real Bulk Rate chart/audio exports were checked; this does not prove every workflow or physical phone works. Production launcher 3.22.3 verified the public archive signature, size and SHA-256, installed an isolated 3.22.6 → 3.22.8 update, reopened saved state and rolled back successfully. V2 remains 2.7.12. Live microphone testing was deferred; physical phone/cable, live music sync and a confirmed osu crash repair remain unverified. Full desktop-to-phone workflow parity is still in progress.
