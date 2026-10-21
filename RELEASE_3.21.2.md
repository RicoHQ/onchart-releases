# ONCHART 3.21.2

Blue default remote theme and app icons

- Updates ONCHART Remote 1.0.1 to match the desktop’s existing default blue accent (#38bdf8), with navy surfaces, blue gradients, selected mod cards, playback controls, pairing illustrations, toggles and navigation. The desktop’s saved custom theme choices remain available.

- Replaces the green browser/home-screen, Android adaptive/legacy and iOS app icons with blue versions of the ONCHART remote mark. Updates Android/iOS launch artwork, browser theme metadata and native system-bar/background colors to the same palette.

- Publishes a signed Android update with the existing app identity and signing key (versionCode 2). Embeds the new remote interface in desktop 3.21.2 and retains pairing, controls, V2/V3 selection, installation folders, signed updates and rollback. Preserves earlier release packages; development sources and signing keys remain private.

## Validation and limitations

Desktop and signed Android release builds passed. The final blue interface passed all five existing Chromium/WebKit touch-layout and interaction checks, including minimum 44-pixel targets. Default computed accent/background colors, browser manifest and icon colors were checked, and screenshots were visually reviewed. Thirteen existing native remote checks and twelve client checks passed. Android signature, versionCode and embedded-asset equality were verified; the native iOS project was synchronized. Limitations: physical Android/iPhone and USB networking remain untested; no native iOS binary was built on Windows. The local remote requires a trusted private network. Game-reader, provider availability and previously documented osu! crash limitations are unchanged; no new gameplay/crash repair is claimed.
