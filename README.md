<div align="center">

<img src="swock_logo.png" width="120" alt="Swock">

# Swock

### Swipe blocker for short videos

[![Platform](https://img.shields.io/badge/Platform-Android_13+-3DDC84?logo=android&logoColor=white)](https://www.android.com)
[![Privacy](https://img.shields.io/badge/Privacy-No%20data%20collection-0047AB)](privacy-policy.md)
[![License](https://img.shields.io/badge/License-Proprietary-red)](terms-of-service.md)

**[Download the APK](https://github.com/Made-in-Jurgistan/swock-public/releases)** &nbsp;·&nbsp; [FAQ](FAQ.md) &nbsp;·&nbsp; [Help and troubleshooting](SUPPORT.md) &nbsp;·&nbsp; [Report a problem](https://github.com/Made-in-Jurgistan/swock-public/issues)

</div>

Swock is an Android app that stops the swipe that takes you to the next video in TikTok, YouTube
Shorts, Instagram Reels and similar apps. You can still watch, tap, like, comment and swipe
sideways. Only the up and down swipe on the video player stops working.

> **Status:** Swock is an early version, an MVP (minimum viable product). Right now anyone
> holding the phone can turn blocking off. PIN or password protection for turning off blocking in Swock is planned for a later version.
> See [Turning Swock off](#turning-swock-off).

This page explains what Swock does, how to set it up, and where to find help.

## Contents

- [What Swock does](#what-swock-does)
- [Supported apps](#supported-apps)
- [Install and set up](#install-and-set-up)
- [Using Swock](#using-swock)
- [Good to know](#good-to-know)
- [Privacy](#privacy)
- [Research on short-form video](#research-on-short-form-video)
- [More help and documents](#more-help-and-documents)
- [About](#about)

---

## What Swock does

In short-video apps, swiping up on the player loads the next video, and swiping down goes back
to the previous one. Swock blocks that one gesture on the video player. It does not block apps,
videos or any other feature.

| Still works on the video player | Blocked on the video player |
|:--------------------------------|:----------------------------|
| Watching the video in front of you | Swiping up to the next video |
| Tapping to pause, like, comment or share | Swiping down to the previous video |
| Long-pressing | |
| Swiping left or right, and pinching with two fingers | |
| Opening the comments or share panel (blocking pauses while it is open) | |
| Going back by swiping in from the screen edge, if your phone uses gesture navigation | |

Everywhere else, such as search, profiles, home feeds, other apps and your home screen, Swock
leaves your touches alone.

Swock needs no root access and no VPN. It has no internet permission and collects no data.

---

## Supported apps

| App | Where Swock blocks the swipe |
|:----|:-----------------------------|
| TikTok | For You and Following feeds |
| TikTok Lite | For You and Following feeds |
| YouTube | Shorts player |
| Instagram | Reels player |
| Snapchat | Spotlight |
| Facebook | Reels |
| Facebook Lite | Reels |
| Twitch | Clips and the clips feed |

All 8 apps are switched on when you install Swock. You can switch each one off separately.

- On YouTube and Instagram, Swock blocks the swipe in the full-screen Shorts or Reels player. The
  grid of Shorts or Reels on a channel or profile page is not affected.
- Instagram Stories are not affected.
- In Snapchat, the Stories viewer can be treated like Spotlight, so swipes there may be blocked too.
- Swock recognises TikTok and Facebook partly by English labels on screen. If those apps are set
  to another language, Swock may not recognise the player and the swipe then works as normal.

Want another app supported? [Open an issue](https://github.com/Made-in-Jurgistan/swock-public/issues)
with the app's name.

---

## Install and set up

You need a phone with Android 13 or newer. Swock does not run on older versions.

### 1. Install

1. Download the APK file from
   [GitHub Releases](https://github.com/Made-in-Jurgistan/swock-public/releases).
2. Open the file on your phone and tap **Install**. If your phone asks, allow installs from that
   source.

### 2. Turn on Swock

Android doesn't let apps switch on their own accessibility service, so you do it yourself in
Settings, once. Swock shows you each step in a pop-up before it opens Settings.

1. Open Swock. On the setup card, tap **Open settings**.
2. Read the steps in the pop-up, then tap **Open settings** again. (**Not now** closes it.)
3. In Settings, follow the steps:
   1. "Scroll down and tap Installed apps. (Some phones say Downloaded apps or Installed
      services.)"
   2. "Tap Swock."
   3. "Turn on the switch, then tap Allow."
   4. "Press Back to return to Swock."

#### If you installed Swock from a downloaded file

Android 13 and newer add an extra lock, called "restricted settings", to apps installed from a
file. Swock notices this and splits setup into three short steps. Each time you press Back from
Settings, the next step appears in Swock on its own.

**Step 1 of 3: Find Swock** (button: **Open settings**)

1. "Scroll down and tap Installed apps. (Some phones say Downloaded apps or Installed services.)"
2. "Tap Swock and try to turn on the switch."
3. "Android says “Restricted setting”. That’s normal! Tap OK."
4. "Press Back to return to Swock."

**Step 2 of 3: Allow Swock** (button: **Open App info**)

1. "Tap ⋮ (three dots) in the top right corner."
2. "Tap Allow restricted settings."
3. "Confirm with your PIN, pattern or fingerprint."
4. "Press Back to return to Swock."

The **Allow restricted settings** option only shows up after Android has shown the "Restricted
setting" message in step 1.

**Step 3 of 3: Turn on Swock** (button: **Open settings**)

Repeat the four steps from the list above. This time the switch turns on.

When setup is done, the status card in Swock says **Active**. **Swipe Blocking** is on from the
start, so there is nothing else to switch on.

Stuck? See [The switch won't turn on](SUPPORT.md#the-switch-wont-turn-on) in the help page.

---

## Using Swock

1. Open one of the supported apps and go to its Shorts or Reels player.
2. A small shield badge that says "Swipe blocked" appears at the top of the screen.
3. Watch, tap, like and comment as usual.
4. Swipe up or down: the video stays where it is.
5. Leave the player or close the app, and the badge disappears.

The status card in Swock shows what is happening:

| Status | Meaning |
|:-------|:--------|
| **Setup Required** | The accessibility service is off. Follow the setup card. |
| **Active** | Swock is on and waiting for a supported app. |
| **Protecting** | Swock is blocking swipes in the app you have open. |
| **Disabled** | **Swipe Blocking** is switched off. |

You can change these in Swock at any time:

- **Swipe Blocking**: switches all blocking on or off.
- **Show indicator**: shows or hides the shield badge. Blocking works either way.
- **Protected Apps**: switches blocking on or off for each app.

### Turning Swock off

Anyone holding the phone can turn Swock off at any time, in any of these ways:

- turn off **Swipe Blocking** in Swock,
- switch off one app under **Protected Apps**,
- turn off Swock in Android's accessibility settings, or
- uninstall Swock.

Swock makes getting to the next video take a deliberate step. It is not built to be impossible
to get around. PIN or password protection for turning off blocking in Swock is planned for a later version. Android's own settings and uninstalling stay
available either way, because no app can lock those.

---

## Good to know

- On a protected player, a tap registers when you lift your finger, so it responds a moment later
  than usual. Other screens are not affected.
- If your phone uses gesture navigation, swiping in from the left or right edge of a protected
  player takes you back. With navigation buttons, use the Back button.
- In split-screen, Swock only checks the app you last touched.
- Swock works on your phone's main screen only. Some outer screens on foldable phones are not
  supported.
- Swock recognises each player by how the app's screen is built. When an app changes its design,
  Swock can stop recognising it until Swock is updated.
- After you leave a player, blocking can take up to about a third of a second to switch off.
- Some phones, Samsung among them, pause apps in the background to save battery. That can make
  Swock slow to react. Setting Swock's battery use to **Unrestricted** helps.
- If you also use TalkBack, Swock does not switch off TalkBack's touch exploration. Android keeps
  it on as long as any service asks for it.
- Swock does not work reliably in Android emulators. Use a real phone.
- Swock is a tool that adds friction to scrolling. It is not a medical treatment and does not
  replace professional help.

---

## Privacy

Swock collects no data. It has no internet permission, so it cannot send anything off your phone.

To work, Swock uses an **accessibility service**. This is a kind of Android permission meant for
tools that help people use their phone. It lets an app look at what is on screen and respond to
touches. Swock uses it for two things only:

- to check whether a Shorts or Reels player is on screen in one of the 8 supported apps, and
- to stop the up and down swipe while that player is showing.

Swock does not save, log or send any text, passwords or personal information it could see. Your
settings stay on your phone, in storage only Swock can read, and are left out of Android backups.

Read the full [Privacy Policy](privacy-policy.md).

---

## Research on short-form video

These published studies look at short-form video and endless scrolling. None of them tested
Swock. Most of the findings are correlations, which show a link but not a cause.

- **Nguyen et al. (2025)**, *Psychological Bulletin*. A review and meta-analysis of 71 studies
  with 98,299 participants. Heavier short-form video use was linked with poorer attention
  (r = −.38) and inhibitory control (r = −.41), and with poorer mental health (r = −.21),
  including stress (r = −.34) and anxiety (r = −.33).
  [doi:10.1037/bul0000498](https://doi.org/10.1037/bul0000498)
- **Luo et al. (2025)**, *Behavioral Sciences*. A small randomized experiment (72 people). After
  30 minutes of TikTok-style videos, participants made less use of extra preparation time in a
  task-switching test than people who watched a documentary or no video. The authors call the
  evidence preliminary.
  [doi:10.3390/bs15081070](https://doi.org/10.3390/bs15081070)
- **Ma & Jiang (2024)**, *Cyberpsychology*. In the second of two experiments, swiping through a
  short-video feed, rather than the videos themselves, lowered people's tendency to think
  analytically.
  [doi:10.5817/CP2024-3-1](https://doi.org/10.5817/CP2024-3-1)
- **Park & Jung (2024)**, *Telematics and Informatics*. A mixed-methods study that linked infinite
  scrolling with a reduced sense of self-control among short-form video users.
  [doi:10.1016/j.tele.2024.102200](https://doi.org/10.1016/j.tele.2024.102200)
- **Ruiz et al. (2024)**, *Mensch und Computer 2024*. In a study of 30 people, those who had to
  react to each post before seeing the next remembered the content better than those using
  infinite scroll. Most participants found the slower design frustrating.
  [doi:10.1145/3670653.3677495](https://doi.org/10.1145/3670653.3677495)

Full references are in the [Press Kit](PRESS.md#research).

---

## More help and documents

| Document | What it covers |
|:---------|:---------------|
| [FAQ](FAQ.md) | Common questions, grouped by topic |
| [Help and troubleshooting](SUPPORT.md) | Fixes for setup and blocking problems, and how to report a bug |
| [Privacy Policy](privacy-policy.md) | What Swock does and does not do with your data |
| [Terms of Service](terms-of-service.md) | The terms for using Swock |
| [Security](SECURITY.md) | How to report a security problem privately |
| [Press Kit](PRESS.md) | Facts, descriptions and the logo for journalists |
| [Releases](https://github.com/Made-in-Jurgistan/swock-public/releases) | APK downloads |

---

## About

Swock is made by [Made in Jurgistan](https://github.com/Made-in-Jurgistan). It is free, with no
ads and no in-app purchases. Swock is proprietary software and all rights are reserved; see the
[Terms of Service](terms-of-service.md).

<div align="center">

<sub>© 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
