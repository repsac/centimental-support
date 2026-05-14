# Changelog

Release notes for every published version of Centimental.

## 1.1 (May 2026)

A polish release shaped by real-device feedback from v1.0. Headline changes are iCloud sync going free + opt-in, a tighter Apple Watch theme set, and a layout pass across the gradient-bar tuner family.

**Changed**

- **iCloud sync is now free for everyone, off by default.** Turn it on under **Settings → Sync** to share your preferences, favorites, and custom tunings across your iPhone, iPad, and any other device signed in to the same iCloud account. Previously a Pro feature that auto-enabled on purchase.

**Improved**

- **Color Gradient, Spectrum Spotlight, and Traffic Light** now share a unified layout across iPhone, iPad, and both orientations. Status text moved below the tuner in portrait and is evenly spaced with the string circles. Tick labels added to Traffic Light to match the family.
- **Pure Flame**: the flame now sits flush with the bottom of the screen on every device and orientation.
- **Neon Crosshairs (iPhone portrait)**: bullseye is now properly vertically centered.
- **Shooting Stars (iPhone & iPad portrait)**: target crosshair is now vertically centered in the visible drawing area.
- **Color Gradient orb** gets a richer pulse: tuning pulses scale with how close to in-tune you are, with a stronger continuous pulse when locked.
- Across-the-board copy pass for readability on Settings, the User Guide, and the support site.

**Apple Watch**

- Removed five themes from the Watch picker — **Classic Radar, Pulse Rings, Sonar Ping, Sun On Arc, and Large Needle** — to focus on themes that render cleanly and consistently on the small display. All five remain available on iPhone and iPad.
- Tuner now holds the last detected note and cents reading on screen briefly between plucks instead of blanking, which makes it easier to glance at while still playing.
- Microphone sensitivity recalibrated for the wrist-near-instrument use case.
- DEBUG-only Pro toggle in the theme picker now persists across Watch app restarts (testing convenience only; production builds still trust the iPhone for entitlement).

**Fixed**

- Watch tuner session-floor regression that affected pitch tracking after the screen dimmed and resumed.
- Various small theme positioning glitches on iPhone Pro models with the Dynamic Island.

## 1.0 (April 2026)

Initial public release.

**Features**
- Chromatic tuner for guitar, bass, and ukulele with real-time pitch detection
- 40+ hand-designed visual themes (6 free, rest unlocked with Centimental Pro)
- 6-string guitar, ukulele, and 4-string bass on the free tier
- 7-, 8-, 12-string guitar and 5-, 6-string bass (Pro)
- Every common alternate tuning, including Drop D, DADGAD, Open G, Open D, Open E, Open A, Double Drop D, half-step down, whole-step down, Nashville, baritone, and more
- Custom tuning builder for Pro users, unlimited tunings per instrument
- Capo support that shifts all string targets automatically (Pro)
- Apple Watch app, fully free, includes all watch-compatible themes regardless of Pro status
- iCloud sync of preferences and custom tunings across devices (Pro)
- Tap-to-select string indicators, long-press-to-clear-lock, optional long-press-anywhere reset
- Optional accent-ring / accent-glow selection indicator for themes with subtle highlighting
- Reference pitch adjustable from 420 to 460 Hz
- Accessibility: unified VoiceOver label on the tuner that reads out current state
- Privacy: audio processed entirely on-device, never recorded or transmitted
