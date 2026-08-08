<div align="center">

<img src="swock_logo.png" width="64" alt="Swock app logo — shield icon">
<br>
<img src="swock_wordmark.jpg" width="280" alt="Swock wordmark">

# Support & Troubleshooting

</div>

---

## Contents

- [Quick fixes](#quick-fixes)
- [Setup issues](#setup-issues)
- [Blocking issues](#blocking-issues)
- [Indicator issues](#indicator-issues)
- [Performance issues](#performance-issues)
- [App-specific issues](#app-specific-issues)
- [Reporting bugs](#reporting-bugs)
- [Requesting new app support](#requesting-new-app-support)
- [Contact](#contact)

---

## Quick fixes

> **Try these first.** Most issues are resolved by one of the steps below.

| Problem | Quick fix |
|:--------|:----------|
| Swock isn't blocking | Check accessibility service is on, Swipe Blocking is on, and the app is in your Protected Apps list |
| Swock was working but stopped | Toggle the accessibility service off and on in Android Settings |
| Indicator badge not showing | Toggle **Show indicator** on in Swock's settings |
| Swock service keeps turning off | Disable battery optimisation for Swock in Android Settings |
| "Swock keeps stopping" | Update to the latest version; if it persists, [report it](#reporting-bugs) |

---

## Setup issues

### Swock isn't blocking swipes

Walk through this checklist in order:

1. **Accessibility service enabled?**
   - Open Swock → the status card should show **Active**
   - If it shows **Setup Required**, tap **Enable Accessibility** and toggle Swock on in the
     Android accessibility settings list

2. **Swipe Blocking on?**
   - Open Swock → ensure the **Swipe Blocking** toggle is on

3. **Target app enabled?**
   - Open Swock → under **Protected Apps**, ensure the app you're using is toggled on

4. **On a Shorts/Reels feed?**
   - Swock only blocks swipes on the short-video feed, not the app's home page, search, or profile
   - Navigate to the Shorts/Reels/For You tab in the app

5. **Indicator badge visible?**
   - If the shield indicator is visible at the top of the screen, Swock is active and blocking
   - If it's not visible, Swock doesn't recognise the current screen as a Shorts/Reels feed

### The accessibility service won't enable

1. Go to **Settings → Accessibility → Swock**
2. Toggle on
3. Accept the warning dialog (this is standard for all accessibility services)
4. Return to Swock — the status card should now show **Active**

If the toggle keeps turning off:
- Go to **Settings → Apps → Swock → Battery**
- Set battery optimisation to **Unrestricted**
- Some manufacturers (Xiaomi, Oppo, Vivo) aggressively kill background services — check their
  specific battery saver settings

### Sideloading installation issues

If you installed Swock from a [GitHub Release](https://github.com/Made-in-Jurgistan/swock-public/releases)
APK instead of the Play Store:

- **"App not installed"** — Your device may block unknown-source installs. Go to
  **Settings → Apps → Special access → Install unknown apps** and allow your file manager or browser.
- **Signature mismatch** — If you previously installed a different build (e.g., Play Store version),
  uninstall it first. Android rejects signature mismatches between builds.
- **"Play Protect blocked install"** — Tap **Install anyway**. Play Protect warns about all
  sideloaded APKs, not just malicious ones.

---

## Blocking issues

### Swock was working but stopped after an app update

App updates can change internal UI structure. Swock updates are released to handle these changes.
Check for Swock updates on Google Play. If the issue persists,
[report it](#reporting-bugs) with the app name and version.

### Swock blocks swipes on a screen where it shouldn't

This can happen if an app's screen structure resembles a Shorts/Reels feed.
[Report it](#reporting-bugs) with:
- App name
- Which screen you were on (e.g., "Instagram Explore page")
- What you expected (e.g., "Swipes should work here")

### Swock doesn't block swipes on a supported app

The app may have changed its UI structure in a recent update.
[Report it](#reporting-bugs) with the app name and version.

### Taps or horizontal swipes aren't working in a supported app

This shouldn't happen — Swock only blocks vertical swipes on Shorts/Reels feeds. If taps or
horizontal swipes are blocked, [report it](#reporting-bugs) immediately with:
- App name and version
- What was blocked (taps, horizontal swipes, etc.)
- What you were doing when it happened

---

## Indicator issues

### The indicator badge isn't showing

1. Ensure **Show indicator** is toggled on in Swock's settings
2. Ensure you're on a Shorts/Reels feed in a supported app
3. Try switching away from the app and back — this triggers a re-scan

### The indicator badge is showing on a screen where it shouldn't

This means Swock thinks the current screen is a Shorts/Reels feed when it isn't.
[Report it](#reporting-bugs) with the app name and which screen you were on.

### The indicator badge is annoying

You can disable it in Swock's settings by toggling **Show indicator** off. Blocking will still
work — you just won't see the visual confirmation.

---

## Performance issues

### Swock service keeps turning off

Android may disable accessibility services to save battery. To prevent this:

1. Go to **Settings → Apps → Swock → Battery**
2. Set battery optimisation to **Unrestricted** or **Don't optimise**

The exact path varies by device manufacturer:

| Manufacturer | Path |
|:-------------|:-----|
| Samsung | Settings → Apps → Swock → Battery → Unrestricted |
| Xiaomi / Redmi / POCO | Settings → Apps → Manage apps → Swock → Battery saver → No restrictions |
| Oppo / Realme / OnePlus | Settings → Battery → App battery management → Swock → Allow background activity |
| Vivo / iQOO | Settings → Battery → Background power consumption management → Swock → Allow |
| Huawei / Honor | Settings → Battery → App launch → Swock → Manage manually → Enable all |
| Pixel / Stock Android | Settings → Apps → Swock → Battery → Unrestricted |

### Swock is using too much battery

Swock should use negligible battery because it only activates on Shorts/Reels feeds. If you're
seeing high battery usage:
1. Check which apps you have enabled in Protected Apps — disable any you don't use
2. Update to the latest version of Swock
3. [Report it](#reporting-bugs) if the issue persists

### "Swock keeps stopping" error

This is a crash. [Report it](#reporting-bugs) with:
- What you were doing when it crashed
- Your Android version and device model
- The Swock version (find it in Swock → Settings → About)

---

## App-specific issues

### TikTok

Swock should block swipes on the For You and Following feeds. If it doesn't:
- Ensure you're on the For You or Following tab (not Discover or Profile)
- Check that TikTok is toggled on in Swock's Protected Apps

### YouTube

Swock blocks swipes on YouTube Shorts. If it doesn't:
- Ensure you're on the Shorts tab (not Home, Subscriptions, or Library)
- Check that YouTube is toggled on in Swock's Protected Apps

### Instagram

Swock blocks swipes on Instagram Reels. If it doesn't:
- Ensure you're on the Reels tab (not Feed, Explore, or Profile)
- Check that Instagram is toggled on in Swock's Protected Apps

### Other apps

For all other supported apps, ensure you're on the short-video feed and the app is toggled on in
Swock's Protected Apps. If issues persist, [report it](#reporting-bugs).

---

## Reporting bugs

[Open an issue](https://github.com/Made-in-Jurgistan/swock-public/issues) with:

1. **What happened** — describe the problem clearly
2. **What you expected** — what should have happened instead
3. **Steps to reproduce** — exact actions to trigger the issue
4. **Your environment**:

| Field | Your value |
|:------|:-----------|
| Swock version | |
| Android version | |
| Device model | |
| Affected app | |
| Affected app version | |

The more detail you provide, the faster we can fix it.

---

## Requesting new app support

[Open an issue](https://github.com/Made-in-Jurgistan/swock-public/issues) with:

1. **App name**
2. **Package name** (find it with `adb shell pm list packages | grep <name>` if you have ADB)
3. **Is the app 100% short-video feed?** Or does it have other screens?
4. **Screenshot** of the Shorts/Reels player screen

We'll investigate whether reliable detection is feasible.

---

## Contact

| Need | Where |
|:-----|:------|
| Bug reports | [GitHub Issues](https://github.com/Made-in-Jurgistan/swock-public/issues) |
| Feature requests | [GitHub Issues](https://github.com/Made-in-Jurgistan/swock-public/issues) |
| Security vulnerabilities | See [SECURITY.md](SECURITY.md) — do not open a public issue |
| Privacy questions | See [Privacy Policy](privacy-policy.md) |
| Press inquiries | See [Press Kit](PRESS.md) |

---

<div align="center">

<sub>© 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
