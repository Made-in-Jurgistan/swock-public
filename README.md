<div align="center">

<img src="swock_logo.png" width="96" alt="Swock">

# Swock

**Block swipe-to-next-video in short-form video apps.**

Videos stay fully visible and playable — only the vertical swipe gesture is intercepted.

[![Platform](https://img.shields.io/badge/platform-Android-3DDC84?logo=android&logoColor=white)](https://www.android.com)
[![Min SDK](https://img.shields.io/badge/min%20SDK-33%20(Android%2013)-blue)](https://developer.android.com/about/versions/tiramisu)
[![License](https://img.shields.io/badge/license-Proprietary-red)](#license)
[![Privacy](https://img.shields.io/badge/privacy-no%20data%20collection-0047AB)](privacy-policy.md)

</div>

---

## Contents

- [Why Swock?](#why-swock)
- [Features](#features)
- [Supported apps](#supported-apps)
- [How to use](#how-to-use)
- [Privacy](#privacy)
- [FAQ](#faq)
- [Changelog](#changelog)
- [Security](#security)
- [Support](#support)
- [License](#license)
- [Research](#research)

---

## Why Swock?

Short-form video apps are engineered around a single mechanic: **the swipe**. Each upward flick
delivers a new, algorithmically-selected video on a *variable-ratio reward schedule* — the same
reinforcement pattern that makes slot machines compulsive. You never know if the next swipe pays
off, so you keep pulling the lever.

This isn't a willpower failure — it's the intended outcome of the design. The measured costs:

- **Attention & cognition** — A 2025 meta-analysis of 71 studies (N = 98,299) in *Psychological
  Bulletin* found heavier short-form video use is associated with poorer cognition overall
  (r = -.34), with the largest deficits in **attention (r = -.38)** and **inhibitory control
  (r = -.41)** ([Nguyen et al., 2025](https://doi.org/10.1037/bul0005001)).
- **Mental health** — Meta-analyses link short-form video addiction to depression
  ([r = .39](https://doi.org/10.3389/fpubh.2023.1156720)), anxiety, sleep disturbance, and
  social isolation ([Fan et al., 2025](https://doi.org/10.3389/fpsyg.2025.1622175)).
- **It's reversible** — In an experimental study, just **five days** of short-video restriction
  improved selective attention and measurably reduced activity in the brain's default-mode and
  visual networks ([Wang et al., 2025, *NeuroImage*](https://doi.org/10.1016/j.neuroimage.2025.121029)).

**The solution: friction at the exact point of compulsion.** Swock doesn't block apps, videos,
or features — it blocks the *swipe-to-next gesture* and nothing else. You can still open TikTok,
watch the video in front of you, like it, comment, share. What you can't do is pull the lever
again. The reward loop is broken; intentional use is preserved.

No root. No VPN. No network traffic. No data collection.

## Features

| Feature | Description |
|:--------|:------------|
| Videos stay visible | Watch, pause, like, and comment normally |
| Vertical swipes blocked | Can't swipe to the next or previous short |
| Taps pass through | Play/pause, like, share, comment buttons all work |
| Horizontal swipes pass through | Navigation within the app still works |
| Long-press passes through | Context menus and video info pop-ups preserved |
| Edge swipes pass through | System back gesture works from screen edges |
| Multi-touch passes through | Pinch-to-zoom and multi-finger gestures unaffected |
| Zero data collection | Everything runs locally — no network, no analytics, no telemetry |
| Per-app control | Choose exactly which apps to protect |
| Visual indicator | A small shield badge shows when blocking is active |
| No root required | Uses Android's built-in accessibility framework |

## Supported apps

| App | Package |
|:-----|:--------|
| TikTok | `com.zhiliaoapp.musically` |
| TikTok Lite | `com.zhiliaoapp.musically.go` |
| TikTok (Aweme) | `com.ss.android.ugc.aweme` |
| Douyin Lite | `com.ss.android.ugc.aweme.lite` |
| YouTube (Shorts) | `com.google.android.youtube` |
| YouTube TV | `com.google.android.youtube.tv` |
| Instagram (Reels) | `com.instagram.android` |
| Snapchat (Spotlight) | `com.snapchat.android` |
| Facebook (Reels) | `com.facebook.katana` |
| Facebook Lite | `com.facebook.lite` |
| Reddit | `com.reddit.frontpage` |
| Twitch (Clips) | `tv.twitch.android.app` |
| Xiaohongshu (RED) | `com.xiaohongshu` |
| Kwai | `com.kwai.video` |

Individual apps can be toggled on or off in the settings. To request support for a new app,
[open an issue](https://github.com/Made-in-Jurgistan/swock-public/issues).

## How to use

### Install

Download Swock from the Google Play Store (coming soon) or sideload the APK.

### Set up

1. Open **Swock**
2. Tap **Enable Accessibility** → find Swock in the list → toggle on
3. Toggle **Swipe Blocking** on
4. Select which apps to protect (TikTok, YouTube, Instagram, etc.)

### Use it

1. Open TikTok, YouTube, Instagram, or any supported app
2. A small shield indicator appears at the top of the screen
3. Watch the current video — tap to pause, like, comment
4. Try to swipe up → **nothing happens** (the gesture is blocked)
5. Close the app → indicator disappears automatically

### What's not blocked

- Watch the current video — fully visible and playable
- Tap to pause, like, comment, share
- Navigate within the app (tabs, search, profile)
- System back gesture from screen edges
- Pinch-to-zoom and multi-touch

## Privacy

**Swock collects no data. No network access, no analytics, no telemetry. Everything runs locally
on your device.**

- No INTERNET permission
- No data collection, no analytics, no telemetry
- No external storage access
- All preferences stored locally in app-private storage
- The accessibility service only inspects screen content to classify whether you're on a
  Shorts/Reels feed — it does not read, log, store, or transmit text, credentials, or personal data

See the full [Privacy Policy](privacy-policy.md) for details.

## FAQ

<details>
<summary><b>Does Swock block the app itself?</b></summary>

No. Swock doesn't block apps. It blocks the vertical swipe gesture that advances to the next
video. You can still open the app, watch the current video, like, comment, and share. You just
can't swipe to the next video.
</details>

<details>
<summary><b>Does Swock collect my data?</b></summary>

No. Swock has no INTERNET permission and collects zero data. Everything runs locally on your
device. See the [Privacy Policy](privacy-policy.md) for full details.
</details>

<details>
<summary><b>Does Swock require root?</b></summary>

No. Swock uses Android's built-in accessibility service framework. No root, no VPN, no special
permissions beyond the accessibility service.
</details>

<details>
<summary><b>Why does Swock need the accessibility service?</b></summary>

The accessibility service is the only Android framework that allows intercepting touch gestures
at the system level without root. Swock uses it to detect when you're on a Shorts/Reels feed and
to block the vertical swipe gesture. The service does not read, store, or transmit any personal
data.
</details>

<details>
<summary><b>Will Swock slow down my phone?</b></summary>

No. Swock only activates when a supported app is in the foreground and you're on a Shorts/Reels
feed. When you're using any other app, Swock is idle and uses negligible resources.
</details>

<details>
<summary><b>Can I still watch videos normally?</b></summary>

Yes. The current video is fully visible and playable. You can tap to pause, like, comment, and
share. Only the swipe-to-next gesture is blocked.
</details>

<details>
<summary><b>What if I want to swipe to the next video?</b></summary>

You can temporarily disable Swock by toggling **Swipe Blocking** off in the Swock app, or by
disabling the accessibility service in Android Settings. Swock is designed to add friction, not
to be unbreakable — the goal is to make the swipe a conscious choice rather than a reflex.
</details>

<details>
<summary><b>Does Swock work with TalkBack?</b></summary>

Swock is compatible with TalkBack. If you experience any issues, please
[report them](https://github.com/Made-in-Jurgistan/swock-public/issues).
</details>

<details>
<summary><b>Why does Swock need Android 13+?</b></summary>

Swock uses a touch interception API that was introduced in Android 13 (API 33). There is no
fallback for older versions.
</details>

<details>
<summary><b>Is Swock open source?</b></summary>

No. Swock is proprietary software. The source code is not publicly available. This repository
contains only public-facing documentation — privacy policy, terms of service, FAQ, and support
information.
</details>

<details>
<summary><b>Is Swock a medical treatment for addiction?</b></summary>

No. Swock is a digital wellbeing tool that adds friction to compulsive scrolling. It is not a
medical device, a treatment for addiction, or a substitute for professional help. If you're
struggling with compulsive social media use, consider speaking with a mental health professional.
</details>

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for release notes.

## Security

Swock is designed with a minimal attack surface. See [SECURITY.md](SECURITY.md) for the security
policy and how to report vulnerabilities.

## Support

- Found a bug? [Open an issue](https://github.com/Made-in-Jurgistan/swock-public/issues)
- Want a new app supported? [Request it](https://github.com/Made-in-Jurgistan/swock-public/issues)
- See [SUPPORT.md](SUPPORT.md) for troubleshooting guides

## License

Swock is proprietary software. All rights reserved. See [Terms of Service](terms-of-service.md)
for usage terms.

## Research

Short-form video use is associated with measurable cognitive costs:

- **Nguyen et al. (2025)** — Meta-analysis of 71 studies (N = 98,299): heavier short-form video
  use linked to poorer attention (r = -.38) and inhibitory control (r = -.41).
  [DOI: 10.1037/bul0005001](https://doi.org/10.1037/bul0005001)
- **Fan et al. (2025)** — Short-form video addiction linked to depression (r = .39), anxiety,
  sleep disturbance, and social isolation.
  [DOI: 10.3389/fpsyg.2025.1622175](https://doi.org/10.3389/fpsyg.2025.1622175)
- **Wang et al. (2025)** — Five days of short-video restriction improved selective attention and
  reduced compulsive brain activity.
  [DOI: 10.1016/j.neuroimage.2025.121029](https://doi.org/10.1016/j.neuroimage.2025.121029)

---

<div align="center">

<sub>(c) 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
