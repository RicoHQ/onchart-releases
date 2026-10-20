# ONCHART — Complete reconstructed changelog

Updated 20 October 2026 from the local source archive, packaged documentation,
release notes, source comparisons and release-rename index. Covers **125 distinct
saved version labels in 126 entries**: 49 single-file Python snapshots, eight
modular Python snapshots, one parallel C prototype and 63 native Qt C++ builds.
The C prototype and modular Python rewrite both use 3.0.0 and are described separately.

This is a reconstruction of preserved evidence. Older Python applications were
**not executed or imported**. Their behavior is described from source; historical
test totals are attributed to their saved reports, not presented as fresh tests.
Not every saved snapshot was necessarily publicly released.

Version labels 1 and 2 are retained as found; no invented 1.0.0 or 2.0.0 release
is inserted. Native releases originally sharing 3.2.12 branding were later renamed
from 3.3.0 by modified-date order. Folder/ZIP timestamps are artifact metadata,
**not confirmed publication dates**. Exact index times and identity hashes are in
[CHANGELOG_INVENTORY.csv](CHANGELOG_INVENTORY.csv).

The early native notes are cumulative and not a reliable first-introduction date
for every sentence. Modular Python folders can also differ from their original
ZIPs. Those distinctions, duplicate copies, syntax failures and absent releases
are retained rather than converted into unsupported feature claims.

**Current crash status:** 3.14.7 corrected a reproduced reader defect. On 18 October 2026, offline analysis of the latest original-client dump confirmed recursive game-update dispatch. An isolated, signed official client also crashed with OnChart closed and a separate empty profile. On 20 October 2026, another original-client baseline exited with System.StackOverflowException before the current reader attached. The initiating cause remains unidentified; no lasting game-crash repair is claimed.

**Hosted speech validation:** 3.18.8: native offline recognition and durable training queue checks passed. Authenticated live training storage write/read/export/deletion passed. Accepted prompt audio and observable conversation records are retained for future training, with pause/delete controls. Actual personalized recognition improvement is unmeasured. Cloudflare speech is currently blocked by the account daily free AI allowance; voices/configuration are preserved and billing is unchanged. Live osu/lazer gameplay crash freedom is unverified.


## Version index

| Version | Generation | Main change |
| --- | --- | --- |
| [1](#python-1) | Python 1.x / 2.x | Original pack maker |
| [1.1](#python-1-1) | Python 1.x / 2.x | Pack metadata and naming controls |
| [1.2](#python-1-2) | Python 1.x / 2.x | Automatic Songs-folder discovery |
| [1.3](#python-1-3) | Python 1.x / 2.x | UI proposal recorded in comments |
| [1.4](#python-1-4) | Python 1.x / 2.x | Tabbed settings interface |
| [1.5](#python-1-5) | Python 1.x / 2.x | Pack-folder synchronization and safer dispatch |
| [1.5.4](#python-1-5-4) | Python 1.x / 2.x | Separate difficulty-name formatting and smaller layout |
| [1.5.7](#python-1-5-7) | Python 1.x / 2.x | Scrollable pages and selectable UI scale |
| [1.6](#python-1-6) | Python 1.x / 2.x | Packing format-call correction |
| [1.7](#python-1-7) | Python 1.x / 2.x | Complete Version-format placeholders |
| [1.7.2](#python-1-7-2) | Python 1.x / 2.x | Narrow blue layout and practical scaling |
| [1.8](#python-1-8) | Python 1.x / 2.x | Rate conversion, patterns, hotkeys and terminal |
| [1.8.2](#python-1-8-2) | Python 1.x / 2.x | Pack-oriented rate output and priority hotkeys |
| [1.8.7](#python-1-8-7) | Python 1.x / 2.x | Complete assets and metadata for rate copies |
| [1.8.11](#python-1-8-11) | Python 1.x / 2.x | FFmpeg discovery |
| [1.9](#python-1-9) | Python 1.x / 2.x | Bundled-encoder fallback |
| [1.9.3](#python-1-9-3) | Python 1.x / 2.x | Modifier compatibility and audio-result checks |
| [1.9.6](#python-1-9-6) | Python 1.x / 2.x | Identical saved copy |
| [2](#python-2) | Python 1.x / 2.x | Slate/indigo interface refresh |
| [2.0.1](#python-2-0-1) | Python 1.x / 2.x | Dense-pattern labels retain their type |
| [2.1.0](#python-2-1-0) | Python 1.x / 2.x | Animated rounded visual system |
| [2.1.1](#python-2-1-1) | Python 1.x / 2.x | Rate-copy background section handling |
| [2.1.2](#python-2-1-2) | Python 1.x / 2.x | Windows frame styling |
| [2.1.3](#python-2-1-3) | Python 1.x / 2.x | Section-aware BPM parsing and title-bar colours |
| [2.1.4](#python-2-1-4) | Python 1.x / 2.x | Reliable Windows title-bar repaint |
| [2.1.5](#python-2-1-5) | Python 1.x / 2.x | Rounded entries and draggable scrollbars |
| [2.1.6](#python-2-1-6) | Python 1.x / 2.x | Single rate-dialog instance |
| [2.1.7](#python-2-1-7) | Python 1.x / 2.x | Batch metadata override page |
| [2.2.1](#python-2-2-1) | Python 1.x / 2.x | Explicit batch-pack action and branding |
| [2.3.0](#python-2-3-0) | Python 1.x / 2.x | Persistent settings and command editing |
| [2.4.0](#python-2-4-0) | Python 1.x / 2.x | Curated pack builder and inline console |
| [2.5.1](#python-2-5-1) | Python 1.x / 2.x | tosu stable/lazer paths and OSZ export |
| [2.5.4](#python-2-5-4) | Python 1.x / 2.x | Fresh batch targets and lazer safeguards |
| [2.5.5](#python-2-5-5) | Python 1.x / 2.x | Hotkey deduplication and fresh rate input |
| [2.5.6](#python-2-5-6) | Python 1.x / 2.x | Per-song pitch control attempt; broken snapshot |
| [2.5.7](#python-2-5-7) | Python 1.x / 2.x | Syntax repair and numeric difficulty bounds |
| [2.5.9](#python-2-5-9) | Python 1.x / 2.x | Quiet Windows subprocesses |
| [2.6.1](#python-2-6-1) | Python 1.x / 2.x | Background converter and filename-aware edits |
| [2.6.4](#python-2-6-4) | Python 1.x / 2.x | Full-effects preview and coloured outlines |
| [2.6.11](#python-2-6-11) | Python 1.x / 2.x | Identical saved copy |
| [2.6.14](#python-2-6-14) | Python 1.x / 2.x | Deterministic banded glitch distortion |
| [2.6.15](#python-2-6-15) | Python 1.x / 2.x | Milder glitch distribution |
| [2.7.4](#python-2-7-4) | Python 1.x / 2.x | Dense scanline distortion |
| [2.7.5](#python-2-7-5) | Python 1.x / 2.x | Shared outline implementation |
| [2.7.6](#python-2-7-6) | Python 1.x / 2.x | Pack manifests, rate precision and band thickness |
| [2.7.9](#python-2-7-9) | Python 1.x / 2.x | Generated-background references and replacement choice |
| [2.7.10](#python-2-7-10) | Python 1.x / 2.x | Unclipped outline margins |
| [2.7.11](#python-2-7-11) | Python 1.x / 2.x | Case-insensitive background lookup |
| [2.7.12](#python-2-7-12) | Python 1.x / 2.x | Full LN / No LN mod attempt; broken snapshot |
| [3.0.0](#python-3-0-0) | Modular Python 3.x | Modular PySide6 / Qt6 rewrite |
| [3.0.9](#python-3-0-9) | Modular Python 3.x | Blue themes, background converter and rate rounding |
| [3.1.7](#python-3-1-7) | Modular Python 3.x | MSD integration, queued packer and configurable paths |
| [3.1.8](#python-3-1-8) | Modular Python 3.x | Graphical MSD bars and packaging support |
| [3.1.9](#python-3-1-9) | Modular Python 3.x | Duplicate modular source snapshot |
| [3.2.0](#python-3-2-0) | Modular Python 3.x | Configurable MSD, rate presets and richer previews |
| [3.2.12](#python-3-2-12) | Modular Python 3.x | Preserved Python beta and native migration workspace |
| [3.2.13](#python-3-2-13) | Modular Python 3.x | Divergent Python snapshot with converter/packaging work |
| [3.0.0](#c-3-0-0) | Win32 C prototype | Separate Win32 C prototype |
| [3.3.0](#native-3-3-0) | Native Qt C++ | Renumbered native baseline |
| [3.4.0](#native-3-4-0) | Native Qt C++ | Website login package |
| [3.5.0](#native-3-5-0) | Native Qt C++ | Analytics timeline, bulk rates and grouped navigation |
| [3.5.1](#native-3-5-1) | Native Qt C++ | Continuous backgrounds and readable fields |
| [3.5.2](#native-3-5-2) | Native Qt C++ | Rounded checkbox states |
| [3.6.0](#native-3-6-0) | Native Qt C++ | Shared skinned mania preview |
| [3.6.1](#native-3-6-1) | Native Qt C++ | Alignment, hold playback and renderer efficiency |
| [3.6.2](#native-3-6-2) | Native Qt C++ | Rounded hold caps and per-hold animation |
| [3.7.0](#native-3-7-0) | Native Qt C++ | Replay playback and MP4 export |
| [3.7.1](#native-3-7-1) | Native Qt C++ | Tap visibility over hold tails |
| [3.8.0](#native-3-8-0) | Native Qt C++ | Direct export settings dialog |
| [3.9.0](#native-3-9-0) | Native Qt C++ | Detached preview and local replay chooser |
| [3.10.0](#native-3-10-0) | Native Qt C++ | Skin HUD, keystrokes and KPS graph |
| [3.10.1](#native-3-10-1) | Native Qt C++ | New account-site connection |
| [3.10.2](#native-3-10-2) | Native Qt C++ | Exact rolling KPS and mania accuracy |
| [3.11.0](#native-3-11-0) | Native Qt C++ | Local diagnostics and opt-in FDP |
| [3.11.1](#native-3-11-1) | Native Qt C++ | Native release without expiry or FDP |
| [3.11.2](#native-3-11-2) | Native Qt C++ | Passive input and bounded live history |
| [3.12.0](#native-3-12-0) | Native Qt C++ | Four-mode previews and expanded map processing |
| [3.13.0](#native-3-13-0) | Native Qt C++ | Linked MugDiffusion and DanOverlay extensions |
| [3.13.2](#native-3-13-2) | Native Qt C++ | .osu generation templates |
| [3.13.3](#native-3-13-3) | Native Qt C++ | Automatic Dan and simpler AI inputs |
| [3.13.4](#native-3-13-4) | Native Qt C++ | Built-in native osu! reader |
| [3.13.5](#native-3-13-5) | Native Qt C++ | Mode skins, taiko timing, catch movement and icon |
| [3.13.6](#native-3-13-6) | Native Qt C++ | Multi-ladder clickable Dan card |
| [3.14.0](#native-3-14-0) | Native Qt C++ | Initial Compact Mode saved build |
| [3.14.1](#native-3-14-1) | Native Qt C++ | Compact visibility and portable Qt deployment |
| [3.14.2](#native-3-14-2) | Native Qt C++ | Shorter Compact Mode |
| [3.14.3](#native-3-14-3) | Native Qt C++ | Denser compact columns and preview |
| [3.14.4](#native-3-14-4) | Native Qt C++ | Private-JIT scans and crash investigation |
| [3.14.5](#native-3-14-5) | Native Qt C++ | Rate retiming, Dan output and MSD validation |
| [3.14.6](#native-3-14-6) | Native Qt C++ | Global scaling, density marker and local overlays |
| [3.14.7](#native-3-14-7) | Native Qt C++ | Data-slot caching and readable-range checks |
| [3.15.0](#native-3-15-0) | Native Qt C++ | Compact keys, browser data rendering and independent difficulty |
| [3.15.1](#native-3-15-1) | Native Qt C++ | JKPS-style compact keystrokes at the bottom |
| [3.16.0](#native-3-16-0) | Native Qt C++ | 4K sessions, skill memory, session planner and Bulk Rate presets |
| [3.16.1](#native-3-16-1) | Native Qt C++ | Theme-aware session curves and four-game chart profiles |
| [3.16.2](#native-3-16-2) | Native Qt C++ | Structured terminal command workspace |
| [3.17.0](#native-3-17-0) | Native Qt C++ | Player Tools and complete MugDiffusion menus |
| [3.17.1](#native-3-17-1) | Native Qt C++ | Player Tools review and convenience fixes |
| [3.17.2](#native-3-17-2) | Native Qt C++ | Smoother scaling and compact MugDiffusion pattern rows |
| [3.17.3](#native-3-17-3) | Native Qt C++ | Uninterrupted scale dragging and visual verification |
| [3.18.0](#native-3-18-0) | Native Qt C++ | Natural voice and chat assistant, selected-game loaders |
| [3.18.1](#native-3-18-1) | Native Qt C++ | Safer osu! polling and concise assistant replies |
| [3.18.2](#native-3-18-2) | Native Qt C++ | Local voice control and map-folder rate outputs |
| [3.18.4](#native-3-18-4) | Native Qt C++ | Offline voice recognition and safer osu! isolation |
| [3.18.5](#native-3-18-5) | Native Qt C++ | Discord-TTS reply speech service |
| [3.18.6](#native-3-18-6) | Native Qt C++ | Microphone setup, local speech detection and current-map recovery |
| [3.18.7](#native-3-18-7) | Native Qt C++ | Local voice memory and Dan-target rate copies |
| [3.18.8](#native-3-18-8) | Native Qt C++ | Training storage, new converters and persistent skinning |
| [3.18.9](#native-3-18-9) | Native Qt C++ | Content-fitting menus and readable scaled bulk presets |
| [3.18.10](#native-3-18-10) | Native Qt C++ | Complete ADOFAI hit streams and distinct navigation icons |
| [3.18.11](#native-3-18-11) | Native Qt C++ | Rhythia geometry, Higgsfield skin prompts and square receptors |
| [3.18.12](#native-3-18-12) | Native Qt C++ | Distinct sidebar icons, all-key random streams and mania skin keys |
| [3.18.13](#native-3-18-13) | Native Qt C++ | Responsive settings, song ambience, stable app identity and voice tools |
| [3.18.14](#native-3-18-14) | Native Qt C++ | Skin generator below the preview |
| [3.18.15](#native-3-18-15) | Native Qt C++ | Bundled Discord-TTS and blue Windows branding |
| [3.18.16](#native-3-18-16) | Native Qt C++ | Map preview receptor squish control |
| [3.18.17](#native-3-18-17) | Native Qt C++ | ADOFAI compatibility and preview refinements |
| [3.19.0](#native-3-19-0) | Native Qt C++ | Windows installer and signed automatic updates |
| [3.20.0](#native-3-20-0) | Native Qt C++ | V2/V3 installer, embedded changelog and archived release history |
| [3.20.1](#native-3-20-1) | Native Qt C++ | Binary search for danrate |
| [3.21.0](#native-3-21-0) | Native Qt C++ | Live music, mod cards, installer folders and service recovery |
| [Site 2026.10.17](#website-2026-10-17) | Website | Premium public website refresh |
| [Site 2026.10.17.2](#website-2026-10-17-2) | Website | React Bits experience additions |
| [Site 2026.10.17.3](#website-2026-10-17-3) | Website | Staff cards and continuous backgrounds |
| [Site 2026.10.20](#website-2026-10-20) | Website | Launcher downloads and V2/V3 setup |
| [Speech 2026.10.18.1](#speech-2026-10-18-1) | Speech service | Direct Discord-TTS audio forwarding |

## Single-file Python history

Comparisons follow the saved version labels, across the v1/v2 boundary. Static syntax checks do not certify runtime correctness. Comment-only and identical copies are explicitly identified.

<a id="python-1"></a>

### 1 — Original pack maker

- First saved single-file Python implementation. Polls the local tosu v2 endpoint for the selected map and its title, difficulty, OD, HP, BPM, creator, background and audio.
- Copies the selected .osu and associated audio/background into a pack folder, rewriting exported references and pack metadata.
- Provides overwrite, skip and increment collision handling, a packing hotkey, a monitor thread and an optional Tk information window.
- The Songs/output location is hard-coded in this snapshot. USE_LAZER is a placeholder, not implemented lazer support.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart v1.py](<../../../1/onchart v1.py>).

<a id="python-1-1"></a>

### 1.1 — Pack metadata and naming controls

- Adds artist and source to the live state, information display and exported metadata.
- Adds configurable creator override, optional Various Artists output, a difficulty-name format and an appended pack tag.
- Updates Unicode artist/title metadata consistently with the generated pack metadata.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart v1.1.py](<../../../1/onchart v1.1.py>).

<a id="python-1-2"></a>

### 1.2 — Automatic Songs-folder discovery

- Searches common Windows osu! Songs locations instead of requiring one fixed installation path.
- Derives the default osupack directory from the discovered Songs folder; falls back to a relative osupack directory when detection fails.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart v1.2.py](<../../../1/onchart v1.2.py>).

<a id="python-1-3"></a>

### 1.3 — UI proposal recorded in comments

- The saved file adds UI-upgrade notes proposing a pack-name field, duplicate-mode dropdown, Various Artists checkbox and Settings tab.
- Executable functions are unchanged from 1.2. These comments do not establish that those proposed controls were implemented in this version.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart v1.3.py](<../../../1/onchart v1.3.py>).

<a id="python-1-4"></a>

### 1.4 — Tabbed settings interface

- Reworks the window into Current Map and Settings notebook pages with a dark theme, prominent Pack Now action and status feedback.
- Exposes pack name, duplicate handling and Various Artists settings through the GUI.
- Revises packing and GUI synchronization to consume the settings and report status without replacing the live map display.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart v1.4.py](<../../../1/onchart v1.4.py>).

<a id="python-1-5"></a>

### 1.5 — Pack-folder synchronization and safer dispatch

- Derives a pack folder from the pack name and keeps the displayed destination synchronized as the name changes.
- Introduces a shared trigger for threaded packing, with explicit settings snapshots and clearer success/error status.
- Restructures field/section helpers and Current Map/Settings layouts; removes the older print_info/update_gui arrangement.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart v1.5.py](<../../../1/onchart v1.5.py>).

<a id="python-1-5-4"></a>

### 1.5.4 — Separate difficulty-name formatting and smaller layout

- Adds a Difficulty Name Format field and placeholders for title, difficulty, OD, HP, BPM, creator, artist and source.
- Separates generated naming from the exported Version field in the packing code.
- Reduces the default window to 700×500 and its minimum to 480×320.
- The saved formatting implementation is transitional; subsequent 1.5.7, 1.6 and 1.7 changes correct the field wiring and placeholder handling.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v1.5.4.py](<../../../1/onchart_v1.5.4.py>).

<a id="python-1-5-7"></a>

### 1.5.7 — Scrollable pages and selectable UI scale

- Wraps Current Map and Settings in vertically scrollable containers.
- Adds a UI Scale selector with 0.75–1.5 choices and an independent Version Format field.
- Reworks the naming expressions, but the saved source mistakenly calls an already formatted string as a function in the packing path. This is a source-visible defect, corrected in 1.6; a successful runtime release is not claimed.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart v1.5.7.py](<../../../1/onchart v1.5.7.py>).

<a id="python-1-6"></a>

### 1.6 — Packing format-call correction

- Removes the erroneous second call on the formatted string introduced in 1.5.7.
- Reconnects the exported .osu Version field to the Version Format control instead of the unrelated difficulty-name format.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart v1.6.py](<../../../1/onchart v1.6.py>).

<a id="python-1-7"></a>

### 1.7 — Complete Version-format placeholders

- Passes title, OD, HP and source into Version formatting alongside the previously supplied difficulty, creator, BPM and artist.
- Updates the control hint to list the supported placeholders, avoiding missing-key failures when those additional fields are used.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart v1.7.py](<../../../1/onchart v1.7.py>).

<a id="python-1-7-2"></a>

### 1.7.2 — Narrow blue layout and practical scaling

- Switches the accent palette from pink to blue/cyan and reduces the default window to 450×520.
- Makes scroll-container content follow the canvas width and adds mouse-wheel scrolling.
- Applies scale changes to individual label, entry, combobox and checkbox fonts as well as Tk scaling.
- Also removes decorative source comments; those edits are not additional product features.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v1.7.2.py](<../../../1/onchart_v1.7.2.py>).

<a id="python-1-8"></a>

### 1.8 — Rate conversion, patterns, hotkeys and terminal

- Adds a rate/BPM dialog with synchronized target fields and optional pitch-changing audio processing through FFmpeg.
- Rewrites note times, timing points and long-note ends for rate copies, with chained atempo filters for tempo-only processing beyond a single filter stage.
- Adds selectable pattern labels, Shift-based folder batching and Alt-based Dense labelling.
- Adds editable global keybindings, a terminal/log page, redirected output and a shared per-map packing helper.
- Rate copies in this initial implementation are written beside the source map; the destination changes in 1.8.2.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v1.8.py](<../../../1/onchart_v1.8.py>).

<a id="python-1-8-2"></a>

### 1.8.2 — Pack-oriented rate output and priority hotkeys

- Changes rate-copy output to the pack folder and simplifies rate-labelled filenames.
- Adds timestamped/coloured terminal output, Pretty Print switching and detailed map-change logging.
- Adds a priority keyboard listener alongside registered hotkeys, with parsed modifier combinations and debounce handling.
- Changes defaults to overwrite duplicates, force Various Artists and replace tags; adds control of tag replacement versus append behavior.
- Reworks FFmpeg filter selection and rate-dialog logging. Historical audio-copy fallbacks can leave unmodified audio when encoding fails; this is not described as a successful rate conversion.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v1.8.2.py](<../../../1/onchart_v1.8.2.py>).

<a id="python-1-8-7"></a>

### 1.8.7 — Complete assets and metadata for rate copies

- Copies and renames the background along with the rate-labelled audio, and rewrites the .osu background event to the exported filename.
- Applies pack title, Unicode title/artist, Various Artists and creator override choices to rate-generated maps.
- Keeps the rate-output metadata path aligned with ordinary pack generation.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v1.8.7.py](<../../../1/onchart_v1.8.7.py>).

<a id="python-1-8-11"></a>

### 1.8.11 — FFmpeg discovery

- Adds a cached FFmpeg resolver that searches PATH and common Windows installation folders.
- Rate generation uses the resolved executable instead of assuming the ffmpeg command is available globally.
- Explicitly handles an unavailable encoder through the historical original-audio fallback.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v1.8.11.py](<../../../1/onchart_v1.8.11.py>).

<a id="python-1-9"></a>

### 1.9 — Bundled-encoder fallback

- Adds an imageio-ffmpeg fallback when PATH/common-folder discovery fails, including a one-time pip installation attempt.
- Caches the located bundled executable and improves unavailable-encoder logging.
- Rewords the rate-processing implementation and documentation; the unchanged-audio fallback still exists in this snapshot.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v1.9.py](<../../../1/onchart_v1.9.py>).

<a id="python-1-9-3"></a>

### 1.9.3 — Modifier compatibility and audio-result checks

- Allows extra Shift/Alt modifiers as batch/Dense augmenters while requiring Ctrl/Windows modifier matches, reducing hotkey collisions.
- Tracks whether encoding actually succeeded and produced a file before treating the output as converted.
- Handles encoder errors and fallback-copy failures separately, clearing unusable audio references and reporting the selected output folder.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v1.9.3.py](<../../../1/onchart_v1.9.3.py>).

<a id="python-1-9-6"></a>

### 1.9.6 — Identical saved copy

- The archived source is byte-for-byte identical to 1.9.3 (verified by SHA-256).
- No additional implementation change can be assigned to this version label. It retains the 1.9.3 behavior.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v1.9.6.py](<../../../1/onchart_v1.9.6.py>).

<a id="python-2"></a>

### 2 — Slate/indigo interface refresh

- Introduces a new slate/indigo palette, cleaner notebook tabs, larger spacing, focus treatments and restyled scrollbars.
- Adds shared flat buttons with hover/press states and migrates the rate dialog, Pack Now and terminal actions to that helper.
- Adjusts header/status presentation and terminal typography while retaining the 1.9.6 packing/rate workflows.
- The saved filename is onchart_v2.py; no separate 2.0.0 filename or confirmed release record was found. This entry preserves the original v2 label.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.py](<../../../2/onchart_v2.py>).

<a id="python-2-0-1"></a>

### 2.0.1 — Dense-pattern labels retain their type

- Alt-prefixed packing and pattern hotkeys now form Dense plus the selected pattern instead of replacing every pattern with the bare word Dense.
- Removes the extra _bg suffix from rate-exported background filenames and simplifies the Override Tags label.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.0.1.py](<../../../2/onchart_v2.0.1.py>).

<a id="python-2-1-0"></a>

### 2.1.0 — Animated rounded visual system

- Adds canvas-drawn rounded buttons with interpolated hover/pressed colours and a configurable palette of surfaces and status colours.
- Redesigns the header, accent divider, button positioning and status strip, including a pulse animation.
- Updates terminal Pretty Print controls to work with the new button implementation.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.1.0.py](<../../../2/onchart_v2.1.0.py>).

<a id="python-2-1-1"></a>

### 2.1.1 — Rate-copy background section handling

- Rewrites background references using the tracked [Events] section instead of a separate state flag that could miss the event row.
- Preserves a valid line ending when replacing the background event, avoiding concatenated or malformed .osu rows.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.1.1.py](<../../../2/onchart_v2.1.1.py>).

<a id="python-2-1-2"></a>

### 2.1.2 — Windows frame styling

- Adds a Windows 11 dark-blue border colour through DWM attributes.
- Adds a matching narrow blue strip at the top of the client area; unsupported platform calls remain guarded.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.1.2.py](<../../../2/onchart_v2.1.2.py>).

<a id="python-2-1-3"></a>

### 2.1.3 — Section-aware BPM parsing and title-bar colours

- Limits BPM extraction during packing to [TimingPoints], preventing numeric rows from unrelated sections from being interpreted as timing points.
- Resets event-section tracking when entering other sections.
- Extends DWM styling to the title-bar background and contrasting caption text.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.1.3.py](<../../../2/onchart_v2.1.3.py>).

<a id="python-2-1-4"></a>

### 2.1.4 — Reliable Windows title-bar repaint

- Resolves the real top-level Tk window before applying DWM styling.
- Forces a non-client repaint and reapplies attributes on mapping and delayed startup callbacks, addressing attributes ignored before the window is realized.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.1.4.py](<../../../2/onchart_v2.1.4.py>).

<a id="python-2-1-5"></a>

### 2.1.5 — Rounded entries and draggable scrollbars

- Adds custom rounded text inputs with animated focus borders and a rounded scrollbar supporting drag and track clicks.
- Applies the new controls across forms, scrollable pages and the rate/BPM dialog.
- Preserves read-only entry presentation and connected scrollbar position updates.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.1.5.py](<../../../2/onchart_v2.1.5.py>).

<a id="python-2-1-6"></a>

### 2.1.6 — Single rate-dialog instance

- Tracks the active rate dialog so simultaneous registered-hotkey and priority-listener callbacks reuse and focus it instead of opening duplicates.
- Clears the stored dialog reference on close, allowing later reopening.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.1.6.py](<../../../2/onchart_v2.1.6.py>).

<a id="python-2-1-7"></a>

### 2.1.7 — Batch metadata override page

- Adds a Batch Edit tab with title, artist, creator, source and tags fields plus Clear All.
- Passes nonempty overrides into packing; explicit batch values take precedence over pack name, Various Artists and default creator/tag options.
- At this stage the overrides affect packed copies. Separate in-place batch editing arrives in 2.3.0.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.1.7.py](<../../../2/onchart_v2.1.7.py>).

<a id="python-2-2-1"></a>

### 2.2.1 — Explicit batch-pack action and branding

- Adds Override + Batch Pack to apply the configured overrides across the current map folder.
- Changes the expanded ONCHART name to Optimal Note Chart Heuristic Addition and Reduction Tool.
- Reduces notebook-tab font size to fit the growing navigation.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.2.1.py](<../../../2/onchart_v2.2.1.py>).

<a id="python-2-3-0"></a>

### 2.3.0 — Persistent settings and command editing

- Saves pack settings, keybindings, current pattern, UI scale and selected toggles to a JSON settings file; reloads them on startup.
- Introduces in-place batch editing of existing .osu files, separate from creating packed copies.
- Adds terminal read/write commands for metadata/difficulty fields, background/folder inspection, rate/BPM output and pattern-aware packing, with history navigation.
- Adds distinct Add to Pack and Add to Same Folder rate actions; the same-folder path retains the original map-set identity and background.
- Adds active-tab labels with icon-only inactive tabs, global wheel routing and debounced settings saving.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.3.0.py](<../../../2/onchart_v2.3.0.py>).

<a id="python-2-4-0"></a>

### 2.4.0 — Curated pack builder and inline console

- Adds a separate Create Pack window with a selected-song queue, background previews, remove controls, editable per-song rates and pack metadata.
- While that window is open, the pack hotkey queues the current map rather than immediately writing it.
- Builds queued maps through rated or unchanged-copy paths with completion/error logging.
- Reworks the terminal into a protected inline prompt with editable input/history while preserving earlier output when new logs arrive.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.4.0.py](<../../../2/onchart_v2.4.0.py>).

<a id="python-2-5-1"></a>

### 2.5.1 — tosu stable/lazer paths and OSZ export

- Accepts absolute as well as Songs-relative paths from tosu and tolerates missing metadata fields.
- Extends Songs discovery to lazer file-store candidates; this is early path-level support, not full content-addressed asset compatibility.
- Adds per-map OSZ export from the curated queue through temporary staging directories and collision-aware archive naming.
- Changes terminal streams to buffer complete lines with timestamps before inserting them into the GUI.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.5.1.py](<../../../2/onchart_v2.5.1.py>).

<a id="python-2-5-4"></a>

### 2.5.4 — Fresh batch targets and lazer safeguards

- Refreshes tosu information before in-place edits and reports missing charts, empty overrides and inaccessible folders explicitly.
- Detects content-hashed lazer storage and restricts that edit to the selected file rather than unrelated files beside it.
- Adds override/completion logging. The saved window version badge regresses to v2.1.0; the filename remains the historical version evidence.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.5.4.py](<../../../2/onchart_v2.5.4.py>).

<a id="python-2-5-5"></a>

### 2.5.5 — Hotkey deduplication and fresh rate input

- Adds a shared 300 ms debounce across both hotkey dispatch mechanisms to prevent duplicate queue additions and repeated actions.
- Refreshes the selected chart before rate generation so a dialog left open across map changes does not use stale paths.
- Changes the default Version format to the difficulty alone and removes the extra main-page OSZ action, keeping export with the curated pack builder.
- The older Difficulty Name Format constant is explicitly marked unused in the saved source; it should not be presented as a newly working control.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.5.5.py](<../../../2/onchart_v2.5.5.py>).

<a id="python-2-5-6"></a>

### 2.5.6 — Per-song pitch control attempt; broken snapshot

- Adds a Pitch checkbox to queued songs and forwards its state through normal pack generation and OSZ export.
- Extends rated-pack audio generation to choose resampling for pitch changes or atempo for tempo-only output.
- The retained file has an indentation error at line 1583. Python AST parsing fails, so these are intended changes in a non-runnable saved source snapshot, not a verified working release.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.5.6.py](<../../../2/onchart_v2.5.6.py>).

**Saved source status:** syntax error: expected an indented block after 'if' statement on line 1582, line 1583.

<a id="python-2-5-7"></a>

### 2.5.7 — Syntax repair and numeric difficulty bounds

- Removes the malformed duplicated pitch branch from 2.5.6, restoring syntactically valid source while retaining per-song pitch options.
- Validates terminal OD and HP changes as numeric values in the range 0–10.
- Syntax parsing passes; this audit did not run the legacy application or certify all workflows.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.5.7.py](<../../../2/onchart_v2.5.7.py>).

<a id="python-2-5-9"></a>

### 2.5.9 — Quiet Windows subprocesses

- Adds shared CREATE_NO_WINDOW/hidden-startup settings for Windows helper processes.
- Applies them to imageio-ffmpeg installation and the single-map/queued rate encoders to reduce console-window flashes.
- Later source snapshots revise some subprocess calls again; this entry describes this saved version rather than promising permanent retention.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.5.9.py](<../../../2/onchart_v2.5.9.py>).

<a id="python-2-6-1"></a>

### 2.6.1 — Background converter and filename-aware edits

- Adds a background conversion engine and UI with folder/current-song input, optional single image, output sizing, blur/vignette, fitted foreground, overlay scaling and black-and-white strength.
- Adds 13 overlay blend modes, chromatic aberration and the initial distortion implementation, with on-demand Pillow/NumPy dependency setup.
- Adds a preview panel, background worker, progress reporting and generation controls.
- Renames a .osu when its Version changes through terminal editing, keeping the loaded path synchronized.
- Some FFmpeg calls in this snapshot omit the earlier hidden-process arguments; the 2.5.9 console behavior should not be assumed for every descendant.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.6.1.py](<../../../2/onchart_v2.6.1.py>).

<a id="python-2-6-4"></a>

### 2.6.4 — Full-effects preview and coloured outlines

- Adds outline colour picking and separate outline blend-mode selection; outlines are no longer conditional on black-and-white mode.
- Expands the preview from an overlay-only display to the full background/foreground/overlay/effects composition.
- Fetches and caches a default preview background in the legacy implementation and regenerates preview output when effect settings change.
- Strengthens chromatic displacement and changes distortion from a radial warp to a horizontal sine-wave ripple.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.6.4.py](<../../../2/onchart_v2.6.4.py>).

<a id="python-2-6-11"></a>

### 2.6.11 — Identical saved copy

- The retained source is byte-for-byte identical to 2.6.4, confirmed by SHA-256.
- No additional implemented change is attributed to this version label.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.6.11.py](<../../../2/onchart_v2.6.11.py>).

<a id="python-2-6-14"></a>

### 2.6.14 — Deterministic banded glitch distortion

- Replaces the sine ripple with seeded horizontal bands shifted by random offsets, including occasional larger shifts.
- Uses a fixed random seed so repeated previews of the same settings are stable.
- Updates the displayed version badge to v2.6.14.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.6.14.py](<../../../2/onchart_v2.6.14.py>).

<a id="python-2-6-15"></a>

### 2.6.15 — Milder glitch distribution

- Uses taller bands, shifts only a fraction of them and limits maximum movement to roughly 6% of image width at full strength.
- Removes the occasional dramatic wide shifts from 2.6.14.
- The saved UI badge returns to v2.5.5; its filename identifies this snapshot as 2.6.15.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.6.15.py](<../../../2/onchart_v2.6.15.py>).

<a id="python-2-7-4"></a>

### 2.7.4 — Dense scanline distortion

- Changes distortion to thin 1–3-pixel bands across the whole image.
- Each band receives an offset bounded by strength, reaching approximately 8% of image width at full strength; the fixed random seed remains.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.7.4.py](<../../../2/onchart_v2.7.4.py>).

<a id="python-2-7-5"></a>

### 2.7.5 — Shared outline implementation

- Moves the outline helper out of the export-only nested scope into a shared function.
- The preview can now call the same glow/outline operation as conversion output rather than referencing an unavailable local helper.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.7.5.py](<../../../2/onchart_v2.7.5.py>).

<a id="python-2-7-6"></a>

### 2.7.6 — Pack manifests, rate precision and band thickness

- Adds numbered, timestamped Pack Info.txt entries with song/creator/difficulty/BPM/rate information for packed output.
- Raises synchronized rate/BPM display precision to six decimal places while trimming trailing zeroes.
- Adds an adjustable 1–500-pixel distortion-band thickness, used by both preview and conversion.
- Adds FFmpeg -vn and automatic thread selection to avoid processing embedded album art during audio conversion.
- Replaces the earlier explicit lazer batch-folder guard with .osu enumeration and a current-file fallback; this changes the historical safeguard and is not claimed as improved lazer compatibility.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.7.6.py](<../../../2/onchart_v2.7.6.py>).

<a id="python-2-7-9"></a>

### 2.7.9 — Generated-background references and replacement choice

- After generating backgrounds, updates matching .osu background references to the generated subfolder.
- Initially rewrites only references whose exact filename exists in the generated output and avoids adding the same prefix twice.
- Adds a Yes/No/Cancel choice to remove old output images, keep them with matching-name overwrites, or cancel generation.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.7.9.py](<../../../2/onchart_v2.7.9.py>).

<a id="python-2-7-10"></a>

### 2.7.10 — Unclipped outline margins

- Pads overlay canvases by the outline width plus blur margin before growing the alpha mask.
- Prevents glow/outline pixels from being cropped at the original image boundary.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.7.10.py](<../../../2/onchart_v2.7.10.py>).

<a id="python-2-7-11"></a>

### 2.7.11 — Case-insensitive background lookup

- Adds case-insensitive matching between .osu background names and generated images.
- Also changes reference rewriting to retain a target name even when no generated match exists. That can produce a reference to a missing file; the audit does not label that behavior a universally safe repair.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.7.11.py](<../../../2/onchart_v2.7.11.py>).

<a id="python-2-7-12"></a>

### 2.7.12 — Full LN / No LN mod attempt; broken snapshot

- Adds a Mods page with Full LN and No LN choices, a mania/key-count check and generation of separate suffixed .osu files.
- Full LN converts taps to holds based on the next note in the same lane; No LN removes hold endpoints and converts long notes to taps.
- Updates the exported difficulty name with the selected mod and logs the changed-note count.
- The saved file has an unexpected indentation at line 692 after removal of a try statement. It cannot be parsed as Python. The mod implementation is recorded as intended source work, not a verified working legacy release.
- Also contains extensive comment edits; those are not counted as separate features.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart_v2.7.12.py](<../../../2/onchart_v2.7.12.py>).

**Saved source status:** syntax error: unexpected indent, line 692.

## Modular Python 3.x history

<a id="python-3-0-0"></a>

### 3.0.0 — Modular PySide6 / Qt6 rewrite

- Replaces the single-file Tk interface with separate core, configuration, tosu, hotkey, command, analytics and Qt UI modules.
- Introduces Dashboard, Create Pack, Batch Editor, Rate Changer, Analytics, Terminal and Settings pages with collapsible navigation, themed cards, drag/drop targets and toast notifications.
- Adds interactive chart analytics for density/NPS, LN ratio, jacks, chords, streams, BPM/SV and a heatmap, with zoom/pan/hover and image/vector/document export controls.
- Adds a coloured command console with timestamps, search and autocomplete, plus optional trailing true/false scope on edit commands.
- Moves packing, audio processing and analytics work to background operations. This is the preserved implementation/design, not a fresh guarantee that every legacy I/O path is stall-free.
- Retains tosu v2 current-map following and global pack/rate/pattern hotkeys, with a fallback when the keyboard library is unavailable.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [README.md](<../../onchart_v3.0.0/onchart_v3/README.md>); [main.py](<../../onchart_v3.0.0/onchart_v3/main.py>).

<a id="python-3-0-9"></a>

### 3.0.9 — Blue themes, background converter and rate rounding

- Adds the modular background conversion engine and page, carrying forward overlay, blur, outline, blend, chromatic and scanline effects.
- Adds midnight/ocean/cobalt palettes and a user-selected accent, a top connection/map/pattern strip and scrollable page containers.
- Sizes the window relative to the display and adds animated page/sidebar transitions.
- Links Rate and Target BPM so editing either updates the other.
- Adds deterministic half-up millisecond quantization for rate-adjusted timing points, note heads and long-note ends.
- Adds Analytics auto-follow of tosu and blue-themed graph/heatmap colours. The saved README still says v3.0.0; the enclosing snapshot folder supplies the 3.0.9 identity.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [README.md](<../../onchart_v3.0.9/onchart_v3.0.0/README.md>); [main.py](<../../onchart_v3.0.9/onchart_v3.0.0/main.py>).

<a id="python-3-1-7"></a>

### 3.1.7 — MSD integration, queued packer and configurable paths

- Adds an MSD calculation module and Dashboard presentation with top-three skillsets. It probes an optional MinaCalc binding and otherwise computes a heuristic estimate; these early values must not all be described as original MinaCalc output.
- Adds a modular curated Packer page with selected-song rows, individual rates, removal, drag/drop and background generation of the chosen pack.
- Adds mapped icon loading, richer settings for UI scale and pack/installation/FFmpeg paths, and revised background-converter settings.
- Updates shared pack information handling and automatic UI sizing/scaling from the Python entry point.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [README.md](<../../onchart_v3.1.7/onchart_v3.1.7/README.md>); [main.py](<../../onchart_v3.1.7/onchart_v3.1.7/main.py>).

<a id="python-3-1-8"></a>

### 3.1.8 — Graphical MSD bars and packaging support

- Adds a dedicated coloured MSD bar-chart widget and uses it on the Dashboard.
- Adds an MSD overlay path to Analytics and revises background-converter persistence.
- Adds executable-building support and broader bundled-asset/icon discovery.
- The MSD engine module is unchanged from 3.1.7, including its optional binding and heuristic fallback.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [README.md](<../../onchart_v3.1.8/onchart_v3.1.8/README.md>); [main.py](<../../onchart_v3.1.8/onchart_v3.1.8/main.py>).

<a id="python-3-1-9"></a>

### 3.1.9 — Duplicate modular source snapshot

- The source modules, requirements and README in this folder match the preceding 3.1.8 snapshot by SHA-256.
- The nested folder and README still identify 3.1.8. No new source feature is attributed to the 3.1.9 outer-folder label.
- This comparison does not assert that all generated build or distribution files are identical; those are excluded from the source comparison.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [README.md](<../../onchart_v3.1.9/onchart_v3.1.8/README.md>); [main.py](<../../onchart_v3.1.9/onchart_v3.1.8/main.py>).

<a id="python-3-2-0"></a>

### 3.2.0 — Configurable MSD, rate presets and richer previews

- Extends MSD binding discovery to minacalc_rs/minacalc, normalizes returned skillset keys and identifies calculator versus heuristic results.
- Adds section-based MSD curves, using a compatible binding API when available and a heuristic section fallback otherwise.
- Adds per-skillset colour settings/reset controls and propagates theme changes to charts.
- Adds persisted rate presets with add, edit, delete, reset and context-menu controls.
- Improves background-preview selection, raw/converted preview display and detected installation/asset paths from the selected map.
- Revises bar rendering and executable asset/icon discovery.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [README.md](<../../onchart_v3.2.0/onchart_v3.2.0/README.md>); [main.py](<../../onchart_v3.2.0/onchart_v3.2.0/main.py>).

<a id="python-3-2-12"></a>

### 3.2.12 — Preserved Python beta and native migration workspace

- The saved Python tree adds converter and marathon modules/pages. Its converter advertises osu!mania, SM/SSC, Quaver, an Interlude-labelled ILC option and CSV; those historical claims are not a certificate of correct conversion to every named format.
- Archive distinction: the original onchart_v3.2.12.zip differs from the maintained workspace in eleven matching files and lacks eleven later account/marathon/test files. The later additions below describe the preserved workspace; they cannot all be assigned to the original ZIP.
- Adds marathon sequencing, per-map rates/cuts, same-key-count checks, silent breaks, output metadata, radial image composition and background generation work.
- Adds website account/license gating, asynchronous login, Windows DPAPI remembered credentials and owner/admin/user display roles.
- Adds Nunito/Lucide assets, rounded styling, eased scrolling, collapsible sidebar, opening/page transitions and low-end mode.
- Adds or revises seven-day beta expiry, windowed packaging, bundled FFmpeg discovery and isolated account/converter/marathon tests.
- The saved main.py also contains an entry-point block that obtains public-IP/location information and sends a Discord report. It was inspected statically and was not executed for this changelog; no destination credential is reproduced here.
- This workspace was updated in place during the native migration, so its present contents are cumulative and cannot establish one original publication date or the exact first release of every feature.
- The later native packages originally reused the 3.2.12/BETA branding before being retrospectively renumbered from 3.3.0.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [README.md](<../README.md>); [main.py](<../main.py>).

<a id="python-3-2-13"></a>

### 3.2.13 — Divergent Python snapshot with converter/packaging work

- This is a separate Python source tree, not the predecessor implied by the later native 3.13.x numbering. Its README still says 3.2.0 and configuration identifies 3.2.12 (BETA).
- Compared with the earlier 3.2.0 source, it includes the universal-converter page/model, revised rate handling and packaging logic that detects/excludes competing installed Qt bindings.
- Compared directly with the original archived 3.2.12, its matched source/document files differ only in build_exe.py and main.py; test.py is additional. This supports treating it as a continuation of that older snapshot rather than a deliberate removal of the later maintained workspace’s features.
- Compared with the currently maintained 3.2.12 Python workspace, it lacks the added account UI/login modules, marathon module/page, visual-effects helper and associated tests. The archive does not establish that these were intentionally removed from a released product.
- It retains legacy startup IP/location-to-Discord reporting in main.py and adds an auxiliary test.py importing browser_history and requests. Neither file was run, and no browser history or reporting destination was collected for this document.
- Treat its feature set and version metadata as a branch/snapshot discrepancy rather than inventing a clean sequential upgrade.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [README.md](<../../onchart_v3.2.13/README.md>); [main.py](<../../onchart_v3.2.13/main.py>).

## Parallel Windows C prototype

<a id="c-3-0-0"></a>

### 3.0.0 — Separate Win32 C prototype

- A separate source/c/onchart.c file identifies itself as the Windows C port, v3.0.0. It is a parallel prototype, not the PySide6 build or the later Qt C++ lineage.
- Its accompanying build guide describes tosu polling, a native dark map-information interface, Ctrl+P packing and detailed logs.
- Targets Windows SDK libraries through a Visual Studio command-line or project build. No compilation or runtime validation was performed for this changelog.

**Validation:** Static source review only; the historical application was not executed.

**Evidence:** [onchart.c](<../../../c/onchart.c>); [BUILD.md](<../../../c/BUILD.md>).

## Native Qt C++ history

<a id="native-3-3-0"></a>

### 3.3.0 — Renumbered native baseline

- Baseline of the modified-date renaming scheme. Earlier binaries/docs may still display 3.2.12 (BETA); renaming did not itself implement new features.
- The preserved Qt 6 C++ package uses original MinaCalc/yaml-cpp, bundled FFmpeg and a GUI executable; Python is not required for its runtime.
- Documents twelve tools: Dashboard, Create Pack, Packer, Batch Editor, Rate Changer, BG Converter, Converter, Analytics, Terminal, Settings, Mods and Marathon Maker (then beta).
- Baseline workflows include metadata-aware packing, per-song queue rates/pitch, rate copies, backed-up edits, Full LN/No LN, OSZ output and persistent presets.
- Includes native image effects: fitted overlays, blur/glow, chromatic/scanline distortion, black-and-white controls and 13 blend modes.
- Original MinaCalc rates 4K at a 93% target with eight skillsets; other counts are not silently rated. Density and BPM summaries follow the selected rate.
- Documents cross-format conversion and same-key-count mania marathons with clipped holds, silence and OGG/PNG assets. Game-specific scoring/storyboards/custom keysounds are not fully reproduced.
- Includes themes/accent choice, collapsible icon navigation, scrollable forms, scaling, low-end mode and portable dependencies.
- Evidence caveat: baseline docs are cumulative and mention later account/design work. Their presence does not prove every listed capability first appeared in 3.3.0.

**Validation:** The package carries historical 31-native/18-Python reports. These were not rerun. The later login package reports fewer checks, so counts are not a monotonic feature measure.

**Evidence:** [README.md](<dist/ONCHART_v3.3.0/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.3.0/docs/VERIFICATION.md>).

<a id="native-3-4-0"></a>

### 3.4.0 — Website login package

- Separately saves the native website-login build originally named ONCHART-website-login.
- Uses asynchronous HTTPS JSON login with strict ok=true and licensed=true approval. The website supplies role/display name; navigation, file tools and tosu remain locked before approval.
- Adds DPAPI-protected remembered credentials with online revalidation, damaged-record rejection and sign-out locking; no offline owner/license bypass.
- Retains the independent seven-day beta restriction. Initial production-route probing returned HTTP 404; later cumulative notes record the route returning Invalid login.

**Validation:** 26 native checks reported with a local contract-server fixture. A working real licensed production account was not verified by that probe.

**Evidence:** [README.md](<dist/ONCHART_v3.4.0-website-login/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.4.0-website-login/docs/VERIFICATION.md>).

<a id="native-3-5-0"></a>

### 3.5.0 — Analytics timeline, bulk rates and grouped navigation

- Adds independent note-head density, LN-head density and MSD-pattern layers, saved selections and a skillset selector.
- Calculates sixteen independent active-chart sections using original MinaCalc, with unavailable sparse sections and separate NPS/MSD axes.
- Normalizes chart identity across Windows case/slash/dot differences so repeated tosu polls preserve calculated MSD/history/timeline; different charts clear them.
- Synchronizes rate-history selection with the rate control, summary and charts. Rate-preset/remove pairs fill and wrap by available width.
- Adds Bulk Rate quick presets, custom min/max/step, 1.0x exclusion, name templates, linked OD/HP controls, destination choice and a 128-copy limit.
- Adds textured theme-aware native steppers/reorder arrows while retaining keyboard, repeat, limits and read-only behavior.
- Updates both gradient stops and related surfaces from the accent, including neutral-grey choices.
- Groups thirteen pages into General, Pack Tools, Mapping and Misc. with exclusive animated expansion, shortcut-aware navigation and compact icons.

**Validation:** Final packaged full/sidebar report: 38 checks. Intermediate section/persistence/preset/bulk/arrow reports describe stages of this same saved package.

**Evidence:** [README.md](<dist/ONCHART_v3.5.0-analytics/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.5.0-analytics/docs/VERIFICATION.md>).

<a id="native-3-5-1"></a>

### 3.5.1 — Continuous backgrounds and readable fields

- Makes layout containers transparent so the workspace gradient continues behind controls/presets.
- Reserves font-aware OD/HP text space and removes extra padding/borders from embedded editors.
- Removes stepper outlines while retaining textured feedback; narrow Rate Changer and themed Bulk Rate remain usable.

**Validation:** Eight focused checks include actual rate copies, wrapping, complete 10.0 text at three sizes and theme changes. Earlier 38-check evidence retained; portable startup passed.

**Evidence:** [README.md](<dist/ONCHART_v3.5.1-ui-fixes/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.5.1-ui-fixes/docs/VERIFICATION.md>).

<a id="native-3-5-2"></a>

### 3.5.2 — Rounded checkbox states

- Adds scale-aware rounded indicators with solid accent checked fill and explicit empty, hover, focus, disabled and partial states.
- Low-end mode retains those shapes without new animation.

**Validation:** Seven focused pixel/geometry, mouse/Space, state, gating and layout checks; portable startup documented.

**Evidence:** [README.md](<dist/ONCHART_v3.5.2-checkboxes/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.5.2-checkboxes/docs/VERIFICATION.md>).

<a id="native-3-6-0"></a>

### 3.6.0 — Shared skinned mania preview

- Adds Show map preview and Keep preview visible on every tab. A shared splitter places it beside wide pages or below narrow ones; hiding restores the page area.
- Adds skin-folder discovery/selection/reload and saved skin, visibility and scroll-speed preferences.
- Reads repeated Mania skin.ini sections by key count: columns/gaps/colours, hit positions, split stages, stage art, receptors and LN heads/bodies/tails.
- Supports custom paths, @2x sprites, animation frames and safe fallback art/settings.
- Adds play/pause, restart, seeking, holds, rate following and independent 50–3000 px/s scroll speed.
- This initial mania-focused preview is silent and does not implement game scoring, hitsounds, storyboards or lighting.

**Validation:** 42 full and six focused checks; synthetic skins/playback and thirteen-page wide/narrow layouts. Not a universal live-game/skin certification.

**Evidence:** [README.md](<dist/ONCHART_v3.6.0-preview/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.6.0-preview/docs/VERIFICATION.md>).

<a id="native-3-6-1"></a>

### 3.6.1 — Alignment, hold playback and renderer efficiency

- Aligns visible sprite edges, compensating for transparent padding, to HitPosition in both scroll directions.
- Lights receptors at note time, pins active hold heads to the line, removes holds at release and prevents bodies extending below the line.
- Supports stretch/two cascade styles, indexes active notes/holds, caches lanes and bounds scaled sprites to 16 MiB; cascades use texture fills.
- Uses absolute monotonic timing with fractional precision and reduces unnecessary transport/seek-control refresh.

**Validation:** 43 full and six focused checks. Archived rendering benchmarks are synthetic offscreen measurements, not live-game FPS claims.

**Evidence:** [README.md](<dist/ONCHART_v3.6.1-preview-fixed/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.6.1-preview-fixed/docs/VERIFICATION.md>).

<a id="native-3-6-2"></a>

### 3.6.2 — Rounded hold caps and per-hold animation

- Joins bodies behind rounded-head centres so leading edges remain visible; fixes tail attachment and double stage reversal.
- Honours independent tail flip settings. Body animation stays on frame one until hold start, then follows that hold’s elapsed time.

**Validation:** 44 full checks plus asymmetric-cap testing across styles/directions; selected actual skin/chart inspected read-only.

**Evidence:** [README.md](<dist/ONCHART_v3.6.2-hold-fix/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.6.2-hold-fix/docs/VERIFICATION.md>).

<a id="native-3-7-0"></a>

### 3.7.0 — Replay playback and MP4 export

- Adds persisted 0.5x–2.0x speed combined with map or recorded replay rate.
- Adds deterministic preview/replay MP4 export, synchronized pitch-preserving audio, resolution/FPS/range controls, progress and cancellation through FFmpeg.
- Adds native LZMA decoding of stable mania OSR inputs, exact beatmap-MD5 matching and input reconstruction.
- Reconstructs heads, releases/breaks, misses/combo and OD windows with speed/EZ/HR, ScoreV2 and mirror handling.
- Cancels stale replay exports on map change; failed/cancelled encoding preserves existing files and successful output commits atomically.
- At this stage combo/judgement overlays cannot be hidden. Extended lazer/Random/co-op/incompatible-key conversions are rejected; reconstruction is not a full historical scoring engine.

**Validation:** 46 full and five focused checks, plus actual H.264/AAC encode/decode for dimensions/FPS/duration/audio and overlay pixels.

**Evidence:** [README.md](<dist/ONCHART_v3.7.0-video-export/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.7.0-video-export/docs/VERIFICATION.md>).

<a id="native-3-7-1"></a>

### 3.7.1 — Tap visibility over hold tails

- Draws normal notes above hold bodies/heads/end caps so large tails cannot cover nearby taps.
- Uses identical layering in chart/replay/video rendering, both directions and all body styles.

**Validation:** 47 full and six focused checks, including pixel-exact tap-over-tail fixtures and prior hold/export regressions.

**Evidence:** [README.md](<dist/ONCHART_v3.7.1-note-layer-fix/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.7.1-note-layer-fix/docs/VERIFICATION.md>).

<a id="native-3-8-0"></a>

### 3.8.0 — Direct export settings dialog

- Export video opens settings directly, replacing the dropdown and later filename picker.
- Defaults to HD 1280×720, 60 FPS, whole map, Videos destination and a map-named MP4 without preview/replay suffixes.
- Combines filename/folder, preview/matching replay, HD/Full HD/portrait, FPS, range, audio and effective-speed review.
- Validates names/extensions and blocks submission after the map changes while the dialog is open.

**Validation:** 48 full and four focused checks, including decoding 1280×720/60 FPS output and the audio-disabled option.

**Evidence:** [README.md](<dist/ONCHART_v3.8.0-export-window/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.8.0-export-window/docs/VERIFICATION.md>).

<a id="native-3-9-0"></a>

### 3.9.0 — Detached preview and local replay chooser

- Adds Pop out/Pop back in using the same widget, retaining skin/replay/speed/position while freeing page space.
- Close/Escape docks it; tab changes keep it visible and initial bounds fit the screen.
- Adds background recursive scanning for exact-map-MD5 supported saved OSR files, with detected or selected replay folder.
- Lists player, score, combo, mods and filename; scans bounded headers before decompressing on load.
- Cancels stale scans/selections on refresh/close/map change. Does not query online scores or the score database.

**Validation:** 49 full checks with matching/subfolder/corrupt/unrelated replay fixtures, docking/layout and actual video encoding.

**Evidence:** [README.md](<dist/ONCHART_v3.9.0-preview-windows/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.9.0-preview-windows/docs/VERIFICATION.md>).

<a id="native-3-10-0"></a>

### 3.10.0 — Skin HUD, keystrokes and KPS graph

- Adds skin-font combo digits and configured judgement positions/artwork/animations, preserving custom paths, @2x dimensions and transparency.
- Adds optional grade totals, reconstructed accuracy, max combo and total judgements with backward seeking and no future-event leakage.
- Adds editable real/display keys, per-key totals/KPS/BPM, colours, sizes/gaps, highlights, motion and fading trails.
- Imports supported JKPS.cfg controls/colours; does not run JKPS or import its desktop settings, texture/font files or lifetime counts.
- Adds 1–300-second KPS graph history, bounded sampling, curve amount and colour, using playback seconds.
- Makes the preview vertically scrollable at full panel width when embedded, narrow or detached.
- Includes enabled recorded-input overlays in replay MP4s; ordinary chart exports do not invent keyboard recordings.

**Validation:** 53 full and eight focused checks, including skin-HUD pixels and decoded telemetry-overlay MP4.

**Evidence:** [README.md](<dist/ONCHART_v3.10.0-preview-telemetry/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.10.0-preview-telemetry/docs/VERIFICATION.md>).

<a id="native-3-10-1"></a>

### 3.10.1 — New account-site connection

- Moves native login and Account website to onchart-db.lovable.app.
- Retains strict licensed/ok approval, bounded requests/timeouts, redirect refusal, sign-out locking and beta expiry.
- Uses a separate remembered-login setting and encrypted records bound to the new site; old-site credentials are not reused.
- Native-only connection change; no Python endpoint migration or cloud chart/pack synchronization.

**Validation:** 54 full and six focused checks. Synthetic production POSTs return expected rejection responses; those probes do not verify a real licensed account.

**Evidence:** [README.md](<dist/ONCHART_v3.10.1-site-connection/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.10.1-site-connection/docs/VERIFICATION.md>).

<a id="native-3-10-2"></a>

### 3.10.2 — Exact rolling KPS and mania accuracy

- Queries the exact highest one-second KPS within the selected trailing window, including its left boundary, independently of sampled graph pixels.
- Indexes inputs for maximum queries, removes aged-out peaks, excludes future events and rebuilds rate-dependent indices on speed changes.
- Corrects ScoreV1/ScoreV2 accuracy weights, late boundaries, combined ScoreV1 holds and separate ScoreV2 head/tail judgements with release lenience.
- Separates body combo breaks from accuracy misses and prevents a tap-consumed press from recovering a later hold.
- Uses recorded OSR counts/max combo after the final possible judgement; rewinding restores reconstructed prefixes.
- Final recorded accuracy is authoritative; historical client tick differences can remain during reconstruction.

**Validation:** 57 full and eight focused checks across peaks, holds, formula boundaries, seeking, overlays and map gating.

**Evidence:** [README.md](<dist/ONCHART_v3.10.2-replay-accuracy/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.10.2-replay-accuracy/docs/VERIFICATION.md>).

<a id="native-3-11-0"></a>

### 3.11.0 — Local diagnostics and opt-in FDP

- Adds network-report preview, masked destination field, recipient review and manual sending.
- Adds FDP successful-login reporting, off by default and requiring reviewed opt-in plus a DPAPI-protected webhook.
- Documents selected public-IP/approximate IP-location data plus account name/ID; no password/GPS field.
- Changing destination/location disables prior consent. Disabling FDP removes the saved destination and cancels pending sends.
- Uses bounded HTTPS, disabled mentions and no retries/redirects. Does not enforce bans or identify ban evasion.
- Local-only diagnostics release; the functionality is removed in 3.11.1.

**Validation:** 57 application plus seven simulated-network diagnostic checks (64 total); no actual report/IP lookup is performed by those tests.

**Evidence:** [README.md](<dist/ONCHART_v3.11.0-local-diagnostics/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.11.0-local-diagnostics/docs/VERIFICATION.md>).

<a id="native-3-11-1"></a>

### 3.11.1 — Native release without expiry or FDP

- Removes the native FDP/diagnostics UI, reporting code and tests, discarding obsolete FDP settings.
- Removes beta expiry class/timer/build switch and expired-map clearing; discards the legacy first-run timestamp.
- Removes BETA wording from titles, opening screen, Marathon and generated metadata.
- Website account/license authorization remains required.
- Release/release-runtime folder and archive variants represent the same version, not extra feature versions.

**Validation:** 57 full checks. Thirty-day-old expiry settings no longer stop licensed polling; portable packaging/startup and dependencies checked.

**Evidence:** [README.md](<dist/ONCHART_v3.11.1-release/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.11.1-release/docs/VERIFICATION.md>).

<a id="native-3-11-2"></a>

### 3.11.2 — Passive input and bounded live history

- Uses passive Windows Raw Input and a shared message-only listener for live keyboard/mouse events.
- Captures short transitions without consuming another app’s keypress flags or changing its registrations.
- Retains physical state across hidden views/replays and clears stale held keys on session/power changes.
- Bounds live history to 601 seconds while retaining lifetime totals/peaks; full replay history and arbitrary seeking remain.
- Retains key/modifier/mouse, KPS, trails, graph and replay features.
- The user later identified this as previously working, but game-only controls also failed. Input/resource fixes do not establish a permanent osu! stack-overflow cure.

**Validation:** 74 historical cases: 57 application, eleven input and six telemetry, including real registration lifecycle and six-hour history simulation.

**Evidence:** [README.md](<dist/ONCHART_v3.11.2-stability/docs/README.md>); [VERIFICATION.md](<dist/ONCHART_v3.11.2-stability/docs/VERIFICATION.md>).

<a id="native-3-12-0"></a>

### 3.12.0 — Four-mode previews and expanded map processing

- Adds standard/taiko/catch preview renderers alongside mania, including standard slider curves and replay cursor/catcher movement.
- Adds independent combo/judgement switches, automatic playback and telemetry in available left-side preview space.
- Aligns KPS peaks/graph sampling during playback/seek; adds automatic MSD, graph samples-per-second and coloured pattern switches.
- Retains BPM/inherited velocity in parsing/preview scroll integration. Rate processing is intended to synchronize notes, BPM, audio and video; a CRLF export regression is later repaired in 3.14.5.
- Adds optional image/video export backgrounds with preview options preserved.
- Adds Inverse/No SV and marathon scroll normalization, retaining meaningful BPM changes without redundant points.
- Extends texture formats/animations and tail placement; adds navigation icons and WIP MugDiffusion/DanOverlay entries.
- Adds independent working copies of lazer content-addressed maps/assets plus extended replay/custom-speed metadata.
- Limits: original MSD remains 4K mania; four-mode reconstruction is not the full ruleset engine, and some slider ticks/droplets/special objects remain incomplete.

**Validation:** Release notes report 78 checks and portable startup. Dumps/private crash evidence excluded from packaging; no game-crash cure established.

**Evidence:** [RELEASE_3.12.0.md](<RELEASE_3.12.0.md>); [src](<dist/ONCHART_v3.12.0-source/src>).

<a id="native-3-13-0"></a>

### 3.13.0 — Linked MugDiffusion and DanOverlay extensions

- Adds a vertical Name/Description/Status/Link catalogue and folder-based linking with persisted menus in a new Extensions sidebar category.
- Unlinking removes the menu and controls only owned processes.
- MugDiffusion connects to its separately running service, discovers API inputs and sends audio, MSD/SR, patterns/style/LN, sampling, CFG, seed and snapping settings.
- Adds current-map filling, chart-to-prompt extraction, direct generation/OSZ result saving and original-interface access; disconnect leaves the external service running.
- DanOverlay can launch its app or analyze the current/selected chart from a source installation with ISOR/Legacy and selected rate, producing detailed results/manual JSON.
- Adds .onchart-venv source-runtime setup and Python selection. Executable-only Dan packages launch the overlay but do not supply source analysis.
- External repositories/weights/environments are separate; the supplied MugDiffusion model supports 4K VSRG.

**Validation:** 62 core, eleven input and six telemetry checks reported. Actual MugDiffusion generated a 73-note OSZ; actual Dan analysis and owned GUI start/stop passed.

**Evidence:** [RELEASE_3.13.0.md](<RELEASE_3.13.0.md>); [src](<dist/ONCHART_v3.13.0-source/src>).

<a id="native-3-13-2"></a>

### 3.13.2 — .osu generation templates

- Adds Use .osu as generation template with a picker when needed.
- Extracts MSD, map type, LN ratio and seven pattern/skillset preferences through the model’s extractor and enables their generation controls.
- Fills chart audio/title/artist; replacement audio can reuse extracted constraints on another song.
- Preserves sampling/steps/CFG/seed/snapping choices, disables uninferred SR/style constraints and reports range clamping.
- Rejects empty/unsupported charts without inventing settings. No saved 3.13.1 record was found; the gap is preserved.

**Validation:** Actual extraction/control application and generated OSZ passed; malformed/unsupported templates left controls unchanged.

**Evidence:** [RELEASE_3.13.2.md](<RELEASE_3.13.2.md>); [src](<dist/ONCHART_v3.13.2-source/src>).

<a id="native-3-13-3"></a>

### 3.13.3 — Automatic Dan and simpler AI inputs

- Recalculates Dan after source-runtime setup and on chart/rate/estimator changes.
- Shows Dan/DP/confidence plus SR/MSD on Dashboard and full metrics/skillsets in Analytics.
- Runs analysis in an owned process, waits for setup/jobs, rejects stale results and avoids repeated automatic JSON reports; manual reports remain.
- Adds Add audio or .osu template before/after MugDiffusion connection; queued input applies when API controls load.
- Uses audio-filename title defaults, missing-audio messages and all installed generation controls.
- Reduces action-button widths without removing options.

**Validation:** Actual Dan refresh/stale/disconnect/report checks and MugDiffusion generation with preselected audio/OSU passed; portable startup recorded.

**Evidence:** [RELEASE_3.13.3.md](<RELEASE_3.13.3.md>); [src](<dist/ONCHART_v3.13.3-source/src>).

<a id="native-3-13-4"></a>

### 3.13.4 — Built-in native osu! reader

- Makes the built-in reader the default while retaining tosu and Disabled options.
- Detects stable/lazer and routes selected maps through preview, analytics, MSD and Dan.
- Reads stable status, standard-mod rate, clock and available gameplay/results score/combo/judgements; omits stale song-select counters.
- Reads lazer map/asset hashes and clock, resolving content into an independent working cache.
- Uses native read/query access only, incremental background discovery, invalid/null-data handling, restart detection and Reconnect. No injected code or game-memory writes.
- Lazer layout snapshot 2026.1005.0 may require updates with future clients.

**Validation:** Selected-map stable reading passed at the time. Synthetic tests cover relocation, overlap, telemetry, map changes, corruption/nulls, exit and lazer assets. A running lazer client was not validated.

**Evidence:** [RELEASE_3.13.4.md](<RELEASE_3.13.4.md>); [src](<dist/ONCHART_v3.13.4-source/src>).

<a id="native-3-13-5"></a>

### 3.13.5 — Mode skins, taiko timing, catch movement and icon

- Loads standard/taiko/catch textures for approach circles, slider parts, big taiko/drumroll pieces and catcher/fruit overlays.
- Supports taiko subfolders, HD art and legacy animation names without irrelevant missing-Mania warnings.
- Aligns taiko centres to the marker at note time and clears autoplay notes on time.
- Moves the chart-preview catcher horizontally toward the next fruit/drop, including slider events; replay motion remains recorded.
- Places MugDiffusion actions beside inputs and sends the full ordered generation API request directly from OnChart.
- Embeds the supplied ONC! artwork as app/window icon and seven Windows icon sizes.

**Validation:** 64 core, four-mode synthetic/installed-skin, API-payload and actual generation checks recorded; icon and packaged startup passed.

**Evidence:** [RELEASE_3.13.5.md](<RELEASE_3.13.5.md>); [src](<dist/ONCHART_v3.13.5-source/src>).

<a id="native-3-13-6"></a>

### 3.13.6 — Multi-ladder clickable Dan card

- Places Dan beside the map background; click/focused Space cycles Reform, Celestial, Signicial, Shoegazer and LN.
- Saves the mode, switches cached values immediately and synchronizes Analytics.
- Combines ISOR Reform/Celestial with Legacy alternatives at the same rate, preserving per-mode engine provenance.
- Labels unsupported/non-LN results and omits missing DP/confidence rather than inventing zeroes.
- Uses UTF-8 in the Python bridge and identifies delegated LN/7K calculations as Legacy.

**Validation:** 66 core, four final focused and three actual Dan checks; an LN fixture at 1.25x produced an 8th Dan result. Layout and startup checks recorded.

**Evidence:** [RELEASE_3.13.6.md](<RELEASE_3.13.6.md>); [src](<dist/ONCHART_v3.13.6-source/src>).

<a id="native-3-14-0"></a>

### 3.14.0 — Initial Compact Mode saved build

- Adds Compact Mode beside Show map preview: hidden navigation, organized map list, slim supported-mania MSD, top-three frequent patterns and clickable Dan.
- Adds optional small preview/Open map, persists the toggle and restores full UI/geometry. Initial sizes: 740×650 with preview or 520×650 without; transport remains visible.
- Adds linked Dan rank palettes and Low/Low-mid/Mid/Mid-high/High bands, preferring returned sublevels and otherwise using DP fractions.
- Pattern abundance is frequency, not difficulty. Non-mania hides MSD; unsupported mania counts show the calculator restriction.
- This executable/folder/note exists but is absent from RELEASE_RENAME_INDEX.csv. It is an intermediate saved build, not an invented indexed/public release.

**Validation:** No independent completed final-suite result is assigned to this snapshot. The subsequent 3.14.1 notes describe final layout/packaging validation.

**Evidence:** [RELEASE_3.14.0.md](<RELEASE_3.14.0.md>).

<a id="native-3-14-1"></a>

### 3.14.1 — Compact visibility and portable Qt deployment

- Finalizes Compact Mode, Dan colours/sublevels and top-three pattern presentation.
- Constrains the preview canvas rather than the whole Dashboard so the Dan card and Open map stay visible.
- Clears compact MSD values after rate changes until recalculation completes.
- Verifies deployed Qt DLLs against installed originals, replacing damaged files even if deployment reports them current.

**Validation:** 68 core and seven preview checks; visible bounds, screenshots, actual Dan synchronization, system-only-PATH startup and 21 Qt library hashes passed.

**Evidence:** [RELEASE_3.14.1.md](<RELEASE_3.14.1.md>); [src](<dist/ONCHART_v3.14.1-source/src>).

<a id="native-3-14-2"></a>

### 3.14.2 — Shorter Compact Mode

- Groups MSD bars into 280 pixels rather than stretching across the panel, with a 76-pixel chart height.
- Tightens sections/Dan and places transport directly beneath the small preview.
- Default compact sizes become 740×560 with preview or 520×560 without, 90 pixels shorter; exiting restores the full window.

**Validation:** Four focused and seven preview checks, on/off screenshots, portable startup and 21 Qt hashes passed.

**Evidence:** [RELEASE_3.14.2.md](<RELEASE_3.14.2.md>); [src](<dist/ONCHART_v3.14.2-source/src>).

<a id="native-3-14-3"></a>

### 3.14.3 — Denser compact columns and preview

- Groups Dan/Open map in a small column beside map information and left of the preview.
- Reduces text/controls and bounds to 650×490 with preview or 460×490 without.
- Narrows preview and makes the canvas 260 pixels high.
- Groups thicker MSD bars into 240 pixels with smaller labels and smaller skillset-coloured values.

**Validation:** Six focused and seven preview checks, screenshots, actual Dan synchronization, startup and 21 Qt hashes passed. Later game crashes do not by themselves identify the UI update as the cause.

**Evidence:** [RELEASE_3.14.3.md](<RELEASE_3.14.3.md>); [src](<dist/ONCHART_v3.14.3-source/src>).

<a id="native-3-14-4"></a>

### 3.14.4 — Private-JIT scans and crash investigation

- Restricts stable discovery to private JIT memory, skipping DLL images/mapped files.
- Reuses reader state when focus returns to the same process; reduces scan slices and optional-signature retries after map discovery.
- Retains live maps/rates/clock/scores/lazer and adds a mapped-memory signature decoy regression.
- Investigation finds an update entry redirected into its caller and tens of thousands of recursive frames; game-only controls fail too, without establishing the rewrite owner.
- External compatibility/shortcut experiments are machine diagnostics, not product features. A successful mamesosu observation was later contradicted by fresh failures and is not a lasting cure.

**Validation:** 68 core, eleven input, six telemetry and six synthetic reader checks; startup/21 Qt hashes passed. Optional live probe skipped; a separate attempt failed before selected-map validation.

**Evidence:** [RELEASE_3.14.4.md](<RELEASE_3.14.4.md>); [src](<dist/ONCHART_v3.14.4-source/src>).

<a id="native-3-14-5"></a>

### 3.14.5 — Rate retiming, Dan output and MSD validation

- Fixes CRLF section recognition so metadata-preserving OSU export no longer replaces converted timing/objects with unscaled original rows.
- Single/bulk/pack uprates and downrates scale each BPM segment, timing offset, head/end, preview time and break with the audio.
- Retains inherited SV multipliers, slider geometry, samples and timing flags; source charts stay unchanged.
- Passes four-decimal Dan rates, accepts result markers followed by diagnostics and names manual reports for the map actually analyzed.
- Displays valid 7K tier/DP/sublevel output.
- Validates 4K mania/columns before calculator masks, widens timestamp subtraction and treats rejected-input zero vectors as unavailable; original 93%-goal MinaCalc and LN-head semantics remain.

**Validation:** 85 core, eight extension and twelve real Dan cases passed; all-mode LF/CRLF 0.75x/1.25x export/audio checks passed. Three unrelated optional checks skipped; startup/21 Qt hashes passed.

**Evidence:** [RELEASE_3.14.5.md](<RELEASE_3.14.5.md>); [src](<dist/ONCHART_v3.14.5-source/src>).

<a id="native-3-14-6"></a>

### 3.14.6 — Global scaling, density marker and local overlays

- Uses 0.01 wheel steps for rate-related inputs in Analytics, rate/converter, pack/bulk, Marathon and extensions; preview speed also steps 0.01x.
- Scales authored geometry, spacing/padding, fonts/rich text, icons, tables and custom graphs while retaining original values for reversible scaling.
- Compact Mode applies 65% automatically, restores prior scale/geometry and fits smaller Dan/preview content.
- Adds a density graph beside frequent patterns with a current-song marker.
- Hides compact Play/Restart and follows existing song-select/gameplay timestamps, interpolating samples and pausing on repeated times.
- Adds Browser/OBS default, Desktop or Both: loopback HTTP page/image/state plus an optional movable always-on-top window.
- Displays map/MSD/pattern/density/Dan and optional skin preview. Browser images refresh five times per second; desktop Dan/Open map remain interactive.
- Reuses existing reader data and keeps normal full-dashboard manual preview independent of overlay tracking.

**Validation:** 90 core, six preview and eight extension checks passed; four optional skipped. Clock checks use controlled payloads rather than a certified long gameplay run. Startup, 21 Qt hashes, screenshots and archive checks passed.

**Evidence:** [RELEASE_3.14.6.md](<RELEASE_3.14.6.md>); [src](<dist/ONCHART_v3.14.6-source/src>).

<a id="native-3-14-7"></a>

### 3.14.7 — Data-slot caching and readable-range checks

- Resolves stable code operands once and retains data-slot addresses for map/state/mod/clock/score snapshots; detaching resets the cache.
- Once signatures are found, polling no longer rereads their generated-code pages.
- Checks every requested range, including cross-region string tails, for committed readable memory; avoids guard/inaccessible/execute-only pages and excludes execute-only discovery regions.
- Does not modify game protections or eliminate every concurrent protection-change race.
- A regression that failed on the old reader now retains map switching/time/rate/combo after the fixture hides its own code pages.
- All OnChart features remain. The October 15 mamesosu test still crashed at 11:52:56 with stack overflow/callback 5f5, so this is a reader correction, not a validated game-crash fix.
- The proposed service comparison did not run because Windows reported the administrator request cancelled. No successful compatibility-service remedy was established.

**Validation:** Nine reader, eleven input, six telemetry and three UI checks passed (29 cases, including setup/cleanup where counted); one optional extra live probe skipped. Runtime/source CRC/SHA/source checks passed; game crash unresolved.

**Evidence:** [RELEASE_3.14.7.md](<RELEASE_3.14.7.md>); [src](<dist/ONCHART_v3.14.7-source/src>); [VERIFICATION.md](<VERIFICATION.md>); [memory-tests.txt](<qa/reader-3147/memory-tests.txt>); [ui-reader-test.txt](<qa/reader-3147/ui-reader-test.txt>).

<a id="native-3-15-0"></a>

### 3.15.0 — Compact keys, browser data rendering and independent difficulty

- Adds a small configured-key/KPS viewer beneath compact Dan controls using passive Raw Input; it also works with the map preview hidden.
- Replaces browser/OBS whole-window PNG polling with JSON state and local HTML/canvas rendering. Static map and skin data is revisioned; ordinary updates omit it. Skin textures are fetched separately.
- Keeps the desktop overlay, density position line, map information, skill bars and Dan display.
- Separates Analytics analysis rate from Rate Changer; automatic Dan estimates use the original map at 1.00x. Conversion-rate edits no longer trigger these estimates or change compact map BPM/duration.
- Uses fresh press edges in standard/taiko replays instead of treating already-held keys as fresh hits. Applies OD/HR/EZ judgement windows and rebuilds combo in event order.
- Keeps missing custom combo digits blank, fixing transparent combo skins that became visible at a missing 8. Bounds animation frame indexing for large/non-finite timestamps.
- Preserves read-only stable/lazer integration and existing feature set. Complete slider/spinner/roll/catch scoring parity and a permanent osu! crash repair are not claimed.
- Adds a project maintenance instruction to update changelogs for future changes.
- Accelerates initial lazer discovery with exact-byte searching, larger bounded chunks and short background slices between normal polls. Exposes search progress while retaining read-only/page-access checks.
- Catches Dan cache creation/write failures so an unwritable cache reports a message instead of terminating the application. Dan Current map also defaults to 1.00x.

**Validation:** Focused UI/difficulty checks and corrected automatic-Dan regression passed; real local Dan engine/export passed. Extension: 7 pass/4 optional skip; reader: 9 pass/1 optional skip; input: 11 pass; telemetry: 6 pass; preview: 9 pass/2 optional skip; selected-skin checks: 3 pass. Counts include setup/cleanup. Live lazer map/assets resolved in 19.899 seconds, followed by user-confirmed map switching, keys and responsiveness in 3.15.0. Browser data rendering and 21 Qt hashes/portable startup passed. Broader core run stopped after 49 passes/no failures; no full-suite or permanent stable-crash cure claimed.

**Evidence:** [RELEASE_3.15.0.md](<RELEASE_3.15.0.md>); [src](<dist/ONCHART_v3.15.0-source/src>).

<a id="native-3-15-1"></a>

### 3.15.1 — JKPS-style compact keystrokes at the bottom

- Uses the existing JKPS-style keystroke painter in Compact Mode, including saved colours, labels, press highlights, trails, counters and KPS/BPM options.
- Places the viewer across the bottom of the compact window beneath map information and the preview; it remains available with the preview hidden and hides in the full interface.
- Gives the desktop overlay the same footer. Browser/OBS draws matching styled keys and trails locally from bounded JSON telemetry and saved settings.
- Reserves compact footer space while preserving 65% UI scaling and normal-window restoration.

**Validation:** Focused compact layout, preview on/off, normal-window restoration, UI scaling, desktop/HTTP overlay and song-clock checks passed. Existing input and telemetry suites passed. Native screenshots were reviewed, and browser footer rendering was checked in the local browser. Portable startup and bundled Qt hashes passed. This visual update does not change the game reader or claim a new crash remedy.

**Evidence:** [RELEASE_3.15.1.md](<RELEASE_3.15.1.md>); [src](<dist/ONCHART_v3.15.1-source/src>).

<a id="native-3-16-0"></a>

### 3.16.0 — 4K sessions, skill memory, session planner and Bulk Rate presets

- Adds General > Sessions with local start/stop logs, per-map accuracy/rate/MSD, retry/result deduplication, replay import and manual results. Atomic journals and active-play checkpoints recover interrupted sessions as partial.
- Updates an eight-skill practice estimate after stopping and completing queued analysis. Uses relevant completed, unassisted 4K results at their actual played rate, independently of Rate Changer; the UI explains evidence counts and the accuracy-based heuristic.
- Adds an editable difficulty curve: right-click adds/removes points, dragging changes time/MSD and left-click cycles skillsets. The default curve follows updated memory; custom edits persist until From skill memory is chosen. Supports duration, Normal/Push/Acc/Fix presets and cancellable background indexing.
- Plans distinct original maps under the requested minutes, shows duration shortfall/target error, and exports numbered asset folders plus an order manifest under ONCHART Session [date]. Maps/audio/timing are preserved and missing audio/unsafe paths stop export.
- Supports ordinary/exported lazer .osu maps. The built-in lazer map/clock reader does not expose score judgements; automatic score learning needs compatible telemetry, with replay/manual entry available otherwise.
- Adds persistent add/apply/update/remove/restore controls for Bulk Rate presets, including range/step, OD/HP, pitch, base-rate exclusion and naming format. Existing default ranges remain available.

**Validation:** Session model/UI tests passed (12 cases including setup/cleanup): persistent learning, accuracy/pattern evidence, interruption recovery, corrupt journals, result deduplication/retries, planning budget/skill curve, actual MinaCalc/rate calculations, map/audio/background export and path containment, graph point editing/dragging, preset persistence, and queued stop/analysis. Focused application integration checks passed; screenshots were reviewed. Portable startup and 21 bundled Qt hashes passed. Live automatic session capture in a real game has not been user-confirmed. Built-in lazer score telemetry remains unavailable; use replay/manual results or a compatible score telemetry source. No new game-crash fix is claimed.

**Evidence:** [RELEASE_3.16.0.md](<RELEASE_3.16.0.md>); [src](<dist/ONCHART_v3.16.0-source/src>).

<a id="native-3-16-1"></a>

### 3.16.1 — Theme-aware session curves and four-game chart profiles

- Adds persistent osu!/Quaver/Etterna/Interlude selection in Settings, supplied per-game window/taskbar icons, a pink default Explorer icon, and a fixed-colour game name in the top-right ONCHART header independent of the theme.
- Planner curve, MSD label and Overall points now follow the theme accent. Skillset-specific point colours remain identifiable.
- Extends 4K session indexing/manual results and generic chart hashes to .qua/.sm/.ssc, distinguishes simfile difficulties, exports selected chart difficulties, and keeps separate session journals/skill memory per game. Game switching is blocked during active sessions or background work.
- Adds a manual simfile difficulty chooser with asset-complete working copies. Rates/bulk rates and packs retain multiple difficulties; native packs and marathon outputs follow the selected game. Generic LN/No LN/Inverse/No SV mods and backed-up native metadata/asset updates extend beyond osu!.
- Reads Interlude Songs/charts.db through a read-only SQLite connection, decodes bounded note/BPM/SV blobs and resolves linked/hashed audio/background assets into independent working .osu copies. Unsupported data and missing assets are reported.
- Preserves standard/normalized Quaver SVs, accepts omitted zero StartTime values and official numeric 4K/7K mode enums, and scales BPM/event/note/audio timing together. Complex scroll/timing cases that cannot be represented are rejected.
- Adds basic Quaver column PNG, Interlude noteskin-frame/config and Etterna PNG-grid texture adapters while retaining osu! skins. Lua actors, native HUD/shaders, fallback chains and several advanced skin effects remain unsupported.
- Routes DanOverlay and MugDiffusion prompt inputs through isolated .osu analysis copies for foreign charts. MugDiffusion outputs are converted in a background task to selected-game .qp/.zip archives while retaining the original .osz; errors mark incomplete conversion output.
- Adds a local telemetry JSON input with game/staleness checks and native non-osu accuracy requirements; other-game profiles do not attach the osu! reader. This does not bundle native producers for the other games. Automatic native live tracking and native non-osu replay decoding remain unfinished, so full four-game feature parity is explicitly not claimed.
- Updates the public website with a persistent Quaver blue → osu! pink → Interlude green → Etterna purple theme cycle, themed accents/glows/animated notes, and 3.16.1 feature and compatibility details. Website theme selection is independent of desktop game profiles.

**Validation:** Targeted suites passed: 12 game profile/format/theme/audio/native-import tests, 12 session tests, 9 UI integration checks, 10 pack/mod/marathon/rate workflow checks, 7 extension fixture checks (4 optional engine/live cases skipped), 9 preview checks (2 optional installed-osu-skin cases skipped), and 5 installed-library/skin checks; totals include setup/cleanup. Real-library samples: 95/100 Quaver files parsed (5 rejected for unsupported/invalid scroll data), 224 Etterna difficulties from 100 files (9 files rejected for unsupported stop/delay/warp timing), and 100/100 Interlude chart blobs decoded with the copied database unchanged. Ran 12 MinaCalc calculations per game, 12 native roundtrips per Quaver/Etterna, and loaded four note/receptor/hold columns from each tested native skin. Reviewed profile and planner screenshots. Portable startup with system-only PATH and 26 bundled Qt hashes passed. Fixture tests needing Qt cache/Python/PowerShell ran with local cache access. No real gameplay/native live/replay parity or new crash fix is claimed; other-game automatic providers/replays and advanced chart/skin features remain unfinished. Reports: qa/3161/. Website update: inline JavaScript syntax and theme cycling/persistence/storage-failure checks passed; desktop browser colour changes and reload persistence passed with no horizontal overflow at the tested viewport; mobile and production deployment verification remain pending. Website source saved to samcheck-rgb/onchart-site at c24f7988eac1c47d3f73a7897366a722b0fd2664.

**Evidence:** [RELEASE_3.16.1.md](<RELEASE_3.16.1.md>); [src](<dist/ONCHART_v3.16.1-source/src>).

<a id="native-3-16-2"></a>

### 3.16.2 — Structured terminal command workspace

- Adds a shared command registry with aliases, quoted Windows paths, positional and named arguments, strict finite-number/range/boolean/choice validation, duplicate/unknown argument errors and per-command examples. Both `help br` and `br --help` describe arguments and defaults.
- Bulk rate syntax: `br <start> <end> <gap> [include-base=true] [pitch=false] --output "folder"`. The 1.0x copy is included only when it lies on the chosen range grid. `--dry-run` reports the exact rates without changing settings or writing files. Real generation reuses the existing raw osu/audio/BPM/timing-preserving workflow and native chart routes.
- Adds session recording, stop/status/log/skills, library index/cancel, duration/preset/base planning, custom curve point editing, pack export and explicitly labelled manual result entry. Planning does not invent play results or change learned skill memory. Manual results must describe a real play; learning completes after the session stops.
- Adds map loading/info/asset updates/backed-up metadata editing, rate/BPM conversion, chart conversion, note modifiers, packing/archive export and explicit-rate MSD/statistics reports.
- Adds preview transport/seek/speed/skin/options, matching replay loading, video export, Compact Mode, local browser/window overlays, game profile/theme/scale, linked extension controls and MugDiffusion generation requests through the existing service pipeline.
- Adds marathon sequence/break/rate editing and generation, image conversion with current effects, and typed named-control discovery/read/write/action commands for less common settings and preset buttons. Private account/password controls are excluded; the terminal remains an application command interface and does not execute arbitrary shell code.
- Improves grouped help, contextual usage hints, Tab completion, F1 help, history/draft preservation, a command guide button and single-timestamp multiline reports. Pretty print uses theme-aware semantic colors, aligned tables and formatted JSON; output remains selectable/copyable.
- Previous `rate rate`, `rate bpm`, metadata shortcuts and positional pack syntax remain available. Mutating commands reject a busy main tool rather than silently queueing a different configuration.

**Validation:** Passed 24 terminal parser/control/pretty-print checks, 12 session checks, 8 application integration checks (including generated BPM/note/audio rate copies, backed-up metadata edits, session result learning/planning, preview controls, typed control access and marathon editing), and 7 extension fixture checks; counts include setup/cleanup. Four optional installed-engine/live extension cases were skipped. Reviewed terminal screenshots in dark/light themes at 65%, 100% and 150% scale. Portable system-only-PATH startup and 26 bundled Qt library hashes passed. Test fixtures use local Qt cache access and a local login-contract server. No new live-gameplay stability or unsupported format/reader parity is claimed. Reports: qa/3162/.

**Evidence:** [RELEASE_3.16.2.md](<RELEASE_3.16.2.md>); [src](<dist/ONCHART_v3.16.2-source/src>).

<a id="native-3-17-0"></a>

### 3.17.0 — Player Tools and complete MugDiffusion menus

- Adds Ctrl+K quick actions for pages, commands and recent maps. Commands open as editable drafts in Terminal.
- Adds a local notebook with favorites, tags, notes, practice goals/status, recent maps, timestamp bookmarks and JSON export/non-destructive merge.
- Adds A/B map-preview looping, dense-section jump points and a pausable practice/break timer. Preview tools do not control game playback or scores.
- Adds cancellable background map scanning/search with mode, keys, BPM, length, LN percentage, No SV and favorite filters. Shows possible matching note/timing copies without deleting anything.
- Adds reference-map metric comparison, missing audio/background/video inspection and map path/folder shortcuts.
- Adds player-tool terminal commands alongside the structured 3.16.2 command workspace.
- Expands MugDiffusion to six model-schema-driven menus: Audio, Difficulty, Rice & long notes, Special, Model configurations and Patterns. Optional gates, pattern/style choices, star/MSD prompts, LN controls, snap/mini-jack controls, sampling, CFG and seed are sent in service input order. Sliders and numeric fields stay synchronized.
- Displays returned generation overview images as thumbnails, with a larger viewer on double-click. Archive download and selected-game conversion continue independently of image availability.

**Validation:** Passed 7 Player Tools checks (metrics, asset inspection, notebook persistence/merge, search filters, preview looping and UI captures), 24 terminal checks, 8 whole-app integration checks and 7 extension fixture checks; totals include setup/cleanup. The extension fixture verifies every generation input, six menus, slider values and downloaded chart thumbnails. Four optional installed-engine/live extension cases were skipped. Reviewed Player Tools and MugDiffusion screenshots. Portable system-only-PATH startup and 26 bundled Qt hashes passed. No installed-model generation, live gameplay, new game crash repair or missing native reader/replay parity is claimed. Reports: qa/3170/. A subsequent review iteration addresses notebook validation, gallery freshness and library presentation in 3.17.1.

**Evidence:** [RELEASE_3.17.0.md](<RELEASE_3.17.0.md>); [src](<dist/ONCHART_v3.17.0-source/src>).

<a id="native-3-17-1"></a>

### 3.17.1 — Player Tools review and convenience fixes

- Validates notebook structure, field lengths, bookmark counts/times and recent-map limits on load/import. Rejected imports leave notes unchanged; unreadable originals stay untouched, with a visible recovery/export message.
- Disconnects only the Player Tools status-message signal during teardown, preserving Qt’s destroyed notification and theme-cache cleanup. Fixes the reproduced next-window theme crash caused by the review’s initial blanket disconnect.
- Keeps library scans marked active until their result is collected, and refreshes favorite/note filters after saving. Includes chart tags in discovery search.
- Includes spatial objects/hit sounds and scroll velocity in possible-copy matching, remembers the last scanned folder, and accepts the full supported unsigned 32-bit MugDiffusion seed range (plus -1 for random).
- Enforces notebook note/tag/goal limits at input, with a visible paste-limit message, so text is not silently shortened only when saved.
- Caches unchanged UI style conversions and reuses compiled expressions during scaling, reducing Compact Mode work without changing the selected scale.
- Gives title/artist columns the available library width and sizes numeric columns to their contents; density headings also fit their data. Exposes filter/timer controls by name for terminal access.
- Clears stale comparisons when switching maps and rejects bookmark commands without a loaded map or above the per-map limit.
- Protects the image gallery against delayed downloads from earlier results replacing newer thumbnails. Supports object captions and bounds decoded thumbnails to 1600 pixels per side.
- Gives model menus a useful minimum height, keeps number inputs compact and scrolls the result gallery into view when it appears.
- Adds an Open map preview shortcut to practice controls and lets explicit preview loops temporarily override automatic clock following, until disabled or a new map is loaded.
- Traverses dynamic widgets/layouts through weak pointers during UI scaling, so a child removed while geometry or styles change is skipped. Includes a destruction-during-scaling regression test. A new osu process crash fix is not claimed.
- Adds keyboard Up/Down navigation to Ctrl+K quick actions and verifies Player Tools navigation/palette integration under the application theme.

**Validation:** Final Release build succeeded. Player Tools: 12 passed; terminal: 24 passed; core UI integration: 8 passed; application/bulk-rate/MSD workflows: 5 passed; extensions: 7 passed and 4 optional installed-runtime checks skipped; preview: 9 passed and 2 optional checks skipped; game profiles: 12 passed; sessions: 12 passed. All completed suites have zero failures (Qt totals include setup/cleanup). The portable executable starts with system-only PATH, and all 26 deployed Qt libraries match the bundled SDK. Screenshots of practice, discovery, notebook, comparison and the themed application were reviewed; a local fixture verified all generation inputs, six model menus and result-image captions/thumbnails. Fresh generation with the installed model and live gameplay were not verified. Existing native reader/replay and advanced-format limitations remain in GAME_COMPATIBILITY.md; this release makes no new osu process crash-fix claim.

**Evidence:** [RELEASE_3.17.1.md](<RELEASE_3.17.1.md>); [src](<dist/ONCHART_v3.17.1-source/src>).

<a id="native-3-17-2"></a>

### 3.17.2 — Smoother scaling and compact MugDiffusion pattern rows

- Separates scale updates from full theme rebuilding: changing size retains existing icons, navigation, actions and control setup.
- Adds a synchronized scale slider beside the percentage input. Rapid wheel/slider changes are coalesced for 120 ms; releasing the slider applies the final value immediately. Typing a percentage commits on Enter or focus loss.
- Applies scale changes as a single paint transaction and cancels redundant queued layout passes. Avoids repeated geometry, stylesheet, rich-text and table-row writes when their values are unchanged. Compact-window fitting no longer rescales the entire widget tree each time it runs.
- Keeps text, spacing, icon sizes, control geometry and table dimensions tied to the chosen scale, including the 65% Compact Mode default. Size-only changes no longer reset theme-specific table/control setup.
- Groups each MugDiffusion pattern preference and its independently enabled MSD on one row. Uses compact More/Less buttons, style choice buttons, a slider and numeric MSD input. Related controls wrap into two lines at narrow widths.
- Preserves the service's field IDs, optional gates and API order, including chart prompting and generated image output. No generation settings or features were removed.

**Validation:** Release build succeeded. UI scale/layout regression: 6 passed, 0 failed; 61 rapid scale inputs coalesced to one apply in 857 ms (589 ms stylesheet, 33 ms geometry/layout). Player tools: 12 passed, 0 failed. Terminal: 24 passed, 0 failed. MugDiffusion/extensions: 7 passed, 0 failed; 4 optional installed-runtime checks skipped. Portable startup succeeded with system-only PATH; all 26 deployed Qt libraries match the bundled SDK. Wide and narrow pattern-menu screenshots and 65%/150% scale screenshots were generated and reviewed. Live osu! crash behavior and fresh external MugDiffusion/Dan runtimes were not verified; no osu! crash repair is claimed. Earlier release folders and archives remain preserved. Follow-up verification in 3.17.3 found the 3.17.2 scale captures were covered by the startup overlay. Their earlier visual-review claim is superseded by the authenticated settings-page captures and rendered-font assertions in 3.17.3.

**Evidence:** [RELEASE_3.17.2.md](<RELEASE_3.17.2.md>); [src](<dist/ONCHART_v3.17.2-source/src>).

<a id="native-3-17-3"></a>

### 3.17.3 — Uninterrupted scale dragging and visual verification

- Keeps the scale slider responsive while its handle is held, including pauses longer than the debounce interval. Releasing the handle applies the final size once. Pressing the handle cancels a previously pending wheel update.
- Retains the 120 ms coalescing for wheel and percentage changes, synchronized inputs, and the compact MugDiffusion pattern/MSD rows introduced in 3.17.2.
- Allows the Sessions status summary to wrap, keeping the page usable in narrow windows instead of forcing horizontal scrolling.
- Strengthens UI regression coverage with actual rendered font sizes, 65%/140%/150%/100% scale checks, authenticated fixture settings-page captures, and theme assertions scoped to the main window.
- Corrects the earlier screenshot-validation claim: the 3.17.2 scale captures showed the startup overlay, not the settings controls. New captures replace that evidence; existing release archives are preserved.
- Repairs the historical 3.11.2 archive index to its current filename, ONCHART_v3.11.2.zip, after confirming its SHA-256 matches the original recorded archive. No historical ZIP was recreated or modified.

**Validation:** Release build and focused UI regression passed: a pending scale update is cancelled on slider press, holding/pausing the handle does not apply scaling, release applies once, and rendered control fonts plus stylesheet sizes agree at 65%, 140%, 150% and 100%. Layout, Compact Mode, game-profile, theme-gradient, terminal and MSD UI checks passed. Fresh fixture extension and terminal suites passed; optional installed MugDiffusion/Dan runtime checks were skipped. Portable startup succeeds with system-only PATH; all 26 deployed Qt libraries match the SDK. Settings-page captures at 65% and 150% were reviewed with the startup overlay hidden. Stylesheet application still runs synchronously on release; this avoids interruptions during the drag but does not promise an instantaneous final resize. Live gameplay and fresh external model generation were not verified.

- integration-tests.txt: Totals: 12 passed, 0 failed, 0 skipped, 0 blacklisted, 45186ms
- extension-tests.txt: Totals: 7 passed, 0 failed, 4 skipped, 0 blacklisted, 4079ms
- terminal-tests.txt: Totals: 24 passed, 0 failed, 0 skipped, 0 blacklisted, 149ms

**Evidence:** [RELEASE_3.17.3.md](<RELEASE_3.17.3.md>); [src](<dist/ONCHART_v3.17.3-source/src>).

<a id="native-3-18-0"></a>

### 3.18.0 — Natural voice and chat assistant, selected-game loaders

- Adds a configurable OpenAI-compatible AI gateway in Settings with an encrypted Windows-user API key, explicit model ID, connection test, and optional API speech model/voice.
- Adds dashboard chat access and Ctrl+Shift+A, visible actions/results, conversation reset, Stop, and optional spoken replies. Natural AI voice is the default, with male/female presets, editable voice IDs, conversational delivery and voice preview; local Windows voice is an explicit fallback.
- Adds local Windows wake recognition gated by “Hey OnChart” and direct one-shot microphone capture. Command audio is transcribed through the gateway with game-vocabulary hints, optional language selection, and optional transcript review. Recording stops after a pause or 15 seconds; silence is not uploaded. Listening starts only when explicitly enabled and pauses during assistant processing/playback.
- Routes AI actions through the validated app command registry for rate/bulk rate, marathon, Dan/MSD, map/metadata tools, sessions, preview, extensions, images, Player Tools and named UI controls. Excludes private/account and assistant configuration controls.
- Returns actual app logs, background-job completion and extension Dan output to the model. Bounds tool steps, context and response sizes; cancels stale replies and avoids automatic retries that could duplicate work.
- Makes forms wrap long rows at narrow widths, gives the new settings page scrolling, and retains a keyboard shortcut for compact layouts.
- Continues the selected-game loader work: shared library paths and chart filters, game-specific Player Tools/session scanning, and read-only Interlude imports into a cached working library. Shared chart pickers cover dashboard, converter, Player Tools and extension map/template inputs.

**Validation:** Release build and portable system-only-PATH startup passed. All deployed Qt libraries match the SDK. Assistant fixtures verify tool completion feedback, command validation, wake text gating, cancellation, step limits, encrypted key storage, multipart audio transcription, optional transcript review, transcription-to-chat routing, and natural male/female voice request payloads. App integration exercises real MinaCalc through the assistant and checks command workflows, narrow layouts, Compact Mode, game profiles and scaling. Game-format, session, Player Tools, terminal and extension fixtures passed; four optional installed-engine tests were skipped. Initial sandboxed format/extension failures came from blocked Qt cache access and passed with normal cache access. Windows fallback speech, local wake-helper microphone initialization, and direct recorder initialization/silence handling passed. No microphone recording or transcript was saved by voice QA. Authenticated themed assistant/settings screenshots were reviewed. No commercial gateway call, natural voice listening test, end-to-end spoken conversation, fresh external model generation or live gameplay crash repair is claimed.

- assistant-tests.txt: Totals: 12 passed, 0 failed, 0 skipped, 0 blacklisted, 1867ms
- integration-tests.txt: Totals: 10 passed, 0 failed, 0 skipped, 0 blacklisted, 27343ms
- game-profile-tests.txt: Totals: 13 passed, 0 failed, 0 skipped, 0 blacklisted, 22048ms
- terminal-tests.txt: Totals: 24 passed, 0 failed, 0 skipped, 0 blacklisted, 251ms
- player-tests.txt: Totals: 12 passed, 0 failed, 0 skipped, 0 blacklisted, 2714ms
- session-tests.txt: Totals: 12 passed, 0 failed, 0 skipped, 0 blacklisted, 1612ms
- extension-tests.txt: Totals: 7 passed, 0 failed, 4 skipped, 0 blacklisted, 3609ms

**Evidence:** [RELEASE_3.18.0.md](<RELEASE_3.18.0.md>); [src](<dist/ONCHART_v3.18.0-source/src>).

<a id="native-3-18-1"></a>

### 3.18.1 — Safer osu! polling and concise assistant replies

- Limits automatic osu! memory discovery to two bounded slices per 100 ms and pauses discovery and snapshot reads while osu! is not foreground; live map detection resumes when focused.
- Adds a main-patterns command that returns exactly the two most common pattern names without percentages or counts.
- Formats assistant Dan results using the currently selected scale and returns only the band and Dan label.
- Retains recent conversation context so short follow-ups such as “what MSD?” reuse the current map; overall MSD is the default unless a skill is named.
- Uses a compact command reference in AI requests to reduce repeated prompt content while preserving the available controls.
- Preserves natural male/female AI voice and speech transcription support from 3.18.0.

**Validation:** Release build and portable system-only-PATH startup passed; all 26 deployed Qt libraries match Qt 6.8.3. Assistant tests passed 13/13, terminal tests 24/24, core integration checks 4/4, and synthetic stable/lazer reader checks 9/9; the optional real-game memory probe was skipped. The assistant regression verifies the main-patterns tool call followed by “what MSD?” retains the prior answer and runs analysis on the current map. The terminal integration verifies the main-patterns response contains two names without percentages or counts. Windows Error Reporting recorded osu! stable 1.3.3.7 with System.StackOverflowException (0xc00000fd) on 2026-10-17 and the same exception type on 2026-10-15. These reports do not attribute the crash to OnChart. Live gameplay was unavailable, so no confirmed crash repair is claimed.

**Evidence:** [RELEASE_3.18.1.md](<RELEASE_3.18.1.md>); [src](<dist/ONCHART_v3.18.1-source/src>).

<a id="native-3-18-2"></a>

### 3.18.2 — Local voice control and map-folder rate outputs

- Transcribes Talk once and wake-triggered commands locally with the installed Windows speech recognizer; command audio is no longer uploaded for transcription.
- Starts Hey OnChart listening by default and keeps the assistant chat hidden after wake activation. Listening remains available while the chat is closed and can be stopped in the assistant.
- Keeps natural male and female AI reply voices with Nova and Onyx presets and conversational speech playback.
- Saves assistant-created rate copies beside the loaded map unless an output folder is explicitly provided.
- Continues bounded, focus-aware osu! polling. New Windows Error Reporting records still show osu! stable stack overflow; no causal link to OnChart or confirmed live crash repair is established.
- Reviewed Discord-TTS/Bot: it is a Rust Discord voice bot requiring Discord hosting and cloud voice credentials, so it cannot serve as an in-process Windows playback engine.

**Validation:** Release application build passed. Assistant tests passed 13/13, terminal command tests 24/24, synthetic memory-reader tests 9/9 with the optional live-game probe skipped, live-input tests 11/11, and four focused core integration cases passed; the added rate-output integration verified a rate copy beside the loaded map. A Windows no-speech probe exercised the local transcription helper and made zero gateway requests. Windows lists an en-US recognizer, but the local System.Speech engine failed to instantiate it (No recognizer of the required ID found), so recognition of spoken words remains unverified on this machine. osu! WER records show exception 0xc00000fd (stack overflow), but identify no faulting module or cause. Live gameplay verification was unavailable; no osu! crash repair is claimed.

**Evidence:** [RELEASE_3.18.2.md](<RELEASE_3.18.2.md>); [src](<dist/ONCHART_v3.18.2-source/src>).

<a id="native-3-18-4"></a>

### 3.18.4 — Offline voice recognition and safer osu! isolation

- Replaces the failing Windows speech recognizer dependency with local whisper.cpp base.en recognition for Talk once and Hey OnChart wake detection. The bundled model runs offline; temporary recordings are deleted after recognition.
- Plays a short system ready tone when Hey OnChart is recognized. A wake command keeps the assistant chat closed unless transcript review is enabled.
- Keeps natural male and female AI reply voice presets through the configured speech gateway. Reviewed Discord-TTS/Bot: it is a Discord client using cloud Polly or Google credentials, so its audio playback stack does not fit in-process Windows speech.
- Disables OnChart's osu! memory reader by default and migrates a previously stored built-in-reader selection to Disabled once on upgrade; users can select tosu, local telemetry or explicitly re-enable built-in reading. Latest WER evidence reports an access violation in osu!auth.dll after earlier stack overflows; the archived report has no call stack, so the migration is an isolation safeguard and not a confirmed osu! crash repair.
- Ships only essential current-use documents in the runtime package; historical release notes and research remain in the source package.

**Validation:** The Windows release build passed. The bundled whisper.cpp v1.9.5 base.en model correctly transcribed the official JFK sample through the local helper, deleted temporary audio and made zero gateway requests. The packaged app starts with only Windows system PATH; all 26 packaged Qt libraries match Qt 6.8.3. Assistant tests passed, and the focused reader-default/migration regression passed. The complete CTest run did not pass: extension and game-profile suites could not write their Qt test cache under the user profile, and the broad native suite ended in a segmentation fault after 88 seconds while exercising builtInReaderSourceControls. These results are retained in QA evidence rather than reported as green. Runtime and source ZIP integrity checks passed. The latest archived osu! stable WER report identifies osu!auth.dll but its dump is no longer available; live post-change gameplay verification is still required, so no osu! crash repair is claimed.

**Evidence:** [RELEASE_3.18.4.md](<RELEASE_3.18.4.md>); [src](<dist/ONCHART_v3.18.4-source/src>).

<a id="native-3-18-5"></a>

### 3.18.5 — Discord-TTS reply speech service

- Replaces chat-gateway speech and Windows SAPI reply playback with the HTTP speech service used by Discord-TTS/Bot. OnChart decodes service audio with bundled FFmpeg.
- Adds service URL, optional encrypted service key, provider, voice and rate settings, with Polly and Google Cloud male/female presets and editable voice ID.
- Preserves local Whisper wake detection and transcription, concise chart replies, map-folder output defaults, and the 3.18.4 osu! reader isolation.

**Validation:** Windows release build passed. Synthetic WAV and Ogg/Opus samples played through the packaged helper, with Ogg decoded by bundled FFmpeg. The assistant service-request regression compiled, but Qt test executables stalled before output on this machine, including an unrelated Qt test executable; no passing end-to-end request test is claimed. Live Polly/Google Cloud playback needs a configured service and provider credentials. Live osu! gameplay was not verified, so the earlier crash isolation is not a confirmed repair. Runtime/source ZIP integrity and prior-release preservation were checked separately.

**Evidence:** [RELEASE_3.18.5.md](<RELEASE_3.18.5.md>); [src](<dist/ONCHART_v3.18.5-source/src>).

<a id="native-3-18-6"></a>

### 3.18.6 — Microphone setup, local speech detection and current-map recovery

- Adds microphone selection/refresh, software input gain, adjustable speech threshold and a local recording/transcription test in Settings. The test displays recognized words without executing commands or uploading audio; chat and settings show live input levels and clipping warnings.
- Runs local voice helpers from extracted files rather than embedding their source in the Windows process command line. Extends offline recognition timeout from 20 to 90 seconds for slower or busy CPUs and ignores intentionally cancelled recognizer exits.
- Bundles checksum-verified Silero v6.2.0 speech detection with Whisper base.en to reject silence and quiet noise before recognition. Adds an audible two-note recording-ready sound and recognition vocabulary hints.
- Adds saved personal assistant instructions for playing goals, terminology and coaching preferences while preserving concise selected-scale Dan replies, two-pattern answers, follow-up context, command validation and map-folder outputs.
- Rediscovers invalid stable map roots using bounded scans, rejects responses from an old reader generation and marks unavailable live maps as stale in assistant context. The built-in reader remains focus-aware and disabled by default; historical release folders and archives remain preserved.

**Validation:** Windows release build passed. Assistant suite: 15 passed, 0 failed, with the opt-in live-microphone case skipped in the automated run. Synthetic memory suite: 9 passed, 0 failed, live-game probe skipped. Native reader UI checks passed after the fixture explicitly opted into the reader: the displayed chart changed to a second synthetic map, missing data was marked stale, and reading recovered; reader source/migration controls also passed. The assistant command/account-protection integration passed separately. Whisper plus Silero correctly transcribed the official JFK sample and rejected silence and quiet noise, without audio uploads. Actual Conexant microphone capture and local transcription worked with no clipping, but the live phrase misheard main as them in; exact spoken-word accuracy is not claimed. An early no-speech live test produced spurious text before VAD was added; early reader UI failures came from the fixture not setting the existing migration marker correctly. The packaged application starts with only Windows system PATH, all 26 Qt libraries match the installed SDK, and the packaged recognizer/detector transcribes locally. Full CTest and live osu! gameplay were not run for this release; no confirmed osu! crash repair is claimed. Runtime/source ZIP integrity and preservation of earlier archives are checked by the package verifier.

**Evidence:** [RELEASE_3.18.6.md](<RELEASE_3.18.6.md>); [src](<dist/ONCHART_v3.18.6-source/src>).

<a id="native-3-18-7"></a>

### 3.18.7 — Local voice memory and Dan-target rate copies

- Full LN resizes taps and existing holds to half the gap to the next same-column note; terminal notes use a 250 ms fallback. Other LN modifiers keep their existing behavior.
- Adds automatic local voice memory with ten-example caps per listed main command, progress counts, pause and delete controls. Audio-derived acoustic matching and vocabulary hints help the recognizer; saved numbers, modes and editing actions are not replayed as current commands. Reviewed transcripts can supply corrected labels after successful actions. Samples stay in user-local data and are excluded from release packages; Whisper weights are not retrained.
- Discards buffered recognition output after Stop or voice-memory deletion so cancelled speech cannot become a command.
- Adds Dan mode query overrides and persistent mode switching for Reform, Celestial, Signicial, Shoegazer and LN through validated dan/danmode commands and assistant instructions.
- Adds danrate for targets such as 4th, Delta or low Alpha. It measures real DP with the linked engine and checks 0.01 rate steps in the needed direction, creating a pitch-preserved copy beside the captured source only when the target tier/band is reached. Difficulty names contain only the actual rate; osu metadata/events and original files are preserved. Search is bounded and reports failure instead of inventing a match.
- Automatically rediscovers running clients every two seconds: the foreground supported osu client wins, otherwise lazer is preferred. Existing read-only, focus-aware and bounded memory scanning remains, with built-in reading disabled by default for crash isolation.

**Validation:** The Windows release build passed. Final native verification passed: assistant: 17 passed, 1 skipped; memory: 10 passed, 1 skipped; extension: 9 passed, 4 skipped; terminal: 24 passed, 0 skipped; core: 8 passed, 0 skipped. Eight deterministic target-search tests passed. Real DanOverlay checks passed for Reform, Celestial, Signicial and Shoegazer; real legacy Rice and ISOR LN searches each checked 12 rates before reaching a different requested band at 1.11x. The native export test encoded real audio at 0.99x, verified the rate-only difficulty name, timing/BPM scaling, retained custom map sections, and unchanged source. Native integration verified a target-Dan copy and persistent Dan-mode selection. Voice-memory checks covered ten-example caps, deletion, gain-tolerant acoustic hints, and exclusion of stored numeric rates from hints/corrections. The packaged application starts with only Windows system PATH; 26 Qt libraries match the SDK and bundled Whisper/Silero recognition passed. Early fixture startup timeouts under compiler load and asynchronous test assertions were corrected/retested; final results are recorded separately from those earlier failures. Full CTest, actual-user personalized recognition accuracy, real lazer client switching and live osu! gameplay/crash freedom were not verified. No confirmed osu! crash repair is claimed.

**Evidence:** [RELEASE_3.18.7.md](<RELEASE_3.18.7.md>); [src](<dist/ONCHART_v3.18.7-source/src>).

<a id="native-3-18-8"></a>

### 3.18.8 — Training storage, new converters and persistent skinning

- Adds automatic local training records for accepted assistant inputs, spoken prompt WAVs, replies, observable processing steps, actions, results and errors. Session/turn IDs link records. Authenticated uploads to the existing voice-service URL require a matching persistence acknowledgement; failed/interrupted uploads remain queued. Settings exposes upload pause, status, local folder and local deletion. Records do not contain saved API keys or private model reasoning and do not automatically fine-tune a model.
- Adds persistent authenticated Cloudflare KV training storage to the existing speech Worker, with bounded ingestion, paginated export and individual read/delete routes. The previous speech route, AI binding and encrypted service-key configuration are preserved. Local training data and voice memory are excluded from packages.
- Adds ADOFAI file/ZIP to mania conversion with 2–18 keys and configurable minimum stream spacing. Retained beats keep timing, dense subdivisions are omitted, and lanes rotate without consecutive jacks. Handles path/angle data, BPM/multiplier changes, twirls, midspins, pauses, holds and two/three planets. Unsupported timing and missing audio fail explicitly. ZIP traversal and expansion are bounded.
- Adds Rhythia SSPM v1/v2 to osu standard conversion with embedded audio/cover extraction and a 16–160 px circle-grid spacing slider. Quantum coordinates are supported within playfield bounds. The supplied legacy SSPM is covered by native verification.
- Adds mania/Quaver/Etterna keyboard-texture conversion, destination configuration and separate output folders. Notes, holds and receptors transfer; animation uses the first frame. Arbitrary Lua choreography, shaders, menus and destination-specific HUD cannot be translated and use destination defaults.
- Adds a persistent Skinning tab under Mapping with Standard, Mania, Taiko, Catch, Evaluation, Song selection, Pause and HUD texture sections. Selected images are copied into a user-local workspace. Gameplay animates and menus show layout previews. OSK installs the skin; OSZ exports a playable silent demonstration map with the textures.
- Makes the bounded read-only stable/lazer reader the default, including migration from earlier crash-isolation Disabled settings. Existing tosu/local-telemetry selections and subsequent manual changes persist. Shared other-game preview, pack, background, rate and marathon workflows remain available; other games still require manual chart selection or telemetry for live data.
- Handles an unwritable skin workspace during startup with a visible error and disabled saving, allowing the rest of the application to remain available instead of propagating a file exception.
- Builds shared window objects once for the application and verification executable, keeping their UI implementation consistent.

**Validation:** Final Windows release build and portable/offline speech checks passed. Native suites: conversion: 9 passed, 0 skipped; assistant: 17 passed, 1 skipped; game_profile: 13 passed, 0 skipped; preview_mode: 9 passed, 2 skipped; memory: 10 passed, 1 skipped; core: 11 passed, 0 skipped. Native conversion checks include the user-supplied SSPM, ADOFAI and ZIP conversion, stream timing/lane constraints, keyboard skin round-trips, persistent texture reopening, OSK/OSZ extraction, durable upload acknowledgements and deletion, and real-audio marathon/background output across osu, Quaver, SM and SSC. Skinning screens were visually checked with the native Windows font renderer. Eight Worker route checks passed. Live authenticated training storage write/read/export/deletion passed and unauthenticated export was rejected. Earlier intermediate compile failures, restricted-cache test failures and an early mixed-build queue-test crash are retained in QA logs; final results supersede them. Cloudflare AI speech requests were unavailable because the provider confirmed the daily free neuron allocation was exhausted; no billing changes were made. Actual in-game skin import, live lazer switching, human microphone recognition and osu gameplay/crash freedom were not verified. No confirmed crash repair is claimed.

**Evidence:** [RELEASE_3.18.8.md](<RELEASE_3.18.8.md>); [src](<dist/ONCHART_v3.18.8-source/src>).

<a id="native-3-18-9"></a>

### 3.18.9 — Content-fitting menus and readable scaled bulk presets

- Prevents UI scaling from scaling scroll-content and layout-generated minimum sizes a second time. Page content recomputes its layout minimum, retaining scrollbars only when its actual content needs more space.
- Settings and Analytics tabs now request height from the active panel, so a taller hidden panel does not make a smaller current menu scroll. Drop-downs allow their complete item list when it fits; Qt bounds larger popups to the available screen.
- Bulk-rate preset buttons measure both their name and numeric range/step lines using the current font and styled padding instead of a fixed 138×50 size. The preset group uses the available page width and wraps into more rows as needed.
- Skinning export actions wrap at narrower window widths rather than forcing the page wider than its viewport.
- Stops and disconnects microphone discovery helpers before destroying the assistant settings controls. Fixes a settings/window teardown access violation reproduced during layout regression checks and traced to a completion callback updating a deleted label.
- Updates release and assistant-training metadata to 3.18.9 while preserving prior release folders and archives.

**Validation:** Release build passed. Targeted native results: layout: 4 passed, 0 skipped; assistant: 18 passed, 1 skipped; core: 7 passed, 0 skipped. Checks cover scrolling only under genuine overflow, switching between short and tall tab contents, repeated 100–160% UI scaling with visibly larger fonts, complete two-line preset text, existing scale round-trips, wrapping presets and application layouts across 760×600, 900×650 and 1280×720 windows. Preset screenshots were visually checked at 160%. A deterministic pending-microphone-discovery close regression passed; the seven-check combined window sequence also passed under the debugger without an access violation after the helper lifetime fix. Initial narrow-page and teardown failures are retained in QA logs. Portable startup, deployed Qt library consistency and bundled offline transcription passed. Live osu/lazer gameplay crash freedom remains unverified; this release does not claim a game crash repair.

**Evidence:** [RELEASE_3.18.9.md](<RELEASE_3.18.9.md>); [src](<dist/ONCHART_v3.18.9-source/src>).

<a id="native-3-18-10"></a>

### 3.18.10 — Complete ADOFAI hit streams and distinct navigation icons

- ADOFAI conversion retains every supported gameplay hit at its source timestamp, including dense subdivisions formerly removed by the spacing filter. Midspin markers do not generate phantom hits.
- Randomly selects lanes for streams and tech instead of cycling in a fixed direction. Consecutive hits never use the same lane; hits rounded to the same millisecond use distinct lanes.
- Replaces the 30–500 ms integer filter with optional preferred lane reuse spacing: zero, six decimal places, and large values are accepted. The preference yields when necessary to preserve all hits and audio synchronization. Extremely large values display compactly instead of widening the form.
- Gives all 19 named navigation pages distinct themed icons, including Sessions, Player Tools, Bulk Rate, Skinning, MugDiffusion and DanOverlay. Icons remain distinct when extensions connect or themes refresh.
- Preserves earlier release folders and archives and updates application/training metadata to 3.18.10.

**Validation:** Release build passed. Targeted checks: conversion: 5 passed, 0 skipped; layout: 4 passed, 0 skipped; core: 8 passed, 0 skipped. Dense fixtures preserve all 400 hits through osu! export/reimport at 2/4/7/18 keys with zero, fractional and large spacing; speed, midspin, twirl, pause/hold timing, ZIP conversion and millisecond collisions are checked. UI checks verify rendered icon uniqueness for all 19 named pages, actual installed icons, decimal controls, scaled layouts and bulk presets. Portable startup, deployed Qt library hashes and bundled offline speech regression passed. Unsupported timing events (including FreeRoam, Multitap, AutoPlayTiles, RepeatEvents, SetPlanetRotation and offset timing events) still fail explicitly before output rather than silently producing an inaccurate chart. osu! timestamps have millisecond precision; charts exceeding the selected number of simultaneous lanes are rejected with a request for more keys. Two-key charts necessarily alternate lanes. No live ADOFAI playback or osu/lazer gameplay crash verification was performed; no game crash repair is claimed.

**Evidence:** [RELEASE_3.18.10.md](<RELEASE_3.18.10.md>); [src](<dist/ONCHART_v3.18.10-source/src>).

<a id="native-3-18-11"></a>

### 3.18.11 — Rhythia geometry, Higgsfield skin prompts and square receptors

- Fixes generated standard osu! exports writing mania lane X and constant Y=192 instead of note coordinates. Rhythia SSPM positions and timestamps now survive export/reimport, including the supplied Angel Dust example. Existing source osu! object records retain their original geometry.
- Fits Rhythia quantum coordinates with one uniform chart scale instead of clamping individual notes against playfield edges. The spacing slider still controls normal 3×3 grids; extended grids scale down only when needed to fit.
- Adds a persistent skin prompt, selected-texture/current-section/entire-skin scope and Higgsfield Ideogram 4.0 generation. Each slot submits one paid image request, saves a PNG to the existing workspace, refreshes preview and participates in OSK/OSZ export. Solid edge-connected magenta is removed for sprite transparency; background textures remain opaque. AI artwork requires visual review.
- Stores the complete Higgsfield API key using Windows user encryption. Adds progress, stop-after-current, resume saved batches and forget-batch controls. Durable request IDs and idempotency keys prevent blind duplicate submission. API credentials stay on the API origin and are omitted from media downloads; skin exports exclude prompt/job metadata.
- Mania receptor textures now stretch or squish to lane-width squares by default, retaining the visible bottom-edge hit anchor. Settings → Map preview → Stretch mania receptor textures to square (1:1) disables this behavior and persists across launches. Video export uses the same saved preview settings.
- Preserves prior release folders and archives; updates app and training metadata to 3.18.11.

**Validation:** Release build passed. Targeted checks: conversion: 14 passed, 0 skipped; skin_generation: 7 passed, 0 skipped; preview_modes: 9 passed, 2 skipped; layout: 4 passed, 0 skipped; core: 9 passed, 0 skipped. Supplied SSPM: 1621 notes and 9 distinct positions verified through export/reimport, with timestamps exact and spatial rounding within half a pixel. Synthetic extended-coordinate fixtures verify uniform fitting. Receptor pixel bounds verify 1:1 default versus original-height option; settings persistence and legacy note/hold anchors are checked. Local HTTP tests cover authenticated submit/poll, unauthenticated media download, durable stop/resume, distinct idempotency keys, Windows encrypted key round-trip, blocked foreign status URLs, sprite transparency and prompt persistence/export filtering. Portable startup, 26 deployed Qt library hashes and bundled offline transcription passed. No Higgsfield API key was available in this environment, so live paid generation and model-account access are unverified. AI images may need manual adjustment if they do not follow requested geometry or chroma background. Source rhythm/timing difficulty is preserved, not automatically redesigned. Live osu!/lazer gameplay/crash freedom is not verified; no game-crash repair is claimed.

**Evidence:** [RELEASE_3.18.11.md](<RELEASE_3.18.11.md>); [src](<dist/ONCHART_v3.18.11-source/src>).

<a id="native-3-18-12"></a>

### 3.18.12 — Distinct sidebar icons, all-key random streams and mania skin keys

- Preserves all existing page SVG artwork and adds four distinct vector icons for General, Mapping, Miscellaneous and the extension category. The pack category keeps its existing distinct icon. Category headers no longer duplicate Dashboard, Marathon Maker, Settings or Extensions page icons.
- Fixes collapsed-sidebar theme refresh replacing page icons with the same fallback: icon selection now uses stable tooltips/saved labels rather than the empty compact-view text. Also resolves the shortened Marathon label. Sidebar rebuilds retain labels and compact state; stale motion/registry icons are refreshed. Mug-Diffusion/Dan Overlay aliases resolve correctly.
- Verifies ADOFAI random nonrepeating lanes for every supported 2K–18K stream layout, including dense hits, fractional spacing and exported/reimported columns. Adds an optional seeded reader argument for deterministic verification; normal conversions keep fresh randomness. 2K necessarily alternates between its two lanes.
- Adds a persistent Mania keys selector from 1K through 18K in Skinning. Preview lanes, skin loading and playable OSZ difficulty key counts follow the selection. Missing skin.ini Mania sections are appended while existing sections/custom settings remain intact.
- Prevents 1K skin-preview holds from overlapping the next note on the same lane. Skin archives retain configured key sections while local key-selector metadata stays out of OSK/OSZ files.
- Updates app/training metadata to 3.18.12 and preserves all prior release folders and archives.

**Validation:** Release build passed. Targeted checks: conversion: 5 passed, 0 skipped; skinning: 8 passed, 0 skipped; layout: 4 passed, 0 skipped; core: 7 passed, 0 skipped; memory: 10 passed, 2 skipped. Sidebar tests compare actual rendered icons across all 24 page/category controls, compact/expanded state, stale identical registry icons and connected extensions. Original page SVG hashes match 3.18.11. ADOFAI tests cover all 2K–18K layouts with fixed-seed noncyclic lane transitions and osu! round trips. Skin tests cover 1K–18K preview/configuration, reopen persistence and 1K/2K/7K/18K exported map counts/columns; 1K holds do not overlap. Portable startup, deployed Qt hashes and bundled offline transcription passed. The hash-verified isolated official osu! client survived 90 seconds without OnChart, then another reader session of 90.0 seconds and 1408 read-only polls. These are menu/process survival observations, not live gameplay verification or a confirmed repair of the installed client's access-violation crash. The user confirmed a Windows restart before this follow-up; no startup exclusions or service changes were made by this work. Live Higgsfield account generation remains unverified without a connected API key; previous ADOFAI advanced-event limits remain explicit errors.

**Evidence:** [RELEASE_3.18.12.md](<RELEASE_3.18.12.md>); [src](<dist/ONCHART_v3.18.12-source/src>).

<a id="native-3-18-13"></a>

### 3.18.13 — Responsive settings, song ambience, stable app identity and voice tools

- Removes nested scroll areas from Settings Shortcuts and AI Assistant. The current settings section expands to its content and uses the main page scrollbar only when needed; inactive sections no longer enforce their height on the current section. Height-for-width and parent geometry are refreshed when tabs change.
- Adds a shared subtle theme-colored background with slow floating glows, curved waves and drifting particles. Song pulses follow the live osu! song position and chart BPM, including playback rate. Paused or stale timing stops pulses. Motion updates are bounded to 25 FPS while the window is visible and active; low-end mode uses a static background. A persisted Appearance checkbox and ambience command disable effects.
- Keeps the existing blue OnChart application and executable icons for every selected game. The game selector now uses unmodified official osu!, Quaver, Etterna and Interlude assets, with provenance and attribution. Switching games no longer changes the application icon.
- Adds validated assistant/terminal commands for ambience, skin key counts, texture imports, skin/preview exports, explicitly requested Higgsfield generation, ADOFAI and Rhythia conversion, and keyboard-skin conversion. Existing square-receptor and named converter controls remain available. ADOFAI/Rhythia default to the current map folder, falling back to the input folder.
- Assistant texture-generation actions wait for the real generator result, or report pending work at the bounded action timeout. No generation or paid API call is implied by preview/navigation commands.
- Packages 3.18.13 separately, preserves all prior releases, and updates the full searchable changelog and inventory.

**Validation:** Release build passed. Targeted checks: core: 7 passed, 0 skipped; assistant: 17 passed, 2 skipped; layout: 4 passed, 0 skipped; visual: 3 passed, 0 skipped. Portable startup, deployed Qt libraries and bundled offline transcription passed. UI/command tests cover flat settings sections, stable application icon across all four game profiles, pulse/pause timing, effect toggles, Mania key selection, OSZ export and real ADOFAI conversion through the same validated executor used by voice tools. Official asset hashes and original blue app icon bytes verified. Screenshots inspected. Song effects use live song timing/BPM rather than audio amplitude analysis. Live spoken recognition and paid Higgsfield account generation were not reverified for this release. The recurring installed osu! access-violation crash remains unresolved; prior 3.18.12 menu-only process/reader observations do not establish gameplay stability. No restart, startup exclusions, service changes or writes to the game process were performed.

**Evidence:** [RELEASE_3.18.13.md](<RELEASE_3.18.13.md>); [src](<dist/ONCHART_v3.18.13-source/src>).

<a id="native-3-18-14"></a>

### 3.18.14 — Skin generator below the preview

- Moves the entire Higgsfield prompt and texture-generation section to the bottom of Skinning, below the gameplay/menu preview, status and export controls. Existing generation, saved prompts and preview behavior are retained.
- Packages the layout change as 3.18.14 while preserving all earlier releases and archives.

**Validation:** Release build, existing Mania skin preview/persistence/export check and portable startup/offline transcription checks passed. The 18K skinning screenshot was inspected to confirm the generator panel is below the preview. No paid generation was run. The previously investigated osu! crash remains unresolved; this layout change does not establish gameplay stability.

**Evidence:** [RELEASE_3.18.14.md](<RELEASE_3.18.14.md>); [src](<dist/ONCHART_v3.18.14-source/src>).

<a id="native-3-18-15"></a>

### 3.18.15 — Bundled Discord-TTS and blue Windows branding

- Bundles a Windows Discord-TTS desktop service using the pinned upstream gTTS provider and voice table. Built-in Discord-TTS is the default when no explicit backend has been selected. It starts on demand; users do not need Rust, Python, Docker, a manually managed service, an API key or Cloudflare for speech.
- Keeps External service / Cloudflare selectable and retains the saved URL, encrypted key, provider, Joanna/Matthew voice and speech-rate settings. A separate built-in language setting prevents external voice names from being incorrectly sent to Google Translate. Voice settings and preview can be saved without entering a chat model.
- The bundled service listens only on a random loopback port with a private per-process session key. Requests are authenticated and bounded by text/audio limits and a 30-second synthesis timeout; rate-limit errors do not retry forever. The app hides its child console, probes readiness asynchronously and closes its own service on exit. Wake listening remains paused while the service starts.
- Fixes the actual Windows executable icon: the prior ICO still contained pink artwork despite the blue Qt application icon. Regenerates all ICO sizes from the existing blue PNG and rebuilds the resource. Sidebar and sign-in branding also use that blue image; compact sidebar hides its header logo to preserve space. Game selection does not change the app icon.
- Documents the pinned upstream source, desktop-specific host/provider changes and third-party dependency notices. Deployment hash verification uses the .NET SHA256 implementation when the Get-FileHash cmdlet is unavailable. Preserves all prior releases under a separate 3.18.15 portable package, without replacing the running copy.

**Validation:** Rust release and native release builds passed. Targeted checks: assistant: 18 passed, 2 skipped; core: 5 passed, 0 skipped. Service lifecycle/default-selection tests validate readiness, retained external settings, unauthorized HTTP 401 and child shutdown; external Polly male/female request compatibility remains covered. A live Google request through the bundled executable returned 33024 bytes of MP3, decoded successfully by FFmpeg. Portable startup, deployed Qt hashes and bundled offline transcription passed. Rendered settings/branding and extracted Windows executable icon were inspected. Built-in gTTS requires internet and sends text to Google; it does not provide Joanna/Matthew or offline neural synthesis. Those named voices remain available through the external service. Training-record uploads retain their separately configured destination. No paid provider request or live gameplay crash repair is claimed; the earlier osu! crash remains unresolved.

**Evidence:** [RELEASE_3.18.15.md](<RELEASE_3.18.15.md>); [src](<dist/ONCHART_v3.18.15-source/src>).

<a id="native-3-18-16"></a>

### 3.18.16 — Map preview receptor squish control

- Adds a Map preview setting slider for vertical squish of Mania receptor textures when square receptors are enabled. The default is 0%, preserving the square 1:1 texture; the persisted slider ranges from 0% to 90%.
- Keeps the legacy skin-based receptor sizing when square receptors are disabled. The setting only affects OnChart's preview renderer and does not hook, change or launch osu!.
- Packages the setting in 3.18.16 while preserving all earlier release folders and archives.

**Validation:** Release build and focused receptor rendering, setting round-trip/clamp, and Settings slider integration checks passed. A portable startup check passed. No osu! gameplay session was run, so this preview-only change does not establish a fix for the previously reported osu! crash.

**Evidence:** [RELEASE_3.18.16.md](<RELEASE_3.18.16.md>); [src](<dist/ONCHART_v3.18.16-source/src>).

<a id="native-3-18-17"></a>

### 3.18.17 — ADOFAI compatibility and preview refinements

- Expands ADOFAI import to accept negative and unwrapped angles, midspins, literal line breaks in quoted editor metadata, additional path symbols, nested ZIPs, and visual-only event types. Impossible BPM and negative Hold/Pause sentinels are skipped to avoid collapsed timing. Valid timing events and source note times are retained, consecutive repeated lanes are avoided, and maps still convert when optional audio or background assets are omitted, leaving absent assets unset.
- Corrects song pulse activation for live unpaused play, stops pulses for paused/non-playing states or stale telemetry, and adds persisted strength (0–300%) and reverse controls in Appearance.
- Changes Mania receptor squish to span 0% (no squish) to 100% (full compression), still defaulting to 0%.
- Caches menu skin preview images, pauses the skin animation timer while its tab is hidden, and adapts its visible frame rate to standard/low-end mode. The existing map preview cache and low-end frame limit remain in effect.
- Shows bounded, redacted Higgsfield provider error text and request IDs for HTTP 503 responses, preserves saved generation progress, and retries only transient status polling; it never automatically resubmits a paid generation.
- Packages the fixes as 3.18.17 while preserving previous release folders and archives.

**Validation:** Release build succeeded. Focused tests passed for the supplied ADOFAI archive (10 maps), sentinel and raw-newline compatibility, ambient pulse and receptor settings, Higgsfield 503 diagnostics/no-resubmission, and hidden skin-preview animation. Portable startup with a system-only PATH and offline Whisper sample transcription passed. Full CTest was partial: 11/14 groups passed; the broad native/core group timed out at 120 seconds, and Dan extension plus game-profile tests failed under local engine/cache fixtures. Higgsfield was not submitted to a paid account. The osu! crash remains unverified and restart-based isolation is deferred at the user’s request; no live crash-free claim is made. ADOFAI speed-event angle offsets are quantized at tile boundaries.

**Evidence:** [RELEASE_3.18.17.md](<RELEASE_3.18.17.md>); [src](<dist/ONCHART_v3.18.17-source/src>).

<a id="native-3-19-0"></a>

### 3.19.0 — Windows installer and signed automatic updates

- Adds a per-user Windows x64 installer, Desktop/Start menu launcher, Windows Apps uninstall entry and a signed offline installation payload, without Python, Qt setup or administrator access.
- Checks the stable release registry at launcher startup, supports manual checks, cancellation and an automatic-update preference, defers installation while ONCHART runs, and preserves launch access after a network failure.
- Verifies exact-byte RSA SHA-256 release signatures, SHA-256 archive checksums and signed sizes; restricts downloads to HTTPS GitHub release assets and validates redirects. Rejects ZIP traversal, links, duplicate Windows paths, reserved names, unexpected roots and oversized archives.
- Stages each version separately and atomically switches the installed pointer only after extraction. Retains earlier versions, and rollback disables automatic updates so the previous version stays selected.
- Adds DPAPI-encrypted local signing material, release signing/publishing tools and a separate hosted Lovable database/API. Lovable was given only the backend/GitHub export brief; desktop functionality is maintained locally.
- Packages 3.19.0 separately, preserves previous releases and regenerates the complete Markdown, searchable HTML and inventory.
- 20 October 2026 distribution activation: connects the private RicoHQ/onchart-updates backend to Lovable, publishes verified binaries in the separate public RicoHQ/onchart-releases repository, and publishes the first signed stable registry envelope. The completed 3.19.0 archives are preserved byte-for-byte.

**Validation:** Native release and launcher compilation passed. Launcher harness passed 32 signature, offline-seed, version, checksum, archive safety, transactional failure, side-by-side install and rollback checks. Public hosted registry verified over HTTPS: HTTP 404 with no published release, as expected for an empty registry. Actual signed offline payload verification and complete isolated installation passed; installed application hash matched. Launcher rendering was visually inspected. System-only-PATH startup, 26 Qt library hash checks and offline Whisper sample transcription passed. On 20 October 2026, live distribution was verified with the production launcher code: installed a signed 3.18.17 baseline, read the actual hosted registry, verified the embedded-key signature, downloaded the public 3.19.0 GitHub ZIP, verified size/SHA-256, installed the complete payload, persisted the version switch and rolled back successfully. The test used an isolated workspace folder, without changing shortcuts/registry or launching ONCHART/osu!. The initial release was published through authenticated administrative database deployment; automatic GitHub Actions publishing still requires the backend/CI publishing secret. Offline installation remains available. Application updates do not replace the launcher itself. Authenticode is not configured; the signing key requires a Windows-user recovery backup. Full native suite and osu! gameplay stability were not reverified, and no crash repair is claimed.

**Evidence:** [RELEASE_3.19.0.md](<RELEASE_3.19.0.md>); [DEPLOYMENT_3.19.0.md](<DEPLOYMENT_3.19.0.md>); [src](<dist/ONCHART_v3.19.0-source/src>).

<a id="native-3-20-0"></a>

### 3.20.0 — V2/V3 installer, embedded changelog and archived release history

- Installer offers V2 Classic 2.7.12 and V3 Native with remembered selection, independent installation state, automatic updates and rollback. Existing V3 installation paths are preserved.
- Rejects signed releases from another major version before installing. V2 uses an independently signed GitHub channel; V3 retains the existing hosted update registry.
- Embeds the complete changelog with text search before installation and saves Markdown, searchable HTML and inventory beside the installed launcher.
- Preserves the supplied V2 executable byte for byte and bundles FFmpeg; launching prepends the selected application folder to the child process PATH.
- Website download buttons point to the latest GitHub launcher; setup instructions explain selecting a version and V3 license requirements.
- Publishes saved native runtime history with curated labels, historical changes, validation limitations and SHA-256 verification. Historical local folders and archives are preserved.
- Native version branding now follows the CMake project version rather than the previous hardcoded label.
- Publishes launcher source with a public-key-only build path in RicoHQ/onchartlauncher; keeps the private release key in its original signing context.

**Validation:** 37 launcher checks passed. Both final signed payloads installed with matching app hashes; UI track selection, remembered choice and full changelog content/search passed. V3 system-only-PATH startup, 26 Qt hashes and offline Whisper transcription passed. Actual production signed downloads and installation passed for V2 and V3, including V3 3.19.0 → 3.20.0 update/rollback without changing V2. All 60 historical runtime archive hashes match their public assets; website production build succeeded. Historical apps/games were not rerun; no new game crash repair is claimed. See DEPLOYMENT_3.20.0.md and qa/3200.

**Evidence:** [RELEASE_3.20.0.md](<RELEASE_3.20.0.md>); [DEPLOYMENT_3.20.0.md](<DEPLOYMENT_3.20.0.md>); [src](<dist/ONCHART_v3.20.0-source/src>).

<a id="native-3-20-1"></a>

### 3.20.1 — Binary search for danrate

- Replaces sequential Dan rate scanning with binary search on the 0.01 rate grid between 0.05x and 8.00x, with at most 11 engine evaluations.
- Chooses direction from actual starting DP and selects the nearest matching grid rate, preserving tier/band targets, selected modes, pitch-preserved rate-only exports and the original chart.
- Caches evaluated rates, verifies the final DP interval and rejects invalid results, observed DP reversals and skipped/unreachable bands without creating a difficulty. Existing cancellation remains available.
- Updates terminal help, assistant guidance and progress text; packages 3.20.1 separately and preserves earlier releases.

**Validation:** 13 deterministic tests passed, including 90 comparisons against an exhaustive nearest-rate oracle, boundary rates, plateaus, selected-mode/7K DP, skipped intervals, invalid inputs and timeouts. Linked DanOverlay legacy engine searches passed for Reform, Celestial, Signicial and Shoegazer (9–10 checks each). The previous 1.00x → 4th fixture still returns 0.49x with at most 11 checks rather than 52. Limitations: binary search assumes DP is nondecreasing with rate; sampled reversals fail closed, but unsampled irregularities cannot be detected. The search grid is 0.01, so narrower bands can be unreachable. No osu! gameplay or crash repair was verified. Release build and focused application search/cancellation, exact-rate framing and pitch-preserved rate export checks passed. System-only-PATH portable startup, 26 Qt library hash checks and offline Whisper sample transcription passed. Full native suite and osu! gameplay were not rerun.

**Evidence:** [RELEASE_3.20.1.md](<RELEASE_3.20.1.md>); [DEPLOYMENT_3.20.1.md](<DEPLOYMENT_3.20.1.md>); [src](<dist/ONCHART_v3.20.1-source/src>).

<a id="native-3-21-0"></a>

### 3.21.0 — Live music, mod cards, installer folders and service recovery

- Replaces the Mods dropdown with selectable lazer-style cards. Full LN, No LN and Inverse are mutually exclusive; No SV and Chordjackify combine with a selected note conversion. Applying mods exports a new difficulty and preserves the source.
- Adds 4K Chordjackify: repeated lanes receive adjacent same-hand taps while occupied hold lanes and existing notes are protected. Combined exports preserve timing and supported original metadata.
- Adds passive selected-map and playback-clock readers for supported Quaver and Interlude layouts, using a self-contained .NET 8 helper with ClrMD 4.0.732401. Reads Quaver’s actual configured song folder/mapset/filename, including backing-field layout differences, and Interlude’s exact selected chart hash. The helper does not suspend, inject, debug, invoke target methods, write target memory or walk the entire heap.
- Adds an Etterna public-API theme bridge with preserved original overlays, idempotent installation, InitCommand startup and isolated Lua errors. Resolves virtual /Songs/ paths under the game folder and identifies the exact simfile description, difficulty and step type. Ambiguous/unsupported charts fail closed. The normal Interlude adapter opens the native database read-only; a missing linked audio file no longer prevents the selected chart from loading.
- Decodes the actual map music with bundled FFmpeg into energy, bass and onset features at 10 ms intervals. Background pulses follow the game clock, rate and seeks, stop on pause/silence/stale or unavailable audio, and no longer invent pulses from BPM alone. Analysis is asynchronous, bounded, cancellable and cached. Rapid decoration disable/re-enable restarts cancelled analysis; frozen managed-game clocks stop effects. Visible windows animate while a game is focused; low-end mode disables decoration.
- Hardens osu! memory reads and scans to readable resident pages, retains guard-page rejection and bounds scanning per poll. Cold data may take longer to discover. This is reader hardening, not a confirmed lasting game-crash repair.
- Adds Installation folder → Change folder to launcher 3.21.0, before or after installation. Stages and checksum-verifies both version families, rollback copies and preferences in an empty dedicated destination, remembers it, updates shortcuts/uninstall registration and keeps the original folder as a backup. Cancellation/failure leaves the original available. Rejects unrelated nonempty destinations, nested roots, drive/personal-folder roots and reparse points; custom-folder uninstall verifies ownership.
- Improves HTTP 503 recovery and diagnostics. Chat retries the exact logical request at most twice for 429/502/503/504, honors bounded Retry-After/backoff and cancellation, and shows redacted provider errors/request IDs. Higgsfield safe status/download retries use a separate consecutive-failure counter instead of exhausting their allowance during normal polling. Paid submissions are not automatically repeated; Resume does not repeat an unconfirmed server-failed submission, while a confirmed same-origin accepted request can resume polling.
- Saves bounded last-failure diagnostics without request bodies or API keys. Retains existing danrate binary search on the 0.01 precision grid, verified at at most 11 evaluations rather than scanning each 0.01 step. Packages 3.21.0 separately and preserves earlier releases.

**Validation:** Release build passed. Sixteen feature checks passed with no skips, including actual selected Interlude/Quaver chart imports and audio decoding, Etterna live state/exact difficulty/audio, a real-audio peak pulse, silence/selection stopping, rapid analysis cancellation/restart, mod exclusions/exports and error redaction. Nine focused assistant checks passed for transient retry, exhaustion, cancellation, authentication failures and tool-completion safeguards; six skin checks passed for normal resume, separate polling/CDN retries, unconfirmed paid-submission protection and unsafe URLs. Fifty-one launcher checks passed, including custom location copy, checksums, both tracks, rollback/preferences, preserved originals and cancellation; the folder UI and uninstaller syntax were inspected. Four existing ambient-setting checks passed. Thirteen deterministic Dan search checks and four real linked DanOverlay modes passed (9–10 evaluations). Resident-memory fixtures passed across the full run and subsequent focused guarded-page recovery checks; the full memory group was not repeated after that fixture correction, and real-game optional memory probes were skipped. Interlude and Quaver live reads showed advancing 0.50x clocks with active music; Etterna exported its actual map/clock/rate, and decoded music drove a pulse while selection stopped it. System-only-PATH portable startup, 26 Qt library hashes and offline Whisper transcription passed. Google’s configured gemini-3.1-flash-lite passed a metadata GET and one minimal chat with HTTP 200; no private application data or tool execution was involved. No new paid Higgsfield generation was submitted. Limitations: external providers can still return 503; their underlying availability cannot be repaired by this client, and the exact older Higgsfield failure body was unavailable. Different game versions may change reader layouts. Quaver-native simfile selection, unsupported SV/timing groups, Etterna stops/warps/mines and native replay/score parity retain the documented limits. The independent osu! baseline exited with System.StackOverflowException before the new reader attached; no lasting crash repair or crash-free gameplay is claimed. Application updates do not replace an older launcher binary: run the new setup for its folder selector.

**Evidence:** [RELEASE_3.21.0.md](<RELEASE_3.21.0.md>); [src](<dist/ONCHART_v3.21.0-source/src>).

## Website releases

<a id="website-2026-10-17"></a>

### Site 2026.10.17 — Premium public website refresh

- Refreshes the public landing and account pages with clearer copy, glass surfaces, themed gradients, textured backgrounds, card lighting, staggered scroll reveals and polished controls inspired by React Bits.
- Keeps the four game themes, account forms, download links and existing desktop feature/compatibility details; reduced-motion preferences disable decorative animation.
- Packages the website in a new dated site release directory without changing prior native release folders or archives.

**Validation:** Static HTML, JavaScript syntax and theme tests passed. Browser screenshot capture was unavailable because the local headless browser GPU process failed; desktop and mobile visual rendering remain unverified. Account backend and live payment/download flows were not exercised.

**Evidence:** [index.html](<../../../../index.html>); [onchart-accounts.html](<../../../../onchart-accounts.html>); [premium-site.css](<../../../../premium-site.css>); [premium-site.js](<../../../../premium-site.js>).

<a id="website-2026-10-17-2"></a>

### Site 2026.10.17.2 — React Bits experience additions

- Adds static-site interpretations of Gradient Waves, Text Loop, Topography, Option Wheel, Electric Border, Card Swap, Tech Text, Branched Menu and Folder Float to the GitHub onchart-site landing page.
- Connects the game option wheel to the existing four-theme controller and includes keyboard, pointer and reduced-motion behavior.
- Preserves the prior website release package and the public site's existing account, download and product-detail flows.

**Validation:** JavaScript syntax and inline-script parsing passed; the updated HTML has no duplicate IDs. Cloudflare Workers Builds reported success for merged site commit a6b6a6d. Direct desktop/mobile browser rendering and live account, payment and download flows remain unverified.

**Evidence:** [reactbits-experience.css](<../../../../website-releases/2026.10.17.2/reactbits-experience.css>); [reactbits-experience.js](<../../../../website-releases/2026.10.17.2/reactbits-experience.js>); [README.md](<../../../../website-releases/2026.10.17.2/README.md>).

<a id="website-2026-10-17-3"></a>

### Site 2026.10.17.3 — Staff cards and continuous backgrounds

- Introduces a responsive six-card staff grid with consistent portraits, clear roles, creator accent, accessible social links and a repaired external-link icon.
- Feathers waves and topography across section edges, releases clipped card shadows and folder details, and spaces feature cards consistently.
- Smooths pointer-driven contours without repeated canvas allocation and pauses card rotation during keyboard focus.
- Replaces the existing public tester credential block with account sign-in guidance.

**Validation:** Experience JavaScript and inline landing-page scripts parsed successfully; six staff cards and no duplicate HTML IDs. Browser preview timed out, so desktop/mobile appearance remains unverified. Live accounts, payments and downloads were not exercised.

**Evidence:** [index.html](<../../../../website-releases/2026.10.17.3/index.html>); [reactbits-experience.css](<../../../../website-releases/2026.10.17.3/reactbits-experience.css>); [reactbits-experience.js](<../../../../website-releases/2026.10.17.3/reactbits-experience.js>); [README.md](<../../../../website-releases/2026.10.17.3/README.md>).

<a id="website-2026-10-20"></a>

### Site 2026.10.20 — Launcher downloads and V2/V3 setup

- All five application download links point to the latest GitHub launcher rather than Google Drive folders.
- Setup explains selecting V2 Classic 2.7.12 or V3 Native 3.20.0, installing and launching through the launcher, updates and V3 licensed-account requirements.
- Preserves existing account/checkout flows, product capabilities and compatibility limits. Uses the site's existing Cloudflare Workers Build integration.

**Validation:** Static link, HTML structure and JavaScript parsing checks are recorded under qa/3200. Production build and download verification are recorded after publishing. Account/payment flows were not exercised by this change.

**Evidence:** [index.html](<../../../../website-releases/2026.10.20/index.html>); [README.md](<../../../../website-releases/2026.10.20/README.md>).

## Speech service changes

<a id="speech-2026-10-18-1"></a>

### Speech 2026.10.18.1 — Direct Discord-TTS audio forwarding

- Adds opt-in forwarding to an actual Discord-TTS HTTP service through DISCORD_TTS_URL and a separate optional upstream secret. MP3, Ogg and WAV bytes are returned directly; modes and voices come from the upstream service.
- Preserves authenticated training storage and the existing Cloudflare route when forwarding is not configured. Bounds audio responses and request duration, rejects redirects and prevents forwarding client credentials.
- The actual Rust service is not deployed: Cloudflare rejected Containers access because the account needs Workers Paid. Docker is unavailable locally; provider credentials are still required for Polly/Google Cloud. Billing, live settings and prior release archives were not changed. Gemini speech is outside this change.

**Validation:** Local Node tests passed for binary preservation, discovery, upstream failures, authentication separation, invalid configuration, oversized responses and the existing eight training/speech route checks. No real Discord-TTS backend or audible end-to-end playback was verified.

**Evidence:** [worker.mjs](<service/tts/worker.mjs>); [discord.test.mjs](<service/tts/discord.test.mjs>); [DISCORD_AUDIO.md](<service/tts/DISCORD_AUDIO.md>).

## Gaps, aliases and reconstruction limits

- **3.13.1:** no matching source folder, release note or indexed artifact was found.
  A version-number gap is not evidence of an unpublished feature set.
- **3.14.0:** a real saved native executable/folder and note exist, but there is no
  rename-index row. It is covered separately as an intermediate build.
- **1.3:** source changes are proposal comments; the proposed UI is not counted
  as implemented until the later tabbed version.
- **1.9.6 / 1.9.3** and **2.6.11 / 2.6.4:** corresponding single-file sources are
  byte-identical. **3.1.9 / 3.1.8:** compared modular source/docs match; this does
  not certify every generated binary or asset in those folders.
- **2.5.6** and **2.7.12:** the saved source fails syntax parsing. Their intended
  edits are documented without claiming those files run successfully.
- **Python 3.2.12:** the original ZIP and later maintained workspace are different
  snapshots under one label. Eleven matched files differ and eleven later
  source/test files are absent from the ZIP. Python 3.2.13 largely follows the
  older archived tree; it is not proof of an intentional account/marathon removal.
- **Early Python archive variants:** 3.0.0 and 3.1.7 have main.py differences
  between preserved folder and ZIP. The archive comparison records them.
- **3.11.1 artifact aliases:** release and release-runtime variants are grouped
  under one version. Runtime/source ZIPs do not count as additional versions.
- **Unversioned Python onchart.py:** a distinct saved file exists under source/1
  but has no reliable numbered release label, so no version is invented for it.
- Legacy Python startup-reporting code and auxiliary tools were inspected as
  text only. No historical code, browser-history utility, network report or
  credential-bearing destination was executed or published for this changelog.
- Historical full/focused suites often overlap and include setup/cleanup.
  They are not summed across versions into an invented total of unique tests.
- The original native rename classifications are preserved in the inventory;
  a patch-labelled release can still contain substantial features requested under
  that version number. No release was renumbered by this documentation task.

## Audit material

The companion [inventory](CHANGELOG_INVENTORY.csv) contains every entry's branch,
evidence paths, saved artifacts, relevant modified/index times and identity hash.
For modular snapshots, the identity hash fingerprints the sorted source-file hash
mapping; for native entries it is the runtime EXE hash; for single files it is
the file SHA-256. These identities are not interchangeable with whole-ZIP hashes.

Detailed local evidence is under [qa/changelog](qa/changelog): reviewed entries,
source deltas, archive/source comparisons, the existing release-index mapping and
the coverage/consistency report. Native source deltas cover src and tests and
compare the last available source package; missing intermediate source snapshots
are named rather than attributed to a single intervening release.

Existing runtime folders, ZIPs, checksums and the rename index were not modified.

