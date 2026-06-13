# Changelog

Release notes for every published version of Centimental.

## 1.2 (pending)

A reliability and polish release: a sharper fix for an Apple Watch rendering
glitch, a roomier iPad layout, a friendlier first run, and a clearer way to
see what Pro includes.

**New**

- **Reference tone.** Open Settings → Reference Tone to pick a note and
  octave and play it to tune by ear. It follows your reference pitch. Free for
  everyone.

**Improved**

- **iPad layout.** The Themes grid now shows more themes at a glance by
  default, and the Strings and Settings screens keep their content at a
  comfortable reading width instead of stretching edge to edge. You can still
  set the grid to 2–4 columns yourself.
- **A more visual welcome.** The first-run style picker now previews each
  theme, so you can see what you're choosing instead of picking by name.
- **A clearer upgrade screen.** Tapping a Pro theme now opens a screen that
  shows exactly what Centimental Pro includes and what it costs, with Restore
  Purchase one tap away.
- **Easier string selection.** The active-string indicator is now on by
  default, and tapping a string circle selects it as your target right away —
  even before you play a note.

**Fixed**

- **Apple Watch rendering reliability:** addressed an occasional glitch where
  part of a Watch theme could flash a solid colored square over the animation.
  Watch themes now animate at a steadier rate and pause cleanly when your
  wrist is down.
- **Converging Columns (iPhone portrait):** the note readout is now correctly
  centered above the bars instead of sitting too high.
- **Split Bar (iPhone and iPad portrait):** the center line is now vertically
  centered, with the note above and the status and string circles evenly
  spaced below the bar.
- **Tapping instrument and tuning rows:** the whole row is now tappable, not
  just the text label — easier to hit, especially on iPad.
- **Lapsed Pro:** if a Pro purchase is refunded or removed through Family
  Sharing, the app now returns you to a free theme, instrument, and tuning
  instead of leaving Pro content selected.

**Under the hood**

- More consistent pitch-detection calibration across iPhone, iPad, and Apple
  Watch, kept in one place so the three stay in sync.
- The Noise Gate setting now takes effect immediately while the tuner is
  running, instead of only after a restart.
- The app now classifies a connected audio interface correctly at launch, and
  shows a friendlier name for the built-in microphone in Settings.
- Reference pitch is now kept within a sensible range, even if a stray value
  arrives from iCloud sync.
- In the rare case its settings store can't load, the app now shows an
  explanatory screen instead of failing to open.
- Added internal diagnostics, routed through the system log, to make Watch and
  purchase issues easier to track down.
- Documentation corrections (accurate theme count, an iCloud Sync section in
  the in-app User Guide).

## 1.1 (May 2026)

A feature-and-polish release shaped by real-device feedback from v1.0.

**New**

- **Eight new instruments**, each with built-in tunings: Baritone Guitar,
  Banjo (5-string), Banjo (4-string), Mandolin, Violin, Viola, Cello, and
  Double Bass. Part of Centimental Pro, joining the 7-, 8-, and 12-string
  guitars and 5- and 6-string basses.

**Changed**

- **iCloud sync is now free for everyone, off by default.** Turn it on under
  Settings → Sync to share your preferences, favorites, and custom tunings
  across your iPhone, iPad, and any other device signed in to the same iCloud
  account. It was previously a Pro feature that turned on automatically with
  purchase.

**Improved**

- **Color Gradient, Spectrum Spotlight, and Traffic Light** share a unified
  layout across iPhone, iPad, and both orientations.
- **Pure Flame** now sits flush with the bottom of the screen on every device.
- **Neon Crosshairs** and **Shooting Stars** are now properly vertically
  centered.
- **Color Gradient orb** gets a richer pulse that intensifies as you approach
  in-tune.
- A copy pass for readability across Settings and the User Guide.

**Apple Watch**

- A more focused theme picker: five themes that did not render cleanly on the
  small display (Classic Radar, Pulse Rings, Sonar Ping, Sun On Arc, Large
  Needle) are now iPhone and iPad only.
- The tuner holds the last detected note and cents on screen between plucks
  instead of blanking, so you can glance at it while still playing.
- Microphone sensitivity recalibrated for the wrist-near-instrument use case.

**Fixed**

- A Watch tuner regression that affected pitch tracking after the screen dimmed and resumed.
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
