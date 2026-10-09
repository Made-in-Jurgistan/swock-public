<div align="center">

<img src="swock_logo.png" width="100" alt="Swock">

# Help and troubleshooting

</div>

Fixes for the most common Swock problems, and how to report one we haven't covered. Find your
symptom below and work through the fix in order.

## Contents

- [Quick fixes](#quick-fixes)
- [Setup problems](#setup-problems)
- [Swipes are not blocked](#swipes-are-not-blocked)
- [Swock blocks too much](#swock-blocks-too-much)
- [The shield badge](#the-shield-badge)
- [Battery and stability](#battery-and-stability)
- [Report a bug](#report-a-bug)
- [Ask for a new app](#ask-for-a-new-app)
- [Contact](#contact)

---

## Quick fixes

| Symptom | Try this first |
|:--------|:---------------|
| Swock isn't blocking anything | Check the status card in Swock. It should say **Active** or **Protecting**. See [Swipes are not blocked](#swipes-are-not-blocked). |
| The switch in Settings won't turn on | See [The switch won't turn on](#the-switch-wont-turn-on). |
| Blocking worked before and then stopped | In Android's accessibility settings, turn Swock off and on again. |
| Blocking is slow to start or comes and goes | Set Swock's battery use to **Unrestricted**. See [Battery and stability](#battery-and-stability). |
| No shield badge | Turn on **Show indicator** in Swock. |
| "Swock keeps stopping" | That's a crash. Please [report it](#report-a-bug). |
| You want to stop yourself from turning Swock off | Not possible yet. Swock is an MVP; PIN or password protection for turning off blocking in Swock is planned for a later version. See the [FAQ](FAQ.md#can-i-stop-myself-from-just-turning-it-off). |

---

## Setup problems

### The switch won't turn on

**Symptom:** Android says "Restricted setting" when you tap the Swock switch.

**Why:** Android 13 and newer lock some settings for apps installed from a downloaded file. You
have to unlock them once.

**Fix:** Follow Swock's three steps. They appear in Swock one after another each time you press
Back from Settings.

1. **Step 1 of 3: Find Swock.** Tap **Open settings**. Then:
   "Scroll down and tap Installed apps. (Some phones say Downloaded apps or Installed services.)"
   → "Tap Swock and try to turn on the switch." → "Android says “Restricted setting”. That’s
   normal! Tap OK." → "Press Back to return to Swock."
2. **Step 2 of 3: Allow Swock.** Tap **Open App info**. Then:
   "Tap ⋮ (three dots) in the top right corner." → "Tap Allow restricted settings." → "Confirm
   with your PIN, pattern or fingerprint." → "Press Back to return to Swock."
3. **Step 3 of 3: Turn on Swock.** Tap **Open settings**. Then:
   "Scroll down and tap Installed apps. (Some phones say Downloaded apps or Installed services.)"
   → "Tap Swock." → "Turn on the switch, then tap Allow." → "Press Back to return to Swock."

When you return, the status card says **Active**.

### I can't find "Allow restricted settings"

**Why:** Android only adds that option after it has shown you the "Restricted setting" message.

**Fix:** Go back to step 1. Tap Swock in the accessibility settings and try the switch once, tap
**OK** on the message, then try step 2 again.

### I can't find "Installed apps"

**Fix:** Phone makers name this list differently. Look for **Downloaded apps** or **Installed
services** in the accessibility settings instead.

### The setup pop-up closed and Settings didn't open

**Why:** Settings only opens from the pop-up's **Open settings** or **Open App info** button.
**Not now** just closes it.

**Fix:** Tap the button on the setup card in Swock to open the pop-up again.

---

## Swipes are not blocked

### Swock doesn't block swipes at all

Check these in order:

1. **Is the service on?** The status card in Swock should say **Active** or **Protecting**. If it
   says **Setup Required**, tap the button on the setup card and follow the steps.
2. **Is Swipe Blocking on?** If the status card says **Disabled**, turn on **Swipe Blocking**.
3. **Is the app switched on?** Check the app under **Protected Apps**.
4. **Are you on the video player?** Swock only blocks swipes on the short-video player, not on an
   app's home page, search or profiles. Open the Shorts, Reels or For You player.
5. **Is the shield badge showing?** If **Show indicator** is on and you see no badge, Swock
   hasn't recognised this screen as a video player. See the next section.

### Swock doesn't block swipes in one particular app

| App | Check |
|:----|:------|
| TikTok, TikTok Lite | You are on the For You or Following feed, not Discover or a profile. |
| YouTube | You are in the full-screen Shorts player. A channel's grid of Shorts is not blocked. |
| Instagram | You are in the full-screen Reels player. A profile's grid of Reels is not blocked. Stories are never blocked. |
| Snapchat | You are in Spotlight. |
| Facebook, Facebook Lite | You are in the Reels player. |
| Twitch | You are watching clips. |

If you are in the right place and the badge still doesn't appear:

- **Language:** Swock recognises TikTok and Facebook partly by English labels ("For You",
  "Following", "Reels, tab"). If the app is set to another language, Swock may not recognise the
  player.
- **App update:** an update may have changed the app's screen in a way Swock doesn't recognise
  yet.

Please [report it](#report-a-bug) with the app name, its version and its language.

### Taps or sideways swipes don't work on the player

On a protected player Swock blocks only up and down swipes. Taps register when you lift your
finger, which makes them respond a moment later than usual. Sideways swipes and two-finger
gestures go straight to the app, and opening comments or share pauses blocking.

If taps or sideways swipes really are blocked, please [report it](#report-a-bug) and say what was
blocked and what you were doing.

### Swiping in from the edge doesn't go back

**Why:** On a protected player, Swock turns an edge swipe into Back only when your phone uses
gesture navigation.

**Fix:** With navigation buttons, use the Back button.

---

## Swock blocks too much

### Swipes are blocked on a screen that isn't a video player

[Report it](#report-a-bug) with:

- the app name and version,
- the screen you were on (for example, "Instagram Explore"), and
- what you expected to happen.

### Snapchat Stories are blocked

**Why:** In Snapchat, the Stories viewer shares screen signals with Spotlight, so Swock can treat
it the same way.

**Fix:** To swipe through Stories, switch Snapchat off under **Protected Apps** for a while.

---

## The shield badge

### The badge doesn't appear

1. Make sure **Show indicator** is on in Swock.
2. Make sure you are on the video player of a supported app.
3. Switch to another app and back, so Swock checks the screen again.

### The badge appears where it shouldn't

Swock thinks this screen is a video player. Please [report it](#report-a-bug) with the app name
and the screen you were on.

### I want to hide the badge

Turn off **Show indicator** in Swock. Blocking keeps working without it.

---

## Battery and stability

### Blocking is slow to start, comes and goes, or stops

**Why:** Some phone makers, Samsung among them, pause apps in the background to save battery.
That can delay Swock.

**Fix:**

1. Open **Settings → Apps → Swock → Battery**. The path differs between phone makers.
2. Choose **Unrestricted** (on some phones, **Don't optimise**).

If blocking still stops, turn Swock off and on again in Android's accessibility settings.

### Swock seems to use a lot of battery

Swock only does work while one of the 8 supported apps is open. If you still see high battery use:

1. Switch off apps you don't use under **Protected Apps**.
2. If that doesn't help, please [report it](#report-a-bug).

### "Swock keeps stopping"

That's a crash. Please [report it](#report-a-bug) and include what you were doing, your Android
version and phone model, and Swock's version (**Settings → Apps → Swock** shows it).

---

## Report a bug

[Open an issue](https://github.com/Made-in-Jurgistan/swock-public/issues) and tell us:

1. what happened,
2. what you expected to happen, and
3. the exact steps that cause it.

Please also copy this table into your report and fill it in:

| Detail | Your answer |
|:-------|:------------|
| Swock version | |
| Android version | |
| Phone model | |
| Navigation (gestures or buttons) | |
| App affected | |
| That app's version and language | |

---

## Ask for a new app

[Open an issue](https://github.com/Made-in-Jurgistan/swock-public/issues) with:

1. the app's name,
2. its package name, if you know it (with adb: `adb shell pm list packages | grep <name>`),
3. whether the whole app is a short-video feed or only one part of it, and
4. a screenshot of the short-video player.

---

## Contact

| What you need | Where to go |
|:--------------|:------------|
| Report a bug or ask for a feature | [GitHub Issues](https://github.com/Made-in-Jurgistan/swock-public/issues) |
| Report a security problem | [Security policy](SECURITY.md). Please don't open a public issue. |
| Questions about privacy | [Privacy Policy](privacy-policy.md) |
| General questions | [FAQ](FAQ.md) |
| Press | [Press Kit](PRESS.md) |

<div align="center">

<sub>© 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
