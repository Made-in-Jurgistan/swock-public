<div align="center">

<img src="swock_logo.png" width="100" alt="Swock">

# Privacy Policy

**Swock — Swipe Blocker for Short Videos**

**Last updated: 2026-10-10**

</div>

This policy explains what information Swock handles, what it does with it, and what it never
does. The short version: **Swock collects no data.** It has no internet access, no analytics and
no tracking. Everything happens on your phone.

## Contents

- [Summary](#summary)
- [What Swock collects](#what-swock-collects)
- [The accessibility service](#the-accessibility-service)
- [Permissions](#permissions)
- [What Swock stores on your phone](#what-swock-stores-on-your-phone)
- [Third-party services](#third-party-services)
- [Children's privacy](#childrens-privacy)
- [Changes to this policy](#changes-to-this-policy)
- [Contact](#contact)

---

## Summary

- Swock does not collect, sell or share personal data.
- Swock does not ask for the `INTERNET` permission, so it cannot connect to any server.
- Swock looks at the screen of 8 supported apps only to recognise a short-video player, and only
  on your phone. It does not save, log or send what it sees.
- Your Swock settings stay on your phone and are excluded from Android backups.

---

## What Swock collects

| Type of data | Collected? | Notes |
|:-------------|:-----------|:------|
| Personal information | No | |
| Device identifiers | No | |
| Usage analytics | No | |
| Crash reports | No | |
| Network traffic | No | Swock has no `INTERNET` permission. |
| Screen layout of supported apps (accessibility node content) | Processed on the phone, not stored or sent | Used to recognise the screen type |
| Touch events | Processed on the phone, not stored or sent | Used to tell swipes, taps and other gestures apart |
| Your Swock settings | Stored on the phone only | Which apps are protected, and Swock's switches |

Swock sends nothing off your phone. There is no backend server, no cloud sync and no data
sharing with third parties.

---

## The accessibility service

Swock works through an Android **accessibility service**. This is a kind of Android permission
meant for tools that help people use their phone. It lets an app look at what is on screen and
respond to touches. You turn it on yourself in Android's settings, and you can turn it off there
at any time.

Swock's accessibility service is set up to retrieve the content of the windows it watches, to
filter touches (Android's touch exploration mode), and to perform gestures, which it uses to
replay your taps. Here is how it uses those abilities.

**Which apps.** Android sends Swock accessibility events only from the 8 supported apps: TikTok,
TikTok Lite, YouTube, Instagram, Snapchat, Facebook, Facebook Lite and Twitch.

**What it looks at.** Swock inspects the accessibility node tree, the screen layout, of the
supported app you are using. It uses this only to decide whether a Shorts or Reels player is on
screen and whether a comments or share panel is open. It does not log, store or transmit text,
passwords, personal data or any other information from that screen. Nothing it inspects is kept
after the decision is made.

**Touches.** Only while a protected player is on screen, Swock receives raw touch events through
Android's `TouchInteractionController` (Android 13 and newer). It sorts each touch as it happens
(up or down swipe, tap, long-press, sideways swipe, multi-finger gesture or edge swipe) and then
discards it. No touch positions or gesture traces are stored or sent.

**Replayed taps.** Taps and long-presses on a protected player are held until you lift your
finger, then replayed on the phone with `dispatchGesture()` once the held touches have cleared.
Replayed taps are not stored or sent.

**When it filters touches.** Swock filters touches only in supported apps you have left switched
on in Swock (all are on when you install it), only while a Shorts or Reels player is showing, and
only while no comments or share panel is open. At all other times, touches reach apps unchanged.

---

## Permissions

| Permission | Type | Used by Swock? | Purpose |
|:-----------|:-----|:---------------|:--------|
| `BIND_ACCESSIBILITY_SERVICE` | System | Yes | Protects Swock's accessibility service so that only Android itself can connect to it |
| `INTERNET` | Normal | No | Not requested. Swock has no network access. |
| `ACCESS_NETWORK_STATE` | Normal | No | Not requested |
| `READ/WRITE_EXTERNAL_STORAGE` | Dangerous | No | Not requested |
| `CAMERA` | Dangerous | No | Not requested |
| `RECORD_AUDIO` | Dangerous | No | Not requested |
| `ACCESS_FINE_LOCATION` | Dangerous | No | Not requested |

Swock requests no dangerous permissions and no network permissions. The only permission Swock
itself requests is an internal, signature-level one that the AndroidX library adds so that other
apps cannot reach Swock's own broadcast receivers.

---

## What Swock stores on your phone

Swock keeps your settings in app-private storage on your phone, using Android's Preferences
DataStore. Other apps cannot read it, and it never leaves your phone.

| Setting | Where it is kept | Encrypted? |
|:--------|:-----------------|:-----------|
| **Swipe Blocking** switch (on or off) | App-private DataStore | No (not sensitive) |
| Which apps are protected | App-private DataStore | No (not sensitive) |
| **Show indicator** switch | App-private DataStore | No (not sensitive) |

Swock does not store anything in external storage, in preferences other apps can read, or in any
cloud service. Its settings are excluded from Android cloud backups and from transfers to a new
device. When you uninstall Swock, Android deletes them.

---

## Third-party services

| Service | Purpose | Data shared |
|:--------|:--------|:------------|
| GitHub Releases | Hosting the APK download | None by Swock. Swock makes no network requests. Downloading the APK from GitHub is covered by GitHub's own terms. |

Swock uses no other third-party services. It contains no analytics, advertising or
crash-reporting SDKs, and no Play Integrity client.

---

## Children's privacy

Swock is not directed at children under 13 and does not knowingly collect personal information
from children. Swock collects no data from any user, so no special protections for children's
data are needed.

---

## Changes to this policy

The copyright holder may change this privacy policy. Changes are posted in this document with a
new "Last updated" date. If you keep using Swock after a change, you accept the revised policy.

---

## Contact

For privacy questions or concerns, open an issue on the
[public GitHub repository](https://github.com/Made-in-Jurgistan/swock-public/issues).

Related documents: [Terms of Service](terms-of-service.md) · [README](README.md) · [FAQ](FAQ.md)

---

<div align="center">

<sub>© 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
