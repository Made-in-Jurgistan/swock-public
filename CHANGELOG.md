<div align="center">

<img src="swock_logo.png" width="100" alt="Swock">

# Changelog

**All notable changes to Swock are documented in this file.**

</div>

---

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [Unreleased]

### Added

- Guided Accessibility setup for Android 13+ restricted settings (“Step 1 / 2 / 3 of 3”), with a short
  hint over each Settings screen; installs Android does not guard skip the extra steps
- Release signing configuration
- Stricter code obfuscation in release builds

### Fixed

- Documentation corrected: Swock supports **8** apps (not 14) and contains no Play Integrity
  integration (it declares no INTERNET permission and makes no network requests)

---

## [1.0.0] — 2026-08-02

### Added

- **Swipe-to-next-video blocking** in short-form video apps
- **8 supported apps**: TikTok, TikTok Lite, YouTube Shorts, Instagram Reels, Snapchat Spotlight,
  Facebook Reels, Facebook Lite, and Twitch Clips
- **Per-app toggle** — choose exactly which apps to protect
- **Visual indicator badge** showing when blocking is active
- **Full gesture pass-through**: taps, horizontal swipes, long-press, edge gestures, and
  multi-touch all work normally
- **Zero data collection** — no network access, no analytics, no telemetry
- **Material 3 settings UI** with dynamic colour theming
- **Battery efficient** — only activates on Shorts/Reels feeds

### Privacy

- No INTERNET permission declared
- No analytics, telemetry, or crash reporting
- All preferences stored locally in app-private storage
- Accessibility service inspects screen structure locally only — never reads, stores, or
  transmits text, credentials, or personal data

---

<div align="center">

[Unreleased]: https://github.com/Made-in-Jurgistan/swock-public/commits/main
[1.0.0]: https://github.com/Made-in-Jurgistan/swock-public

</div>

---

<div align="center">

<sub>© 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
