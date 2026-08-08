<div align="center">

<img src="swock_logo.png" width="64" alt="Swock app logo — shield icon">
<br>
<img src="swock_wordmark.jpg" width="280" alt="Swock wordmark">

# FAQ — Frequently Asked Questions

</div>

---

## Contents

- [General](#general)
- [Privacy & data](#privacy--data)
- [Usage](#usage)
- [Technical](#technical)
- [Supported apps](#supported-apps)
- [Accessibility service](#accessibility-service)
- [Comparison & alternatives](#comparison--alternatives)

---

## General

<details>
<summary><b>What is Swock?</b></summary>

Swock is an Android app that blocks the swipe-to-next-video gesture in short-form video apps like
TikTok, YouTube Shorts, and Instagram Reels. It doesn't block the apps themselves — it blocks the
specific gesture that drives the compulsive scroll loop.

</details>

<details>
<summary><b>Why is it called Swock?</b></summary>

Swock is a portmanteau of "swipe" and "block" — it blocks swipes. The name is short, memorable,
and describes exactly what the app does.

</details>

<details>
<summary><b>Who is Swock for?</b></summary>

Swock is for anyone who finds themselves scrolling short-form video apps more than they want to.
You don't need to be clinically addicted to benefit — if you've ever lost an hour to TikTok when
you meant to spend five minutes, Swock is for you.

</details>

<details>
<summary><b>Is Swock open source?</b></summary>

No. Swock is proprietary software. The source code is not publicly available. This repository
contains only public-facing documentation — privacy policy, terms of service, FAQ, and support
information. The app's privacy practices are fully documented, and the fact that it declares no
INTERNET permission can be verified by anyone who inspects the APK.

</details>

<details>
<summary><b>Is Swock a medical treatment for addiction?</b></summary>

No. Swock is a digital wellbeing tool that adds friction to compulsive scrolling. It is not a
medical device, a treatment for addiction, or a substitute for professional help. If you're
struggling with compulsive social media use, consider speaking with a mental health professional.

</details>

<details>
<summary><b>How much does Swock cost?</b></summary>

Swock is free. No ads, no in-app purchases, no subscription.

</details>

---

## Privacy & data

<details>
<summary><b>Does Swock collect my data?</b></summary>

No. Swock collects zero data. There is no INTERNET permission, no analytics, no telemetry, and no
crash reporting. Everything runs locally on your device. See the
[Privacy Policy](privacy-policy.md) for full details.

</details>

<details>
<summary><b>Does Swock send data to any server?</b></summary>

No. Swock does not communicate with any server. The only network activity is through Google Play
Services for app integrity verification (Play Integrity API), which sends a random nonce, package
name, and device integrity signals to Google. See the [Privacy Policy](privacy-policy.md) for
details.

</details>

<details>
<summary><b>What does the accessibility service see?</b></summary>

The accessibility service inspects the screen structure of supported apps to determine whether
you're on a Shorts/Reels feed. It does not read, log, store, or transmit text content,
credentials, or personal data. The inspection is discarded immediately after classification.

</details>

<details>
<summary><b>Does Swock sell or share my data?</b></summary>

No. Swock has no data to sell or share. It collects nothing.

</details>

<details>
<summary><b>Where are my settings stored?</b></summary>

All preferences are stored locally on your device in app-private storage. They never leave your
device.

</details>

<details>
<summary><b>Can I verify that Swock doesn't collect data?</b></summary>

Yes. Swock declares no INTERNET permission, which can be verified by inspecting the APK's manifest
using tools like `aapt dump permissions` or any APK analyser. Without the INTERNET permission, the
app cannot make network connections (except through Google Play Services for integrity
verification, which is handled by the Play Services process, not Swock itself).

</details>

---

## Usage

<details>
<summary><b>Can I still watch videos?</b></summary>

Yes. The current video is fully visible and playable. You can tap to pause, like, comment, and
share. Only the swipe-to-next gesture is blocked.

</details>

<details>
<summary><b>Can I still navigate within the app?</b></summary>

Yes. Horizontal swipes (tab navigation), taps, long-press, and edge gestures all pass through
normally. You can search, browse profiles, and use all non-feed features of the app.

</details>

<details>
<summary><b>What if I want to swipe to the next video?</b></summary>

You can:
1. Toggle **Swipe Blocking** off in the Swock app
2. Disable the Swock accessibility service in Android Settings
3. Toggle off the specific app in Swock's Protected Apps list

Swock is designed to add friction, not to be unbreakable. The goal is to make the swipe a
conscious choice rather than a reflex. If you deliberately decide to swipe, that's a success.

</details>

<details>
<summary><b>Does Swock work in multi-window mode?</b></summary>

Swock only activates in the active/focused window pane in split-screen mode.

</details>

<details>
<summary><b>Does Swock work with TalkBack?</b></summary>

Swock is compatible with TalkBack. If you experience any issues, please
[report them](https://github.com/Made-in-Jurgistan/swock-public/issues).

</details>

<details>
<summary><b>How do I know Swock is active?</b></summary>

A small shield indicator badge appears at the top of the screen when Swock is actively blocking
swipes on a Shorts/Reels feed. When you leave the feed or close the app, the indicator disappears
automatically.

</details>

<details>
<summary><b>Can I disable Swock for specific apps?</b></summary>

Yes. In Swock's settings, toggle individual apps on or off under **Protected Apps**.

</details>

<details>
<summary><b>What happens if I uninstall Swock?</b></summary>

The accessibility service is removed, and all blocking stops immediately. Your preferences are
deleted with the app. No data remains anywhere because Swock never collected any.

</details>

---

## Technical

<details>
<summary><b>Why does Swock need Android 13+?</b></summary>

Swock uses a touch interception API introduced in Android 13 (API 33). There is no fallback for
older Android versions.

</details>

<details>
<summary><b>Does Swock require root?</b></summary>

No. Swock uses Android's built-in accessibility service framework. No root, no VPN, no special
permissions beyond the accessibility service.

</details>

<details>
<summary><b>Does Swock drain my battery?</b></summary>

No. Swock only activates when a supported app is in the foreground and you're on a Shorts/Reels
feed. When you're using any other app, Swock is idle and uses negligible resources.

</details>

<details>
<summary><b>Will Swock work after app updates?</b></summary>

Swock operates at the touch gesture level, not the view hierarchy level, so touch interception
continues to work even when apps update their UI. Screen detection may occasionally need updates
if apps significantly change their interface — these are handled in Swock updates.

</details>

<details>
<summary><b>Does Swock work on emulators?</b></summary>

Touch interception requires a physical Android 13+ device. Emulators do not reliably support the
touch interception API that Swock uses.

</details>

<details>
<summary><b>Is the APK available for sideloading?</b></summary>

Yes. Swock can be sideloaded. Download the latest APK from
[GitHub Releases](https://github.com/Made-in-Jurgistan/swock-public/releases) and install it with
`adb install swock-v1.0.0-debug.apk`. Enable the accessibility service after installation.

</details>

---

## Supported apps

<details>
<summary><b>Which apps are supported?</b></summary>

See the [README](README.md#supported-apps) for the full list. Swock supports 14 apps and variants
including TikTok, YouTube, Instagram, Snapchat, Facebook, Reddit, Twitch, Xiaohongshu, and Kwai.

</details>

<details>
<summary><b>Can I request support for a new app?</b></summary>

Yes. [Open an issue](https://github.com/Made-in-Jurgistan/swock-public/issues) with the app name
and package name. We'll evaluate whether detection is feasible.

</details>

<details>
<summary><b>Why isn't [app X] supported?</b></summary>

Some apps don't have a clear enough screen structure to reliably detect when the user is on a
short-video feed. If an app's Shorts/Reels feed can't be distinguished from its other screens,
Swock can't target it without blocking swipes everywhere in the app, which would defeat the
purpose. [Request it](https://github.com/Made-in-Jurgistan/swock-public/issues) and we'll
investigate.

</details>

---

## Accessibility service

<details>
<summary><b>Why does Swock need the accessibility service?</b></summary>

The accessibility service is the only Android framework that allows intercepting touch gestures at
the system level without root. Swock uses it to detect when you're on a Shorts/Reels feed and to
block the vertical swipe gesture.

</details>

<details>
<summary><b>Is it safe to give Swock the accessibility permission?</b></summary>

Yes. The accessibility service is a powerful permission, but Swock uses it for a narrow purpose:
detecting Shorts/Reels feeds and intercepting the vertical swipe gesture. Swock has no INTERNET
permission, so even if it could read screen content (which it doesn't store or transmit), it
couldn't send it anywhere.

</details>

<details>
<summary><b>Can Swock read my passwords or personal information?</b></summary>

The accessibility service technically has access to screen content, but Swock only uses it to
classify whether the current screen is a Shorts/Reels feed. It does not read, log, store, or
transmit text content, credentials, or personal data. And since Swock has no INTERNET permission,
it couldn't transmit anything even if it wanted to.

</details>

<details>
<summary><b>Android says Swock has full access to my screen. Is that dangerous?</b></summary>

Android displays this warning for all accessibility services because the framework is powerful.
The warning is generic — it doesn't mean Swock actually reads your screen content. Swock uses the
service only for screen classification and gesture interception. Combined with the fact that Swock
has no internet access, the risk is minimal.

</details>

---

## Comparison & alternatives

<details>
<summary><b>How is Swock different from screen time apps like Digital Wellbeing?</b></summary>

Screen time tools like Google's Digital Wellbeing set daily app timers — when the timer runs out,
the app is paused. But until then, the swipe loop runs at full speed, and 30 minutes of compulsive
swiping has already impaired cognitive flexibility. Swock doesn't limit *how long* you use an app —
it blocks the specific gesture driving the compulsion, in real time.

</details>

<details>
<summary><b>How is Swock different from app blockers like Opal, AppBlock, or Freedom?</b></summary>

App blockers (Opal, AppBlock, Freedom) block entire apps — you can't open TikTok at all during a
block session. This is all-or-nothing: either full access or no access. Users often compensate by
switching to another app, so the compulsive behaviour migrates rather than resolves.

Swock blocks a single gesture — the swipe-to-next-video — while leaving the app fully functional.
You can open TikTok, watch the video in front of you, like, comment, and share. You just can't
swipe to the next video.

AppBlock on Android can block specific sections (Reels, Shorts) inside apps — the closest
competitor to Swock. But it blocks the *section*, not the *gesture*. You still can't use Reels at
all, even to watch a single video intentionally.

</details>

<details>
<summary><b>How is Swock different from One Sec?</b></summary>

One Sec adds a breathing exercise or mindful task before you open a distracting app, creating
friction at the point of *opening*. But once you're inside the app, the swipe loop runs
uninterrupted. Swock adds friction *inside* the app, at the exact gesture where the compulsion
operates — the swipe to the next video.

</details>

<details>
<summary><b>How is Swock different from just using willpower?</b></summary>

Willpower fails under stress, fatigue, and boredom — exactly the states where compulsive scrolling
is strongest. Swock provides structural friction that doesn't depend on willpower. You don't have
to decide not to swipe; Swock makes the swipe impossible. If you want to swipe, you have to
consciously disable Swock first, which breaks the automatic loop.

</details>

<details>
<summary><b>Can I use Swock alongside other digital wellbeing tools?</b></summary>

Yes. Swock is compatible with screen time apps, app blockers, and other wellbeing tools. Swock
complements them by adding gesture-level friction that other tools don't provide.

</details>

---

<div align="center">

<sub>© 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
