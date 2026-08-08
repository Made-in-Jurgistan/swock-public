<div align="center">

<img src="swock_logo.png" width="80" alt="Swock">

# Support & Troubleshooting

</div>

---

## Contents

- [Getting started](#getting-started)
- [Common issues](#common-issues)
- [Reporting bugs](#reporting-bugs)
- [Requesting new app support](#requesting-new-app-support)
- [Contact](#contact)

---

## Getting started

### Swock isn't blocking swipes

1. **Check the accessibility service is enabled**
   - Open Swock → the status card should show **Active**
   - If it shows **Setup Required**, tap **Enable Accessibility** and toggle Swock on

2. **Check Swipe Blocking is on**
   - Open Swock → toggle **Swipe Blocking** on

3. **Check the target app is enabled**
   - Open Swock → under **Protected Apps**, ensure the app you're using is toggled on

4. **Check you're on a Shorts/Reels feed**
   - Swock only blocks swipes on the short-video feed, not the app's home page, search, or
     profile. Navigate to the Shorts/Reels tab in the app.

5. **Check the indicator badge**
   - If the shield indicator is visible at the top of the screen, Swock is active and blocking
   - If it's not visible, Swock doesn't recognise the current screen as a Shorts/Reels feed

### The indicator badge isn't showing

1. Ensure **Show indicator** is toggled on in Swock's settings
2. Ensure you're on a Shorts/Reels feed in a supported app
3. Try switching away from the app and back — this triggers a re-scan

---

## Common issues

### Swock was working but stopped after an app update

App updates can change internal UI structure. Swock updates are released to handle these
changes. Check for Swock updates on Google Play. If the issue persists,
[report it](#reporting-bugs).

### Swock blocks swipes on a screen where it shouldn't

This can happen if an app's screen structure resembles a Shorts/Reels feed.
[Report it](#reporting-bugs) with the app name, which screen you were on, and what you expected.

### Swock doesn't block swipes on a supported app

The app may have changed its UI structure in a recent update.
[Report it](#reporting-bugs) with the app name and version.

### Taps or horizontal swipes aren't working in a supported app

This shouldn't happen — Swock only blocks vertical swipes on Shorts/Reels feeds. If taps or
horizontal swipes are blocked, [report it](#reporting-bugs) immediately with details.

### Swock service keeps turning off

Android may disable accessibility services to save battery. To prevent this:

1. Go to **Settings → Apps → Swock → Battery**
2. Set battery optimisation to **Unrestricted** or **Don't optimise**

The exact path varies by device manufacturer.

### "Swock keeps stopping" error

This is a crash. [Report it](#reporting-bugs) with:
- What you were doing when it crashed
- Your Android version and device model
- The Swock version

---

## Reporting bugs

[Open an issue](https://github.com/Made-in-Jurgistan/swock-public/issues) with:

1. **What happened** — describe the problem
2. **What you expected** — what should have happened
3. **Steps to reproduce** — exact actions to trigger the issue
4. **Your environment**:
   - Swock version
   - Android version
   - Device model
   - Affected app name and version

The more detail you provide, the faster we can fix it.

---

## Requesting new app support

[Open an issue](https://github.com/Made-in-Jurgistan/swock-public/issues) with:

1. **App name**
2. **Package name** (find it with `adb shell pm list packages | grep <name>` if you have ADB)
3. **Is the app 100% short-video feed?** Or does it have other screens?
4. **Screenshot** of the Shorts/Reels player screen

---

## Contact

- **Bugs and feature requests**: [GitHub Issues](https://github.com/Made-in-Jurgistan/swock-public/issues)
- **Security vulnerabilities**: See [SECURITY.md](SECURITY.md) — do not open a public issue
- **Privacy questions**: See [Privacy Policy](privacy-policy.md)

---

<div align="center">

<sub>(c) 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
