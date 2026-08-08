<div align="center">

<img src="swock_logo.png" width="120" alt="Swock">

# Swock

### Break the scroll loop.

**An Android app that blocks the swipe-to-next-video gesture in short-form video apps.**

Videos stay fully visible and playable — only the compulsive swipe is intercepted.

<br>

[![Platform](https://img.shields.io/badge/Platform-Android_13+-3DDC84?logo=android&logoColor=white)](https://www.android.com)
[![Kotlin](https://img.shields.io/badge/Built%20with-Kotlin-7F52FF?logo=kotlin&logoColor=white)](https://kotlinlang.org)
[![UI](https://img.shields.io/badge/UI-Jetpack%20Compose-06B6D4?logo=jetpackcompose&logoColor=white)](https://developer.android.com/jetpack/compose)
[![Privacy](https://img.shields.io/badge/Privacy-Zero%20data%20collection-0047AB)](privacy-policy.md)
[![License](https://img.shields.io/badge/License-Proprietary-red)](terms-of-service.md)

<br>

**[Download on Google Play](https://play.google.com/store/apps/details?id=com.swock)** &nbsp;·&nbsp; [Report an issue](https://github.com/Made-in-Jurgistan/swock-public/issues) &nbsp;·&nbsp; [Read the FAQ](FAQ.md) &nbsp;·&nbsp; [Press kit](PRESS.md)

</div>

<br>

---

## The problem

> *"You never know if the next swipe pays off, so you keep pulling the lever."*

Short-form video apps — TikTok, YouTube Shorts, Instagram Reels — are engineered around a single
mechanic: **the swipe**. Each upward flick delivers a new, algorithmically selected video on a
*variable-ratio reward schedule*. That's the same reinforcement pattern that makes slot machines
compulsive. It's not a design accident. It's the design.

This isn't a willpower failure. It's the intended outcome. And the costs are measurable:

<table>
<tr>
<td width="33%" align="center" valign="top">

### Attention

A 2025 meta-analysis of **71 studies** (N = 98,299) found heavier short-form video use linked to
**poorer attention** (r = -.38) and **inhibitory control** (r = -.41).

<br>

<sub>[Nguyen et al., 2025<br>Psychological Bulletin](https://doi.org/10.1037/bul0000498)</sub>

</td>
<td width="33%" align="center" valign="top">

### Mental health

The same meta-analysis found short-form video use linked to **poorer mental health** (r = -.21),
with **stress** (r = -.34) and **anxiety** (r = -.33) showing the strongest associations.

<br>

<sub>[Nguyen et al., 2025<br>Psychological Bulletin](https://doi.org/10.1037/bul0000498)</sub>

</td>
<td width="33%" align="center" valign="top">

### Reducing access can help

A 2025 randomized controlled trial found that **2 weeks** of blocking mobile internet on
smartphones improved **sustained attention**, mental health, and well-being. **91%** of
participants improved. This study tested total internet blocking, not Swock specifically —
but it suggests that reducing digital access can produce measurable cognitive benefits.

<br>

<sub>[Castelo et al., 2025<br>PNAS Nexus](https://doi.org/10.1093/pnasnexus/pgaf017)</sub>

</td>
</tr>
</table>

---

## The solution

**Friction at the exact point of compulsion.**

Swock doesn't block apps. It doesn't block videos. It doesn't block features. It blocks
**one gesture** — the swipe-to-next-video — and nothing else.

| You can still... | You can't... |
|:-----------------|:-------------|
| Open TikTok, YouTube, Instagram | Swipe to the next video |
| Watch the video in front of you | Pull the lever again |
| Tap to pause, like, comment, share | Fall into the scroll loop |
| Navigate within the app normally | |
| Use the system back gesture | |

The reward loop is broken. Intentional use is preserved.

> **No root. No VPN. No network traffic. No data collection.** Just an accessibility service that
> intercepts one gesture.

---

## Features

<div align="center">

| | | |
|:---:|:---:|:---:|
| **Videos stay visible** | **Vertical swipes blocked** | **Taps pass through** |
| Watch, pause, like, comment | Can't swipe to next or previous short | Play/pause, like, share, comment all work |
| | | |
| **Horizontal swipes pass through** | **Long-press passes through** | **Edge swipes pass through** |
| Navigation within the app works | Context menus and info pop-ups preserved | System back gesture works from edges |
| | | |
| **Multi-touch passes through** | **Per-app control** | **Visual indicator** |
| Pinch-to-zoom unaffected | Choose exactly which apps to protect | Shield badge shows when blocking is active |
| | | |
| **Zero data collection** | **No root required** | **Battery efficient** |
| No network, no analytics, no telemetry | Uses Android's accessibility framework | Only activates on Shorts/Reels feeds |

</div>

---

## How Swock is different

Most digital wellbeing tools take an **all-or-nothing** approach: they block entire apps, set time
limits, or add friction before you open an app. Swock is the only app that targets the **specific
gesture** driving the compulsion — the swipe-to-next-video — while leaving the app fully usable.

| App | Mechanism | What it blocks | Gesture-level? | Platform | Root/VPN? |
|:----|:----------|:---------------|:---------------|:---------|:----------|
| **Swock** | AccessibilityService | Swipe-to-next-video gesture only | **Yes** | Android 13+ | No root, no VPN |
| **Opal** | Screen Time API / AccessibilityService | Entire apps (block lists, schedules, sessions) | No | iOS, macOS, Android | No |
| **One Sec** | Shortcuts Automation / AccessibilityService | App opening (adds breathing delay before app opens) | No | iOS, Android, browser | No |
| **AppBlock** | Screen Time API / AccessibilityService | Entire apps; some in-app sections (Reels/Shorts) on Android | No (section-level on Android) | iOS, Android, browser | No |
| **Freedom** | Local VPN | Entire apps + websites (network-level blocking) | No | Mac, Windows, iOS, Android, Chrome | Local VPN |
| **Digital Wellbeing** | Built-in Android | App timers (pauses app after time limit) | No | Android | No |

### Why gesture-level blocking matters

App blockers and screen time tools address **how long** or **whether** you use an app. Swock
addresses **how** you use it. The research is clear: the swipe gesture itself — not the content, not
the app, not the time spent — is what drives the compulsive loop ([Luo et al., 2025](https://doi.org/10.3390/bs15081070);
[Ma & Jiang, 2024](https://doi.org/10.5817/CP2024-3-1)).

- **App blockers** (Opal, AppBlock, Freedom) remove access entirely. You can't open TikTok at all.
  But users compensate by switching to another app or finding workarounds — the compulsive behaviour
  migrates, it doesn't resolve.
- **One Sec** adds a breathing exercise before you open an app. This creates friction at the point
  of *opening*, but once you're in, the swipe loop runs uninterrupted.
- **Digital Wellbeing** sets time limits. When the timer runs out, the app pauses. But until then,
  the swipe loop runs at full speed — and a 30-minute session of compulsive swiping has already
  impaired cognitive flexibility ([Luo et al., 2025](https://doi.org/10.3390/bs15081070)).
- **AppBlock** on Android can block specific sections (Reels, Shorts) inside apps — the closest
  competitor to Swock. But it blocks the *section*, not the *gesture*. You still can't use Reels at
  all, even to watch a single video intentionally.

**Swock is different.** You open TikTok. You watch the video in front of you. You can like, comment,
share, pause. The app is fully functional. The only thing you can't do is swipe to the next video.
The reward loop is broken at the exact point of compulsion — not at the app level, not at the time
level, but at the gesture level.

---

## Supported apps

<div align="center">

| App | Feature | App | Feature |
|:----|:--------|:----|:--------|
| TikTok | For You / Following | Reddit | Video feed |
| TikTok Lite | For You / Following | Twitch | Clips |
| TikTok (Aweme) | For You / Following | Xiaohongshu (RED) | Video feed |
| YouTube | Shorts | Kwai | Video feed |
| YouTube TV | Shorts | Instagram | Reels |
| Snapchat | Spotlight | Facebook | Reels |
| Facebook Lite | Reels | Douyin Lite | For You |

</div>

Individual apps can be toggled on or off in the settings. To request support for a new app,
[open an issue](https://github.com/Made-in-Jurgistan/swock-public/issues).

---

## Quick start

### 1. Install

Download Swock from the [Google Play Store](https://play.google.com/store/apps/details?id=com.swock).

### 2. Enable

1. Open **Swock**
2. Tap **Enable Accessibility** → find Swock in the list → toggle on
3. Toggle **Swipe Blocking** on
4. Select which apps to protect

### 3. Use

1. Open TikTok, YouTube, Instagram, or any supported app
2. A **shield indicator** appears at the top of the screen
3. Watch the current video — tap to pause, like, comment
4. Try to swipe up → **nothing happens**
5. Close the app → indicator disappears automatically

> **Requirements**: Android 13 (API 33) or higher. Physical device recommended (emulators do not
> reliably support touch interception).

---

## Privacy

<div align="center">

### Swock collects no data.

**No network access. No analytics. No telemetry. Everything runs locally on your device.**

</div>

| Principle | Detail |
|:----------|:-------|
| No INTERNET permission | Swock cannot connect to any server |
| No data collection | No personal info, no device IDs, no usage analytics, no crash reports |
| No external storage | All preferences stored in app-private storage |
| No data transmission | The accessibility service inspects screen structure locally to classify screens — it never reads, logs, stores, or transmits text, credentials, or personal data |
| Open privacy policy | Read the full [Privacy Policy](privacy-policy.md) |

The only network activity is through Google Play Services for app integrity verification (Play
Integrity API), which sends a random nonce and package name to Google. See the
[Privacy Policy](privacy-policy.md) for full details.

---

## FAQ

<details>
<summary><b>How is Swock different from app blockers like Opal, AppBlock, or Freedom?</b></summary>
<br>

App blockers (Opal, AppBlock, Freedom) block entire apps — you can't open TikTok at all during a
block session. This is an all-or-nothing approach: either you have full access or no access. Users
often compensate by switching to another app, so the compulsive behaviour migrates rather than
resolves.

Swock blocks a single gesture — the swipe-to-next-video — while leaving the app fully functional.
You can open TikTok, watch the video in front of you, like, comment, and share. You just can't
swipe to the next video. The reward loop is broken at the gesture level, not the app level.

One Sec is closer in spirit — it adds friction (a breathing exercise) before you open an app. But
once you're in, the swipe loop runs uninterrupted. Swock adds friction *inside* the app, at the
exact point where the compulsion operates.

</details>

<details>
<summary><b>Does Swock block the app itself?</b></summary>
<br>

No. Swock doesn't block apps. It blocks the vertical swipe gesture that advances to the next
video. You can still open the app, watch the current video, like, comment, and share. You just
can't swipe to the next video.

</details>

<details>
<summary><b>Does Swock collect my data?</b></summary>
<br>

No. Swock has no INTERNET permission and collects zero data. Everything runs locally on your
device. See the [Privacy Policy](privacy-policy.md) for full details.

</details>

<details>
<summary><b>Does Swock require root?</b></summary>
<br>

No. Swock uses Android's built-in accessibility service framework. No root, no VPN, no special
permissions beyond the accessibility service.

</details>

<details>
<summary><b>Can I still watch videos normally?</b></summary>
<br>

Yes. The current video is fully visible and playable. You can tap to pause, like, comment, and
share. Only the swipe-to-next gesture is blocked.

</details>

<details>
<summary><b>What if I want to swipe to the next video?</b></summary>
<br>

You can temporarily disable Swock by toggling **Swipe Blocking** off in the Swock app, or by
disabling the accessibility service in Android Settings. Swock is designed to add friction, not
to be unbreakable — the goal is to make the swipe a conscious choice rather than a reflex.

</details>

<details>
<summary><b>Is Swock a medical treatment for addiction?</b></summary>
<br>

No. Swock is a digital wellbeing tool that adds friction to compulsive scrolling. It is not a
medical device, a treatment for addiction, or a substitute for professional help. If you're
struggling with compulsive social media use, consider speaking with a mental health professional.

</details>

> **See the [full FAQ](FAQ.md) for all questions.**

---

## For the press

Journalists, reviewers, and content creators — see the **[Press Kit](PRESS.md)** for:

- One-line and paragraph-length descriptions of Swock
- Key statistics and research citations
- Company boilerplate
- Media contact
- Logo and brand assets

---

## Documentation

| Document | Description |
|:---------|:------------|
| [FAQ](FAQ.md) | Frequently asked questions, organized by category |
| [Support](SUPPORT.md) | Troubleshooting guides and bug reporting |
| [Changelog](CHANGELOG.md) | Release notes for each version |
| [Security](SECURITY.md) | Security policy and vulnerability reporting |
| [Privacy Policy](privacy-policy.md) | Full privacy policy |
| [Terms of Service](terms-of-service.md) | App usage terms and conditions |
| [Press Kit](PRESS.md) | Resources for journalists and reviewers |

---

## Research

Short-form video use is associated with measurable cognitive and mental health costs. The
following peer-reviewed studies informed Swock's design. **None of these studies tested Swock
itself** — they establish the problem, the mechanism (the swipe gesture, not the content), and the
general principle that reducing digital access can help.

### The problem: short-form video use is associated with cognitive and mental health costs

1. **Nguyen, L., et al. (2025)**. "Feeds, feelings, and focus: A systematic review and
   meta-analysis examining the cognitive and mental health correlates of short-form video use."
   *Psychological Bulletin*, 151(9), 1125–1146. N = 98,299 across 71 studies. Found heavier use
   linked to poorer cognition (r = -.34), with attention (r = -.38) and inhibitory control
   (r = -.41) showing the strongest associations. Also found poorer mental health (r = -.21),
   with stress (r = -.34) and anxiety (r = -.33) showing the strongest associations.
   [DOI: 10.1037/bul0000498](https://doi.org/10.1037/bul0000498)

### The mechanism: the swipe gesture itself — not the content — drives the compulsion

2. **Luo, W., et al. (2025)**. "Swiping disrupts switching: Preliminary evidence for reduced
   cue-based preparation following short-form video exposure." *Behavioral Sciences*, 15(8),
   1070. A randomized experiment (N = 72) found that 30 minutes of TikTok-style swiping
   selectively disrupted proactive cognitive flexibility — the ability to prepare for upcoming
   tasks. The documentary control group (same content duration, no swiping) showed no deficit.
   The authors summarize this as "swiping disrupts switching": the gesture itself impairs
   goal-directed cognitive control.
   [DOI: 10.3390/bs15081070](https://doi.org/10.3390/bs15081070)

3. **Ma, L., & Jiang, Q. (2024)**. "Swiping more, thinking less: Using TikTok hinders analytic
   thinking." *Cyberpsychology*, 18(3), Article 1. Two experiments found that **the process of
   swiping through short video feeds — rather than the video content itself — negatively
   influenced users' propensity to think analytically**. Swiping shifts users toward fast,
   automatic processing (Type 1) at the expense of deliberate analytic reasoning (Type 2).
   [DOI: 10.5817/CP2024-3-1](https://doi.org/10.5817/CP2024-3-1)

4. **Park, J., & Jung, Y. (2024)**. "Unveiling the dynamics of binge-scrolling: A comprehensive
   analysis of short-form video consumption using a Stimulus-Organism-Response model."
   *Telematics and Informatics*, 95, 102200. A mixed-method study found that the **infinite
   scrolling feature** — not content quality — drives perceived loss of self-control in
   short-form video users. The scrolling interaction itself mediates the relationship between
   platform design and negative outcomes.
   [DOI: 10.1016/j.tele.2024.102200](https://doi.org/10.1016/j.tele.2024.102200)

5. **Clark, L., & Zack, M. (2023)**. "Engineered highs: Reward variability and frequency as
   potential prerequisites of behavioural addiction." *Addictive Behaviors*, 140, 107626. Shows
   that infinite scroll and personalised recommendations introduce **novel forms of reward
   variability** — the same variable-ratio reinforcement schedule that drives gambling
   addiction. The swipe-to-next-video mechanic is the delivery mechanism for this variability.
   [DOI: 10.1016/j.addbeh.2023.107626](https://doi.org/10.1016/j.addbeh.2023.107626)

### Evidence that friction and limiting swipes can help

6. **Ruiz, N., et al. (2024)**. "Design frictions on social media: Balancing reduced mindless
   scrolling and user satisfaction." *Proceedings of Mensch und Computer 2024*, 442–447. A study
   (N = 30) compared infinite scroll with an interface that added **friction** — requiring users
   to react to each post before accessing the next. The friction interface produced
   **significantly better content recall** and reduced mindless scrolling. This directly
   supports Swock's approach of adding friction at the gesture level.
   [DOI: 10.1145/3670653.3677495](https://doi.org/10.1145/3670653.3677495)

7. **Barton, N., & Smyth, M. (2025)**. "Context-switching in short-form videos: What is the
   impact on prospective memory?" *Memory*, 33(7), 788–801. A between-groups experiment
   (N = 45) found that **unlimited context-switching** (free swiping between videos) **degraded
   prospective memory**, while **limited context-switching improved it**. Limiting the ability
   to swipe to the next video has a measurable cognitive benefit.
   [DOI: 10.1080/09658211.2025.2521076](https://doi.org/10.1080/09658211.2025.2521076)

### Evidence that reducing access can help

8. **Castelo, N., et al. (2025)**. "Blocking mobile internet on smartphones improves sustained
   attention, mental health, and subjective well-being." *PNAS Nexus*, 4(2), pgaf017. A
   randomized controlled trial found that 2 weeks of blocking **all mobile internet** on
   smartphones improved sustained attention, mental health, and well-being; 91% of participants
   improved on at least one outcome. This was a blanket internet block, not a targeted
   swipe-blocking intervention — but it demonstrates that reducing digital access can produce
   measurable cognitive benefits.
   [DOI: 10.1093/pnasnexus/pgaf017](https://doi.org/10.1093/pnasnexus/pgaf017)

---

## About

**Swock** is developed by [Made in Jurgistan](https://github.com/Made-in-Jurgistan), an
independent software studio building digital wellbeing tools that respect privacy.

Swock is proprietary software. All rights reserved. See the [Terms of Service](terms-of-service.md)
for usage terms.

---

<div align="center">

<sub>© 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
