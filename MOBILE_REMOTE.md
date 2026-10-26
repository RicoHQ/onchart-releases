# ONCHART Remote 1.1.3

The default interface and app icons use ONCHART's blue accent (#38bdf8) with navy backgrounds. Choose another accent in **More → Remote theme**; it saves on that phone. Desktop 3.22.6 includes this interface; the signed Android app is version 1.1.3.

Update the Android app to receive the new icon. For an existing iPhone home-screen shortcut that retains the old icon, remove and re-add the shortcut from Safari after updating ONCHART on the PC.

The phone remote works with **ONCHART V3 Native 3.22.0 or newer**. V2 Classic does not include its desktop server.

## Connect over Wi-Fi or LAN

1. Start ONCHART on the PC and sign in normally.
2. Open **Settings → Phone remote** and enable the remote for this session.
3. Put the phone and PC on the same trusted network. If Windows asks, allow ONCHART on **Private** networks. Guest Wi-Fi may isolate devices.
4. On Android, install the signed **ONCHART.Remote.apk**, or open one of the listed PC addresses in Chrome. On iPhone, open the address in Safari.
5. Enter the computer address and the six-digit code shown on the PC. The browser version fills in its current address automatically.

On iPhone, Safari **Share → Add to Home Screen** provides a home-screen remote. Chrome can also add a home-screen shortcut. The local browser version requires ONCHART running; local HTTP does not provide an offline service worker. The Android APK contains its own interface and can show connection help while the PC is unavailable.

No extra testing app or phone account is required. A native iOS project is included in the private development files; producing and signing an iOS binary requires macOS/Xcode and an appropriate Apple signing identity. A Windows build must not be described as a tested native iPhone binary.

## Connect using a cable

Use a data-capable cable. Charging alone does not create a network connection.

- **Android:** enable USB tethering and use the PC address belonging to the USB network adapter. The PC still needs to allow inbound ONCHART traffic on that private network.
- **Android developer USB:** with the phone authorized for USB debugging, run `adb reverse tcp:24060 tcp:24060` on the PC, then connect the Android app to `http://127.0.0.1:24060`. This forwards only the remote port. Disable USB debugging when finished if it is not normally needed.
- **iPhone:** enable Personal Hotspot over USB, trust the PC and install Apple's device drivers if Windows requires them. Use the PC's USB network address. This route requires the USB network to permit phone-to-PC traffic; it is not a generic raw-USB protocol.

The same pairing and controls apply to every route. Physical phones, cables, drivers and router/firewall combinations require their own live verification; browser tests alone do not establish that a particular cable works.

## Controls

- Current chart, selected game, key count, BPM, note count and chart-density display.
- Silent visual-preview play/pause, restart, seeking and chart rate. Timing follows the actual preview clock, including desktop speed multipliers and game-following rates. Loaded replays keep their recorded rate; clear a replay on the PC before changing chart rate. These controls do not change or inject input into a running rhythm game.
- Practice-loop start/end points, and return to game-following compact view.
- Recent single-chart files through opaque identifiers; native simfile difficulty selection remains on the PC.
- Full LN, No LN, Inverse, No SV and Chordjackify selection. The LN conversion mods remain mutually exclusive. Export creates a new difficulty and preserves the original. Check ONCHART's activity log for the output or failure details.
- Desktop page navigation and music-pulse, compact-view and low-end settings.
- The **Tools** tab exposes the desktop's typed terminal command catalog, including chart editing, rate and bulk-rate tools, pack generation, conversions, images, analytics, sessions, overlays, extensions, marathon workflows, preview options and supported named controls. Search an action, review its help/example, then confirm it before sending. Commands run through ONCHART's parser; there is no shell endpoint.
- AI Assistant text chat, recent assistant messages, desktop activity output and a phone action to start the PC microphone. The assistant uses the configured desktop provider and bundled local speech recognizer. Microphone access remains subject to Windows privacy settings; the phone must explicitly confirm before capture begins. The recorder stops after a pause or its existing 15-second limit.
- Phone push-to-talk, where the phone/browser exposes microphone capture: tap **Record from phone**, speak for up to 10 seconds, and tap **Finish and review**. Allow microphone permission when requested. A short mono WAV goes only to the paired PC over the local connection and is transcribed by the bundled offline Whisper runtime. ONCHART returns the recognized words to the phone; choose **Use latest recognized words** and **Send message** to continue. Audio does not auto-run a command or go to the configured AI provider. Capture stops on cancel, app backgrounding, disconnect or the ten-second limit. If your browser disables microphone capture at its local HTTP address, use the separate **PC microphone** action; a signed native iOS app is not currently released.
- Landscape layout uses a wider two-column control view and exposes the tool catalog beside the session controls.

## Pairing and connection behavior

The remote is off at every desktop start. Pairing codes expire after three minutes. Up to four phones can pair; **Disconnect all phones**, turning the remote off or signing out revokes them. Session tokens are kept hashed in desktop memory, and the phone retains its token only for its current app/browser session. Idle sessions expire after twelve hours.

Use a trusted local network. The connection is local HTTP, so it does not encrypt traffic against other devices monitoring that network. Do not expose or port-forward the remote to the internet. The server limits private IPv4 peers, validates host/origin headers, and requires pairing for state and commands. Tools call only commands documented by ONCHART's parser; there is no shell command or filesystem browsing endpoint.

The client backs off after connection loss, pauses polling in the background and does not replay a button press when reconnecting. Duplicate command identifiers are handled once by the server. Clock interpolation is bounded to fresh samples and stops when the desktop clock is not advancing. Sliders submit on release; static screens do not run a permanent animation loop. File-taking tools use their documented ONCHART command and path arguments, so paths must be supplied on the phone; native Windows file dialogs and simfile difficulty dialogs still require desktop interaction.

## Build and verification

The private mobile project is in `mobile-remote`. Use Node 22.12+ (the validated build environment uses Node 24), `npm ci`, `npm run build`, and `npm test`. Its generated `remote.qrc` embeds compiled assets in the desktop application; it is not a development source distribution. Android builds use the workspace-local JDK/SDK and `mobile-remote/Build-Android.ps1`; signing material stays under the excluded `.tools/mobile/signing` directory and is never a public asset.

The native protocol/integration tests are `onchart_remote_tests`; browser end-to-end tests use an isolated desktop fixture and Chromium/WebKit phone-sized viewports. Release-specific results and limitations belong in `RELEASE_3.22.3.md` and the complete generated changelog. Third-party notices ship with the mobile assets and desktop documentation.

## Approved PC files in 3.22.6

Approve a read-only folder in Settings → Phone remote on the PC. The phone can browse it and choose files for 13 supported existing-file inputs, review the filename and explicitly run the action. Approval covers paired phones for the current session and can be revoked on the PC. Directory/output selection and global command/assistant/indirect-resource path permissions remain unfinished; this picker does not restrict every existing desktop tool.

The release passed 20 native suites (19 optional skips), 40 phone-core checks and 30 browser checks across six profiles. Selected map-open is the end-to-end reference. Physical Android/iPhone, USB and live microphone/game tests remain unverified. Safari/home-screen remains the iPhone delivery route; separate native iOS packaging is outside the current roadmap.
