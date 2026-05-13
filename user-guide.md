# User Guide

A complete walkthrough of Centimental. If you're just getting started, read top to bottom. Everything else is organized by topic for later reference.

## Getting Started

Pick your instrument under the **Strings** tab (guitar, bass, or ukulele), then choose a tuning preset. The tuner screen shows all the strings in your preset as circles along the bottom.

Pluck any string. Centimental detects which one you're playing, snaps to it, and shows the note, the cents deviation, and (on most themes) a visual needle or bar guiding you to pitch.

When a string lands in tune and stays stable for a moment, its circle goes green: a breadcrumb that you've successfully tuned that string this session. Move to the next string and repeat.

## Tuning Basics

- **A4 (440 Hz)** is the reference pitch by default. Change it under **Settings → Pitch** if you're playing alongside an ensemble tuned differently (439–442 Hz is common in orchestras).
- **Cents deviation** is the unit of how off-pitch a note is. ±5 cents is imperceptible to most ears; most themes treat anything inside ±4 cents as "in tune" and lock the string.
- **Auto-switching** is on by default. Pluck a different string and the tuner jumps to it within a second. If that feels too jumpy (or not snappy enough), tune **Settings → Picking Style**.

## String Indicators

The row of dots at the bottom of the tuner screen represents each string in your active preset. Each one is interactive:

| Gesture | What it does |
|---|---|
| **Tap** | Selects that string as the active tuning target. Useful when auto-switching picks the wrong string from sympathetic resonance. |
| **Long-press (0.8s)** | Clears that string's "already tuned" breadcrumb so you can re-tune it from scratch. Light haptic confirmation. |
| **Long-press empty tuner area** | Clears every string's lock at once. **Off by default**; enable in **Settings → Reset Locks** if you want it. |

If the default active-string highlighting is too subtle on your chosen theme, pick an extra ring or glow in **Settings → String Indicators → Selection Indicator**.

## Gestures

- **Tap / swipe the tuner**: cycles through themes when **Settings → Theme Switching** is on. Pick between tap-to-advance, swipe, or favorites-only. Off by default so you don't change themes accidentally mid-song.
- **Settings tab**: every preference lives here. Each picker has a one-line hint on the main screen and a verbose explanation per option in its sub-view.

## Themes

Open the **Themes** tab to browse. Tap a theme thumbnail to apply it. Six themes are free; Pro unlocks the full library of 40+.

- **Per-theme light/dark override**: long-press a thumbnail to change appearance for that theme only. The global **Settings → Default Color** applies to everything else.
- **Favorites**: tap the heart on a thumbnail to favorite it. **Settings → Theme Switching → "Tap to advance favorites"** then cycles only between your favorites on the tuner screen.
- **Column count**: use the column icon in the Themes tab toolbar to switch between 1, 2, 3, or 4 columns. 1 column is an accessibility option on iPhone for users who prefer larger thumbnails.

See the **[Theme Gallery](themes/)** for screenshots of every theme.

## Apple Watch

The Apple Watch app is **free**. Every watch-compatible theme is included regardless of whether you've unlocked Pro on iPhone. Haptics guide you to pitch so you can tune without looking at the screen, useful for backstage tuning in the dark.

- **Pairing** syncs your active theme, instrument, tuning preset, reference pitch, Pro status, and (Pro) custom tuning library from iPhone to Watch automatically. Subsequent changes propagate over WatchConnectivity.
- The Watch runs its own tuner independently, so it doesn't need iPhone nearby while tuning.

## Pro Features

Centimental Pro is a **one-time purchase**, no subscription. It unlocks:

- The full theme library (40+ themes)
- 7-, 8-, and 12-string guitar
- 5- and 6-string bass
- Every alternate tuning (Drop D, DADGAD, Open G, Open D, Open E, Open A, Double Drop D, half-step down, whole-step down, Nashville, baritone, and more)
- The custom tuning builder, with unlimited tunings per instrument
- Capo support (shifts all string targets up by your chosen fret)

Restore a previous purchase from **Settings → Upgrade → Restore Purchase**. Purchases are tied to your Apple ID.

## Custom Tunings (Pro)

1. Go to the **Strings** tab.
2. Scroll to the **Custom** section and tap **Create Custom Tuning**.
3. Name your tuning, pick an instrument, and set each string's note + octave.
4. Save. The tuning appears in the Custom section and syncs to your other devices via iCloud.
5. To edit or delete, swipe on the tuning in the list.

## Capo (Pro)

Under **Settings → Capo**, pick the fret your capo is clipped to (1 through 12). Centimental shifts all string targets up that many semitones automatically, so your tuner displays the capo'd pitch, but note names stay in the familiar open-chord names for each string.

## Settings Tour

Organized by category on the Settings tab:

- **Playing**
  - Capo
  - String Indicators (lock behavior, selection indicator ring/glow)
  - Lock Feedback (animation + haptic style)

- **Signal**
  - Reference Pitch
  - Noise Gate
  - Attack Mute
  - Picking Style
  - Stability Indicator

- **Interface**
  - Display (fractional cents, prefer sharps, show theme name on switch)
  - Theme Appearance (default color mode)
  - Theme Switching (tap / swipe gesture)
  - Reset Locks (long-press-anywhere toggle)

- **Hardware**
  - Audio Input (active input, microphone selection on multi-mic phones)

- **Sync**
  - iCloud Sync (off by default; share preferences, favorites, and custom tunings across devices signed in to the same iCloud account)

- **Upgrade** (pre-Pro only)
  - Upgrade button
  - Restore Purchase

- **About**
  - User Guide
  - Version
  - Contact / Feedback

## Troubleshooting

See the dedicated **[Troubleshooting](troubleshooting.md)** page for common questions and fixes.

## Feedback

The developer genuinely reads every email: [appstore@edcaspersen.com](mailto:appstore@edcaspersen.com). If something's broken or missing, say so.
