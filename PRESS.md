<div align="center">

<img src="swock_logo.png" width="80" alt="Swock app logo — shield icon">
<br>
<img src="swock_wordmark.jpg" width="320" alt="Swock wordmark">

# Press Kit

**An Android app that breaks the scroll loop by blocking a single gesture.**

</div>

---

## Contents

- [Fact sheet](#fact-sheet)
- [One-line description](#one-line-description)
- [Short description](#short-description)
- [Full description](#full-description)
- [Company boilerplate](#company-boilerplate)
- [Key statistics](#key-statistics)
- [Research citations](#research-citations)
- [How Swock works (non-technical)](#how-swock-works-non-technical)
- [What makes Swock different](#what-makes-swock-different)
- [Privacy at a glance](#privacy-at-a-glance)
- [Frequently asked press questions](#frequently-asked-press-questions)
- [Brand assets](#brand-assets)
- [Media contact](#media-contact)
- [Coverage guidelines](#coverage-guidelines)

---

## Fact sheet

| Field | Value |
|:------|:------|
| **Product name** | Swock |
| **Tagline** | Break the scroll loop |
| **Category** | Digital wellbeing / Tools |
| **Platform** | Android 13+ (API 33+) |
| **Developer** | Made in Jurgistan |
| **Release date** | August 2026 |
| **Version** | 1.0.0 |
| **License** | Proprietary (All Rights Reserved) |
| **Open source** | No |
| **Price** | Free |
| **Ads** | No |
| **In-app purchases** | No |
| **Data collection** | None |
| **Network access** | None (no INTERNET permission) |
| **Root required** | No |
| **Download** | [Google Play](https://play.google.com/store/apps/details?id=com.swock) · [APK releases](https://github.com/Made-in-Jurgistan/swock-public/releases) |
| **Website** | [github.com/Made-in-Jurgistan/swock-public](https://github.com/Made-in-Jurgistan/swock-public) |

---

## One-line description

> Swock is an Android app that blocks the swipe-to-next-video gesture in short-form video apps,
> breaking the compulsive scroll loop without blocking the apps themselves.

---

## Short description

> Swock breaks the scroll loop. Short-form video apps like TikTok, YouTube Shorts, and Instagram
> Reels are engineered around a single mechanic — the swipe — which delivers new content on a
> variable-ratio reward schedule, the same pattern that makes slot machines compulsive. Swock
> blocks that one gesture and nothing else. Videos stay fully visible and playable. You can still
> open the app, watch, like, comment, and share. You just can't pull the lever again. No root, no
> VPN, no data collection.

---

## Full description

Swock is an Android digital wellbeing app that addresses compulsive short-form video consumption
by targeting the specific gesture that drives it: the vertical swipe.

Short-form video platforms — TikTok, YouTube Shorts, Instagram Reels, and others — are designed
around a variable-ratio reward schedule. Each swipe delivers a new, algorithmically selected video,
and the unpredictability of the reward keeps users swiping in a pattern that closely resembles
slot machine behaviour. This is not a side effect; it is the core engagement mechanic.

Existing solutions fall short. **Screen time tools** like Digital Wellbeing set time limits, but
until the timer expires, the swipe loop runs at full speed — and 30 minutes of compulsive swiping
has already impaired cognitive flexibility ([Luo et al., 2025](https://doi.org/10.3390/bs15081070)).
**App blockers** like Opal and Freedom remove access to the app entirely — you can't open TikTok at
all during a block session. This all-or-nothing approach leads to substitution (switching to
another app) rather than behaviour change. **One Sec** adds a breathing exercise before you open an
app, creating friction at the point of *opening* — but once you're in, the swipe loop runs
uninterrupted. **AppBlock** on Android is the closest competitor: it can block specific sections
(Reels, Shorts) inside apps. But it blocks the *section*, not the *gesture* — you still can't use
Reels at all, even to watch a single video intentionally.

Swock takes a different approach: **friction at the exact point of compulsion**. It uses Android's
accessibility service framework to detect when a user is on a short-video feed and intercept the
vertical swipe gesture. The app itself remains fully functional — videos play, taps work,
horizontal navigation works, liking and commenting work. Only the swipe-to-next gesture is blocked.

The result is that the reward loop is broken while intentional use is preserved. Users can still
watch a video they chose to watch. They just can't reflexively swipe to the next one.

Swock collects no data. It has no INTERNET permission, no analytics, no telemetry, and no crash
reporting. Everything runs locally on the device. The app requires no root access and uses only
Android's built-in accessibility framework.

---

## Company boilerplate

> **Made in Jurgistan** is an independent software studio building digital wellbeing tools that
> respect user privacy. The studio's products are characterised by zero data collection, minimal
> permissions, and a focus on structural behaviour change rather than surveillance or nagging.
> Swock is the studio's first public release.

---

## Key statistics

### The problem

| Statistic | Source |
|:----------|:-------|
| **71 studies** meta-analysed (N = 98,299) showing short-form video use linked to poorer cognition | [Nguyen et al., 2025](https://doi.org/10.1037/bul0000498) |
| **r = -.38** correlation between short-form video use and attention deficits | [Nguyen et al., 2025](https://doi.org/10.1037/bul0000498) |
| **r = -.41** correlation between short-form video use and inhibitory control deficits | [Nguyen et al., 2025](https://doi.org/10.1037/bul0000498) |
| **r = -.34** correlation between short-form video use and stress | [Nguyen et al., 2025](https://doi.org/10.1037/bul0000498) |
| **r = -.33** correlation between short-form video use and anxiety | [Nguyen et al., 2025](https://doi.org/10.1037/bul0000498) |

### The mechanism: the swipe gesture, not the content

| Statistic | Source |
|:----------|:-------|
| **30 min** of TikTok-style swiping disrupted cognitive flexibility; documentary control group (no swiping) showed no deficit. "Swiping disrupts switching." | [Luo et al., 2025](https://doi.org/10.3390/bs15081070) |
| **"The process of swiping... rather than the video content itself, negatively influenced users' propensity to think analytically"** | [Ma & Jiang, 2024](https://doi.org/10.5817/CP2024-3-1) |
| **Infinite scrolling feature** — not content quality — drives perceived loss of self-control in short-form video users | [Park & Jung, 2024](https://doi.org/10.1016/j.tele.2024.102200) |
| Swipe-to-next-video operates on a **variable-ratio reward schedule**, the same reinforcement pattern as gambling addiction | [Clark & Zack, 2023](https://doi.org/10.1016/j.addbeh.2023.107626) |

### Evidence that friction and limiting swipes can help

| Statistic | Source |
|:----------|:-------|
| Adding **friction** to scrolling (requiring reaction before next post) produced **significantly better content recall** vs. infinite scroll | [Ruiz et al., 2024](https://doi.org/10.1145/3670653.3677495) |
| **Limiting context-switching** (limiting swipes to next video) **improved prospective memory**; unlimited switching degraded it | [Barton & Smyth, 2025](https://doi.org/10.1080/09658211.2025.2521076) |

### Evidence that reducing access can help

| Statistic | Source |
|:----------|:-------|
| **2 weeks** of blocking all mobile internet improved sustained attention; 91% of participants improved. This tested total internet blocking, not Swock. | [Castelo et al., 2025](https://doi.org/10.1093/pnasnexus/pgaf017) |

### The product

| Statistic | Value |
|:----------|:------|
| **Supported apps** | 14 (TikTok, YouTube, Instagram, Snapchat, Facebook, Reddit, Twitch, Xiaohongshu, Kwai, and variants) |
| **Data collected** | 0 bytes |
| **Permissions requested** | 1 (Accessibility Service) |
| **Network permissions** | 0 |
| **Root required** | No |
| **Minimum Android version** | 13 (API 33) |
| **App size** | ~62 MB (debug build); release build smaller with R8 shrinking |

---

## Research citations

> **Note:** These studies informed Swock's design. None tested Swock itself. They establish the
> problem (Nguyen), the mechanism — the swipe gesture, not the content (Luo, Ma & Jiang, Park,
> Clark & Zack) — the principle that friction and limiting swipes can help (Ruiz, Barton & Smyth) —
> and the general principle that reducing digital access can help (Castelo).

### Nguyen, L., et al. (2025)

> "Feeds, feelings, and focus: A systematic review and meta-analysis examining the cognitive and
> mental health correlates of short-form video use."
> *Psychological Bulletin*, 151(9), 1125–1146.

Meta-analysis of 71 studies with a combined sample of 98,299 participants. Found that heavier
short-form video use is associated with poorer cognition overall (r = -.34), with the largest
deficits in attention (r = -.38) and inhibitory control (r = -.41). Also found poorer mental
health (r = -.21), with stress (r = -.34) and anxiety (r = -.33) showing the strongest
associations. This is correlational evidence — it establishes the problem but does not prove that
reducing use improves outcomes.

DOI: [10.1037/bul0000498](https://doi.org/10.1037/bul0000498)

### Luo, W., et al. (2025)

> "Swiping disrupts switching: Preliminary evidence for reduced cue-based preparation following
> short-form video exposure."
> *Behavioral Sciences*, 15(8), 1070.

A randomized experiment (N = 72) in which participants viewed either 30 minutes of TikTok-style
content, a neutral documentary, or no video. The short-form video group showed selective
disruption of proactive cognitive flexibility — the ability to prepare for upcoming tasks. The
documentary group (same content duration, no swiping) showed no deficit. The authors call this
"swiping disrupts switching": the **gesture itself** impairs goal-directed cognitive control,
independent of the content being watched.

DOI: [10.3390/bs15081070](https://doi.org/10.3390/bs15081070)

### Ma, L., & Jiang, Q. (2024)

> "Swiping more, thinking less: Using TikTok hinders analytic thinking."
> *Cyberpsychology: Journal of Psychosocial Research on Cyberspace*, 18(3), Article 1.

Two experiments using dual-process theory found that **the process of swiping through short video
feeds — rather than the video content itself — negatively influenced users' propensity to think
analytically**. Swiping shifts users toward fast, automatic Type 1 processing at the expense of
deliberate Type 2 analytic reasoning, impairing judgment and decision-making.

DOI: [10.5817/CP2024-3-1](https://doi.org/10.5817/CP2024-3-1)

### Park, J., & Jung, Y. (2024)

> "Unveiling the dynamics of binge-scrolling: A comprehensive analysis of short-form video
> consumption using a Stimulus-Organism-Response model."
> *Telematics and Informatics*, 95, 102200.

A mixed-method study found that the **infinite scrolling feature** — not content quality — drives
perceived loss of self-control in short-form video users. The scrolling interaction itself
mediates the relationship between platform design and negative outcomes, including regret and
diminished cognitive engagement.

DOI: [10.1016/j.tele.2024.102200](https://doi.org/10.1016/j.tele.2024.102200)

### Clark, L., & Zack, M. (2023)

> "Engineered highs: Reward variability and frequency as potential prerequisites of behavioural
> addiction."
> *Addictive Behaviors*, 140, 107626.

Shows that infinite scroll and personalised recommendations introduce **novel forms of reward
variability** — the same variable-ratio reinforcement schedule that drives gambling addiction.
The swipe-to-next-video mechanic is the delivery mechanism for this variability, creating
unpredictable rewards that exploit dopaminergic signalling.

DOI: [10.1016/j.addbeh.2023.107626](https://doi.org/10.1016/j.addbeh.2023.107626)

### Ruiz, N., et al. (2024)

> "Design frictions on social media: Balancing reduced mindless scrolling and user satisfaction."
> *Proceedings of Mensch und Computer 2024*, 442–447.

A study (N = 30) compared infinite scroll with an interface that added **friction** — requiring
users to react to each post before accessing the next. The friction interface produced
**significantly better content recall** and reduced mindless scrolling, drawing on the concept of
"microboundaries" — small moments of friction that interrupt automatic, mindless interactions.
This directly supports Swock's approach of adding friction at the gesture level.

DOI: [10.1145/3670653.3677495](https://doi.org/10.1145/3670653.3677495)

### Barton, N., & Smyth, M. (2025)

> "Context-switching in short-form videos: What is the impact on prospective memory?"
> *Memory*, 33(7), 788–801.

A between-groups experiment (N = 45) with three conditions: unlimited context-switching (free
swiping), limited context-switching, and control. **Unlimited switching degraded prospective
memory**; **limited switching improved it**. The pace of context-switching — how fast users swipe
to the next video — is identified as the underlying factor behind cognitive decline. Limiting
the ability to swipe has a measurable cognitive benefit.

DOI: [10.1080/09658211.2025.2521076](https://doi.org/10.1080/09658211.2025.2521076)

### Castelo, N., et al. (2025)

> "Blocking mobile internet on smartphones improves sustained attention, mental health, and
> subjective well-being."
> *PNAS Nexus*, 4(2), pgaf017.

A month-long randomized controlled trial in which participants blocked **all mobile internet
access** on their smartphones for 2 weeks. The intervention improved mental health, subjective
well-being, and objectively measured sustained attention; 91% of participants improved on at
least one outcome. This was a blanket internet block — not a targeted swipe-blocking
intervention like Swock. It demonstrates the general principle that reducing digital access can
produce measurable cognitive benefits, but does not prove that Swock produces similar results.

DOI: [10.1093/pnasnexus/pgaf017](https://doi.org/10.1093/pnasnexus/pgaf017)

---

## How Swock works (non-technical)

Swock uses Android's accessibility service — a built-in Android framework designed to help users
with disabilities interact with their devices. When you enable Swock's accessibility service, it
gains the ability to:

1. **Detect** when you're on a short-video feed in a supported app (TikTok's For You page,
   YouTube Shorts, Instagram Reels, etc.)
2. **Intercept** the vertical swipe gesture that would advance to the next video
3. **Allow** all other touches — taps, horizontal swipes, long-press, edge gestures — to pass
   through to the app normally

When you leave the short-video feed (close the app, navigate to a different tab), Swock returns to
an idle state and stops intercepting anything.

A small shield indicator appears at the top of the screen when Swock is actively blocking, so you
always know when the protection is on.

---

## What makes Swock different

| App | Mechanism | What it blocks | Gesture-level? | Limitation |
|:----|:----------|:---------------|:---------------|:-----------|
| **Swock** | AccessibilityService | Swipe-to-next-video gesture only | **Yes** | None — app fully usable minus one gesture |
| **Opal** | Screen Time API / AccessibilityService | Entire apps | No | All-or-nothing; users switch to another app |
| **One Sec** | Shortcuts / AccessibilityService | App opening (breathing delay) | No | Friction only at open; swipe loop runs once inside |
| **AppBlock** | Screen Time API / AccessibilityService | Entire apps; some in-app sections on Android | No | Blocks the section, not the gesture; can't use Reels at all |
| **Freedom** | Local VPN | Entire apps + websites | No | Network-level blocking; requires VPN profile |
| **Digital Wellbeing** | Built-in Android | App timers | No | Time-based; swipe loop runs until timer expires |

Swock is the only app that targets the **specific gesture** driving the compulsion, without
removing access to the app itself. App blockers remove the app entirely. One Sec adds friction
before opening. Digital Wellbeing sets time limits. Swock breaks the loop *at the gesture level* —
you can still open the app, watch a video, like, comment, and share. You just can't pull the lever
again.

---

## Privacy at a glance

| Question | Answer |
|:---------|:-------|
| Does Swock collect personal data? | **No** |
| Does Swock use analytics or telemetry? | **No** |
| Does Swock have internet access? | **No** (no INTERNET permission declared) |
| Does Swock store data in the cloud? | **No** |
| Does Swock read what's on my screen? | It inspects screen structure locally to detect Shorts/Reels feeds. It never reads, logs, stores, or transmits text content, credentials, or personal data. |
| Does Swock sell or share data? | **No** — there is no data to sell or share |
| Where are my settings stored? | Locally on your device, in app-private storage |

Full details: [Privacy Policy](privacy-policy.md)

---

## Frequently asked press questions

**Is Swock anti-TikTok?**

No. Swock is not against any particular platform. It's a tool for people who want to change their
own behaviour. Swock works across 14 apps — TikTok, YouTube, Instagram, Snapchat, Facebook, Reddit,
Twitch, and others. The goal is not to stop people from using these apps, but to help them use them
intentionally rather than compulsively.

**Is Swock an addiction treatment?**

No. Swock is a digital wellbeing tool, not a medical device or treatment. It adds friction to a
specific compulsive behaviour. People struggling with serious addiction should consult a mental
health professional.

**Does Swock work by spying on what users do?**

No. Swock has no internet access and collects no data. The accessibility service inspects screen
structure locally — it determines whether the current screen is a Shorts/Reels feed — and then
discards that information immediately. No text, credentials, or personal data is ever read, stored,
or transmitted.

**Why isn't Swock open source?**

Swock is proprietary software. The source code is private to protect the app's integrity and the
detection heuristics that make it work. However, Swock's privacy practices are fully documented in
the public [Privacy Policy](privacy-policy.md), and the app declares no INTERNET permission, which
can be verified by anyone who inspects the APK.

**How does Swock make money?**

Swock is free with no ads and no in-app purchases. The developer is an independent studio building
tools for digital wellbeing.

**Can users bypass Swock?**

Yes — users can disable Swock at any time. Swock is designed to add friction, not to be
unbreakable. The goal is to make the swipe a conscious choice rather than a reflex. If a user
deliberately decides to swipe to the next video, that's a success — it means the behaviour is now
intentional.

---

## Brand assets

| Asset | Format | Available from |
|:------|:-------|:---------------|
| App logo (shield) | PNG | This repository (`swock_logo.png`) |
| Wordmark | JPG | This repository (`swock_wordmark.jpg`) |
| App icon | PNG | Google Play Store listing |
| Screenshots | PNG | Google Play Store listing |
| Brand colour | Cobalt Blue `#0047AB` | — |

> For high-resolution assets, interview requests, or review copies, contact the developer via
> [GitHub](https://github.com/Made-in-Jurgistan/swock-public/issues).

---

## Media contact

- **GitHub**: [Made-in-Jurgistan/swock-public](https://github.com/Made-in-Jurgistan/swock-public)
- **Issues**: [Open a private issue](https://github.com/Made-in-Jurgistan/swock-public/issues)
- **Developer**: [Made in Jurgistan](https://github.com/Made-in-Jurgistan)

---

## Coverage guidelines

We ask that coverage of Swock includes:

1. **A link to the public repository**: `https://github.com/Made-in-Jurgistan/swock-public`
2. **A link to the Google Play Store** (when available)
3. **Accurate description of privacy**: Swock collects no data and has no internet access
4. **Accurate description of scope**: Swock blocks the swipe gesture, not the app itself

Please avoid:

- Describing Swock as an "app blocker" or "TikTok blocker" — it blocks a gesture, not an app
- Describing Swock as a medical treatment or addiction cure
- Claiming Swock is unbreakable — it's designed to add friction, not to be impossible to bypass

---

<div align="center">

<sub>© 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
