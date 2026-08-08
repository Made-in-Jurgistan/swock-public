<div align="center">

<img src="swock_logo.png" width="100" alt="Swock">

# Security Policy

</div>

---

## Contents

- [Supported versions](#supported-versions)
- [Reporting a vulnerability](#reporting-a-vulnerability)
- [Security posture](#security-posture)
- [Scope](#scope)

---

## Supported versions

| Version | Supported |
|:--------|:----------|
| 1.0.x | Yes |

---

## Reporting a vulnerability

> **Do not open a public GitHub issue for security vulnerabilities.**

Instead, email the maintainer directly with:

- A description of the vulnerability
- Steps to reproduce or a proof of concept
- The impact and affected versions
- Suggested fix (optional)

You will receive an acknowledgement within **72 hours**. Coordinated disclosure is preferred —
please allow reasonable time for a fix before publishing details.

---

## Security posture

Swock is designed with a minimal attack surface:

| Principle | Detail |
|:----------|:-------|
| **No declared INTERNET permission** | No analytics, no telemetry, no ad SDKs. The Play Integrity API makes network calls via Google Play Services for integrity verification, but Swock itself declares no INTERNET permission. |
| **No data collection** | All processing is local. No user data leaves the device. See the [Privacy Policy](privacy-policy.md) for details. |
| **No external storage** | Preferences are stored in app-private storage. |
| **Accessibility service** | The service only inspects screen structure of target apps to classify screens and intercept the vertical swipe gesture. It does not read or transmit text, credentials, or personal data. |
| **App integrity** | Play Integrity API verifies the app binary is unmodified and installed from Google Play. |
| **Release signing** | Release builds are signed with a 2048-bit RSA key. |

---

## Scope

**In scope:**

- Accessibility service abuse (reading sensitive data, exfiltration)
- Privilege escalation
- Crash or denial-of-service via crafted accessibility events
- Supply chain risks in dependencies
- App repackaging or tampering bypass

**Out of scope:**

- Bypassing swipe blocking (the app is meant to add friction, not be unbreakable)
- Issues in third-party apps (TikTok, YouTube, etc.) that Swock interacts with

---

<div align="center">

<sub>© 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
