# Privacy Policy

**Last updated:** April 19, 2026

## What Centimental does with your data

**Nothing.** Centimental is an on-device tuner. It does not collect, store, or transmit personal data. There is no user account, no analytics backend, no tracking, and no advertising.

## Microphone access

Centimental requires microphone access to detect pitch in real time. Audio from the microphone is processed entirely on your device, frame by frame, to estimate the pitch you're playing. **Audio is never recorded, saved, or sent anywhere.** The moment a frame has been analyzed, it is discarded.

If you deny microphone access, the app cannot function. Pitch detection is the entire purpose of a tuner.

## Data stored on your device

Centimental uses Apple's SwiftData framework to persist your preferences locally:

- Active instrument, tuning preset, and visual theme
- Your custom tunings (if you've created any with Centimental Pro)
- Your favorite themes and tunings
- Preference choices (reference pitch, lock behavior, haptic style, selection indicator, theme appearance mode, etc.)

All of this data stays on your device. The app cannot read it, modify it, or share it over the network.

## iCloud sync (opt-in)

iCloud sync is **off by default**. Turn it on in **Settings → Sync** if you want to share your preferences across devices. Available to every user, no purchase required.

When enabled and you're signed in to iCloud, the preferences above are synchronized across your Apple devices using Apple's `NSUbiquitousKeyValueStore` (iCloud Key–Value Storage).

- Sync is end-to-end managed by Apple. Centimental does not operate any server.
- The data stored in iCloud KVS is limited to your app preferences and custom tunings. No audio, no usage data, no identifiers.
- You can disable iCloud sync at any time from **Settings → Sync**, by signing out of iCloud in iOS Settings, or by removing iCloud Drive access for Centimental. Disabling stops further sync; data already in iCloud is preserved until you sign out of iCloud or delete the app.
- Apple's privacy policy governs iCloud: <https://www.apple.com/legal/privacy/>

## App Store purchase

The one-time Centimental Pro in-app purchase is processed entirely by Apple's App Store. Centimental never sees your payment information. Your purchase is associated with your Apple ID for restore purposes.

## WatchConnectivity

If you install Centimental on Apple Watch, your iPhone and Watch exchange preferences (active theme, active tuning, custom tuning library, reference pitch, Pro status) using Apple's WatchConnectivity framework. This data travels only between your iPhone and your paired Watch, with no server involved.

## Crash reports and diagnostics

Centimental does not include any third-party crash reporter, analytics SDK, or tracking library. If you choose to share crash logs with Apple via **Settings → Privacy & Security → Analytics & Improvements**, Apple may include Centimental crash data in the reports they send to developers. This is controlled entirely by you through iOS's system settings.

## Children's privacy

Centimental does not knowingly collect data from any user, including children.

## Changes to this policy

If this policy ever changes in a material way, the update will be reflected here and noted in the app's release notes. The app's in-app User Guide points at this page.

## Contact

For privacy questions, email **appstore@edcaspersen.com**.
