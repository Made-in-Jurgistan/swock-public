<div align="center">

<img src="swock_logo.png" width="100" alt="Swock">

# Security policy

</div>

How to report a security problem in Swock privately, which versions are covered, and how Swock
is built to limit what it can do.

## Contents

- [Supported versions](#supported-versions)
- [Reporting a vulnerability](#reporting-a-vulnerability)
- [How Swock limits its access](#how-swock-limits-its-access)
- [Scope](#scope)

---

## Supported versions

| Version | Supported |
|:--------|:----------|
| 1.0.x | Yes |

---

## Reporting a vulnerability

**Please don't open a public GitHub issue for a security problem.**

Report it privately through
[GitHub's private vulnerability reporting](https://github.com/Made-in-Jurgistan/swock-public/security/advisories/new).
Include:

- a description of the problem,
- steps to reproduce it, or a proof of concept,
- its impact and the versions affected, and
- a suggested fix, if you have one.

You will get an acknowledgement within **72 hours**. We prefer coordinated disclosure, so please
allow reasonable time for a fix before publishing details.

---

## How Swock limits its access

| Area | What Swock does |
|:-----|:----------------|
| Network | Swock does not ask for the `INTERNET` permission, so Android does not let it open network connections. It contains no analytics, telemetry, ad SDKs or Play Integrity client. |
| Data | All processing happens on the phone. No user data leaves the device. See the [Privacy Policy](privacy-policy.md). |
| Storage | Settings are kept in app-private storage and excluded from Android backups. Swock does not use shared or external storage. |
| Accessibility service | Receives events from the 8 supported apps only. It inspects their screen layout to recognise Shorts and Reels players and, only while a player is protected, drops the vertical swipe. It does not store or transmit text, credentials or personal data. Outside that window, touches reach apps unchanged. |
| Touch handling | Uses Android's `TouchInteractionController` (Android 13 and newer) on the default display only. The shield badge cannot receive touches. |
| Errors | If Swock briefly cannot read the screen or start touch filtering, it switches touch filtering off rather than leaving it on. |
| Release signing | The release workflow only builds with the project's release signing key and fails without it. Check the APK signature before you install it from a file. |

---

## Scope

**In scope:**

- abuse of the accessibility service, such as reading sensitive data or sending it off the
  device,
- privilege escalation,
- crashes or denial of service caused by crafted accessibility events,
- supply chain risks in dependencies,
- repackaging or tampering with the app, and
- touch filtering left on after a service error.

**Out of scope:**

- getting around swipe blocking (Swock adds friction and is not meant to be unbreakable),
- problems in the third-party apps Swock works with, such as TikTok or YouTube, and
- secondary displays and foldable outer screens (Swock supports the default display only).

Other questions: [Help and troubleshooting](SUPPORT.md) · [FAQ](FAQ.md) · [README](README.md)

<div align="center">

<sub>© 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
