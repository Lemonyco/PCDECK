# Changelog

## 1.13.0-dev.1 — LiveDeck
- Added full-screen LiveDeck widget board for the tablet.
- Added context-aware active-app controller with bounded window/media/audio controls.
- Added live Windows per-app audio mixer.
- Added server-owned Workspace Snapshot / Restore with exact window geometry and master-volume recovery.
- Added local LiveDeck widget sizing/reordering.
- Added LiveDeck to the professional command strip, Quick Dock, Control Hub, and Control Center summary.
- Snapshot restore accepts opaque snapshot IDs only; executable paths and geometry remain PC-side.
- Added 1.13 regression/security tests.

## 1.12.0-dev.1
- Added professional segmented navigation to Control Center.
- Added Editor selection inspector and faster tablet entry.
- Added professional tablet command strip and progressive disclosure.
- Unified visual hierarchy across PC and tablet surfaces.

# PCDeck 1.11.0-dev.1

- Added Workspace Engine for one-tap app/activity orchestration.
- Added installed-app workspace builder with opaque App Stage IDs.
- Added bounded Windows layouts: fullscreen, halves, quarters, and centered.
- Added profile/page and tablet Layout Studio handoff per workspace.
- Added optional master-volume presets, progress, cancellation, and starter templates.
- Added Workspace Engine to Quick Dock and Control Hub.

# Changelog

## 1.10.0-dev.1 — Whole Product Polish

- Unified Control Center and Editor around shared desktop themes, density, text scaling, and accent preferences.
- Added customizable Control Center cards and a compact live status strip.
- Reworked Editor hierarchy, search/filter performance, preview customization, and toolbar density.
- Added tablet density, surface, motion, and Quick Dock position controls to Layout Studio.
- Fixed stale hard-coded desktop version labels by packaging `VERSION`.
- Added 1.10 regression coverage for customization settings and remote-surface safety.

## 1.9.0-dev.1 — Layout Studio

- Added tablet-local Layout Studio with drag/reorder, resize, hide, undo and redo.
- Added optional tablet-specific pages independent of PC profile page assignments.
- Added tablet-only folders/stacks for grouping existing controls.
- Added customizable Quick Dock including favorite control shortcuts.
- Added widget gallery controls for active app, storage, audio, running apps, clock and connection.
- Added Professional, Developer, Gaming, Media and Minimal layout presets.
- Added compact, hero and minimal Big App presentation modes.
- Added optional separate portrait/landscape layouts.
- Added JSON layout-pack copy/import foundation for sharing layouts later.
- Added Simple vs Advanced dashboard complexity modes.
- Kept Layout Studio client-side and reused existing authenticated PCDeck action IDs.

## 1.8.0-dev.1 — Professional Tablet

- Added a professional default tablet design system with calmer surfaces, consistent spacing and restrained shadows.
- Reworked the symbol-only Command Rail into a labeled Quick Dock on tablets.
- Replaced the animated Overdrive orb with a compact Control Hub pill.
- Polished Big Apps and App Stage cards for a more commercial launcher/Mission Control feel.
- Improved tablet dialog sizing, header hierarchy, touch targets and responsive spacing.
- Kept RGB/Aura/Showcase effects available as opt-in customization rather than making them dominate the default UI.
- Added 1.8 UI regression tests without changing the existing remote-command/network security surfaces.

## 1.7.0-dev.1 — App Stage

- Added Big Apps shelf with large one-touch cards.
- Added full-screen App Stage with My Apps, Installed and Running modes.
- Added cached Windows Start-menu app catalog with opaque launch IDs.
- Added Running/Mission Control cards for focus, minimize, maximize and close.
- Added app search and explicit app-catalog refresh.
- Active-app widget now opens Mission Control.
- Expanded tablet dialog sizing to viewport-based tablet detection in addition to coarse-pointer detection.
- Added 1.7 regression/security tests.

## 1.6.0-dev.1 — Tablet Command OS

- Added full-screen Pilot Mode combining AirTouch, live PC telemetry, launch controls and recent actions.
- Upgraded AirTouch to AirTouch Pro with precision mode, middle click, dedicated scroll rail and opt-in Gyro Pointer.
- Added optional floating Command Rail for instant tablet navigation.
- Enlarged feature dialogs and touch targets on tablet/coarse-pointer devices.
- Kept Pilot/Command Rail client-side and reused the existing paired action + bounded AirTouch security model.

## 1.5.0-dev.1
- Added Tablet Overdrive control surface.
- Added Command Orbit radial launcher using favorites, recent actions, and current-profile controls.
- Added full-screen Showcase HUD with clock, active app, Flow mode, CPU/RAM, profile, and dashboard latency.
- Added optional Idle Showcase timer.
- Added System Pulse visual response to live PC load.
- Added opt-in Holo Tilt device-orientation parallax.
- Added Touch Sparks and safe blank-area swipe profile navigation.
- Added tablet-local recent action history and Replay Last.
- Kept Overdrive history/preferences entirely in browser localStorage and added no new remote-command endpoint.
- Added three regression tests for the 1.5 tablet feature surfaces and privacy boundaries.

## 1.4.1-dev.1
- Fixed Windows test/build timeouts caused by synchronous PowerShell adapter discovery inside `/api/status`.
- Added cached network snapshots with background stale refresh so tablet polling stays responsive.
- Manual Network Refresh and Diagnostics still force a fresh Windows adapter scan.
- Added a regression test for network-discovery caching.

## 1.4.0-dev.1

### Added
- Product-style Windows Control Center with connection, pairing, system health, tools, and diagnostics cards.
- Multi-adapter IPv4 discovery and dynamic host allow-list refresh.
- Packaged-app firewall inspection and UAC-backed LocalSubnet repair flow.
- NeuralDeck Local opt-in application-transition learning and next-control suggestions.
- PCDeck Fusion paired-device file drop into `Downloads\PCDeck Incoming`.
- Fusion recent-file surface and incoming-folder shortcut.
- Six new automated tests for 1.4 behavior.

### Fixed
- Wi-Fi/Ethernet addresses on multi-homed Windows PCs no longer disappear from PCDeck host validation just because hostname lookup preferred a different adapter.
- The connection UI no longer blindly advertises the first IP returned by Python.

### Privacy / security
- NeuralDeck is disabled by default and stores only local app transition counts.
- Fusion requires pairing, sanitizes filenames, blocks traversal, avoids overwrites, and limits the development transport to 8 MB.
- Firewall repair targets only the packaged PCDeck executable and LocalSubnet traffic.

## 1.3.0-dev.1

### Added
- PCDeck Flow context engine and adaptive visual mode.
- PCDeck Spaces for switching among saved PCDeck computers.
- QuickDrop explicit paired-device clipboard bridge.
- Global Command Palette (`Ctrl/Cmd + K`) across profiles/pages.
- Feature-pack validation tests.

### Retained
- AirTouch wireless touchpad.
- Smart Controls and active-app profile matching.
- Scenes/macros, media controls, live PC metrics, trusted-device pairing.
- RGB/aura tablet appearance system.

### Safety / privacy behavior
- QuickDrop never monitors the clipboard in the background.
- Flow does not execute arbitrary commands automatically.
- New APIs remain behind PCDeck pairing/session authentication.
