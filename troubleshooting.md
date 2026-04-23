# Troubleshooting

Quick answers to the most common questions. If your issue isn't here, email [appstore@edcaspersen.com](mailto:appstore@edcaspersen.com) with a short description and what device / iOS version you're on.

## The tuner isn't detecting my pitch

1. Check that microphone permission is granted. Open iOS **Settings → Privacy & Security → Microphone** and confirm Centimental is toggled on. If it's off, toggle on and relaunch.
2. In Centimental, go to **Settings → Audio Input** and confirm the "Active Input" reads a real device.
3. If the input looks right but notes still don't register, open **Settings → Attack Mute → Off**. The mute can swallow very soft plucks on some instruments.

## Detection is jumpy on low strings

Low E on guitar and low B on a 5-string bass are physically the hardest pitches to detect cleanly. Their fundamentals are below ~80 Hz where acoustic energy is quiet and overtones are louder than the fundamental.

- Try **Settings → Picking Style → Standard (Pick)**. A firmer strum helps the pitch detector find the fundamental faster.
- Raise **Settings → Noise Gate** if you're in a loud room. The threshold filters out background noise that can confuse low-string detection.
- If you're on the iPhone's built-in mic, consider plugging in a USB-C audio interface. Direct signal from the pickup is dramatically cleaner than mic'd sound.

## The wrong string is getting detected

Sympathetic resonance (other strings vibrating in sympathy with the one you plucked) can fool auto-switching.

- **Tap the string circle** for the string you want to tune. This manually selects it as the active target and suppresses auto-switching for a moment.
- Damp the other strings with your fretting hand while you tune.

## My lock haptic isn't firing

1. Make sure **Settings → Lock Feedback → Haptic** is on.
2. Pick a haptic style: **Medium** or **Heavy** are the most reliably felt. **Light** is genuinely subtle on newer iPhones.
3. Tap **Test Haptic Now** to preview.
4. If Test works but lock haptics don't, silent mode or a Focus profile may be suppressing system haptics. iOS 17 and later routes many haptics through the audio ducking system.

## Audio cuts out when I plug in a USB-C interface

Centimental handles USB-C audio route changes automatically, but some interfaces need a few seconds to negotiate sample rate and settle.

- Wait ~3 seconds after plugging in. If nothing happens, go to **Settings → Audio Input** and tap **Stop Tuner → Start Tuner** to force a fresh engine startup.
- Some interfaces default to 96 kHz on first connect. Centimental works at 44.1 or 48 kHz. If your interface has a sample-rate switch, try the lower setting.

## iCloud sync isn't working across devices

- iCloud sync requires **Centimental Pro**. Without Pro, the sync service is gated off.
- Confirm both devices are signed in to the same iCloud account.
- Confirm iCloud Drive is enabled: **iOS Settings → your Apple ID (top of Settings) → iCloud → iCloud Drive**.
- KVS sync propagation can take a few seconds on Wi-Fi, up to a minute on cellular. It's not instant.
- Try force-quitting and relaunching the app on the receiving device. Apps occasionally miss a sync notification if they've been backgrounded for a long time.

## A custom tuning I made disappeared

Custom tunings are stored locally and (for Pro users) backed up to iCloud KVS. If a tuning vanishes:

1. Force-quit and relaunch the app. iCloud sync occasionally needs a foreground event to fetch.
2. Check the **Strings** tab on your other devices. If the tuning's there, a sync will bring it back to the device that "lost" it.
3. Centimental uses UUID-based union merge when two devices have different tunings offline, so in normal operation no tuning should be lost, even during offline edits. If you have a genuinely missing tuning, please email us at [appstore@edcaspersen.com](mailto:appstore@edcaspersen.com) with your Apple ID email and we'll investigate.

## The Watch app can't find my custom tuning

The Watch syncs your custom tuning library from the iPhone via WatchConnectivity. If a custom tuning selected on iPhone doesn't appear on Watch:

1. Confirm both devices have **Centimental Pro**.
2. Open the iPhone app. The moment the iPhone app is in the foreground, pending WatchConnectivity transfers flush.
3. On the Watch, force-quit and relaunch the app (digital crown → app switcher → swipe right on Centimental → X).
4. If nothing works, unpair and re-pair in the iPhone **Watch** app.

## The app crashes on launch

If a crash happens before the UI appears, iOS's persistent store may have been corrupted (power loss during a write, interrupted update). Centimental automatically recovers with an in-memory fallback, but preferences won't persist until the store heals.

- Force-quit the app and relaunch. SwiftData's recovery path creates a fresh persistent store.
- If the problem persists, uninstall and reinstall. If you have Pro and iCloud sync, your custom tunings will re-sync on first launch.

## How do I reset everything?

Delete the app and reinstall. All local preferences, favorites, and custom tunings are wiped. If you're Pro with iCloud sync enabled, iCloud values will still be there and resync on first launch. To truly start fresh, turn off iCloud sync briefly, delete the app, then reinstall.

## Feature requests and bugs

Email [appstore@edcaspersen.com](mailto:appstore@edcaspersen.com) or file an issue on the app's [GitHub issues page](https://github.com/repsac/centimental-ios/issues). Include:

- What you expected to happen
- What actually happened
- Device model and iOS version (**iOS Settings → General → About**)
- Centimental version and build (**Settings → About → Version**)

Short, specific reports are much easier to act on than vague ones. Screenshots help a lot.
