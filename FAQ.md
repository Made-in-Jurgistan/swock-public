<div align="center">

<img src="swock_logo.png" width="80" alt="Swock">

# FAQ — Frequently Asked Questions

</div>

---

## General

### What is Swock?

Swock is an Android app that blocks the swipe-to-next-video gesture in short-form video apps
like TikTok, YouTube Shorts, and Instagram Reels. It doesn't block the apps themselves — it
blocks the specific gesture that drives the compulsive scroll loop.

### How does Swock work?

Swock uses Android's accessibility service framework to detect when you're on a Shorts/Reels feed
and intercept the vertical swipe gesture. When you try to swipe to the next video, nothing
happens. Everything else — tapping, liking, commenting, sharing, horizontal navigation — works
normally.

### Is Swock open source?

No. Swock is proprietary software. The source code is not publicly available. This repository
contains only public-facing documentation.

## Privacy

### Does Swock collect my data?

No. Swock collects zero data. There is no INTERNET permission, no analytics, no telemetry, and
no crash reporting. Everything runs locally on your device.

### Does Swock send data to any server?

No. Swock does not communicate with any server. The only network activity is through Google Play
Services for app integrity verification (Play Integrity API), which sends a random nonce and
package name to Google. See the [Privacy Policy](privacy-policy.md) for details.

### What does the accessibility service see?

The accessibility service inspects the screen structure of supported apps to determine whether
you're on a Shorts/Reels feed. It does not read, log, store, or transmit text content,
credentials, or personal data. The inspection is discarded immediately after classification.

## Usage

### Can I still watch videos?

Yes. The current video is fully visible and playable. You can tap to pause, like, comment, and
share. Only the swipe-to-next gesture is blocked.

### Can I still navigate within the app?

Yes. Horizontal swipes (tab navigation), taps, long-press, and edge gestures all pass through
normally. You can search, browse profiles, and use all non-feed features of the app.

### What if I want to swipe to the next video?

You can:
1. Toggle **Swipe Blocking** off in the Swock app
2. Disable the Swock accessibility service in Android Settings
3. Toggle off the specific app in Swock's Protected Apps list

Swock is designed to add friction, not to be unbreakable. The goal is to make the swipe a
conscious choice rather than a reflex.

### Does Swock work in multi-window mode?

Swock only activates in the active/focused window pane in split-screen mode.

### Does Swock work with TalkBack?

Swock is compatible with TalkBack. If you experience any issues, please
[report them](https://github.com/Made-in-Jurgistan/swock-public/issues).

## Technical

### Why does Swock need Android 13+?

Swock uses a touch interception API introduced in Android 13 (API 33). There is no fallback for
older Android versions.

### Does Swock require root?

No. Swock uses Android's built-in accessibility service framework. No root, no VPN, no special
permissions beyond the accessibility service.

### Does Swock drain my battery?

Swock only activates when a supported app is in the foreground and you're on a Shorts/Reels
feed. When you're using any other app, Swock is idle and uses negligible resources.

### Will Swock work after app updates?

Swock operates at the touch gesture level, not the view hierarchy level, so touch interception
continues to work even when apps update their UI. Screen detection may occasionally need updates
if apps significantly change their interface — these are handled in Swock updates.

## Supported apps

### Which apps are supported?

See the [README](README.md#supported-apps) for the full list.

### Can I request support for a new app?

Yes. [Open an issue](https://github.com/Made-in-Jurgistan/swock-public/issues) with the app name
and package name. We'll evaluate whether detection is feasible.

### Can I disable Swock for specific apps?

Yes. In Swock's settings, toggle individual apps on or off under **Protected Apps**.

---

<div align="center">

<sub>(c) 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
