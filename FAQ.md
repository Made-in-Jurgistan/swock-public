<div align="center">

<img src="swock_logo.png" width="100" alt="Swock">

# Frequently asked questions

</div>

Short answers to the questions people ask most about Swock. If something isn't working, the
[help and troubleshooting page](SUPPORT.md) has step-by-step fixes.

## Contents

- [About Swock](#about-swock)
- [Setting up](#setting-up)
- [Using Swock](#using-swock)
- [Supported apps](#supported-apps)
- [Privacy and the accessibility permission](#privacy-and-the-accessibility-permission)
- [Swock and other tools](#swock-and-other-tools)

---

## About Swock

### What is Swock?

Swock is an Android app that stops the swipe to the next video in short-video apps such as
TikTok, YouTube Shorts and Instagram Reels. The apps themselves keep working. You can watch the
current video, tap, like, comment and swipe sideways. Only the up and down swipe on the video
player is blocked.

### Where does the name come from?

It joins "swipe" and "block".

### Who is it for?

Swock is for people who want to keep using these apps but would rather not be carried from one
video to the next by a swipe, for example because they often scroll for longer than they meant to.

### How much does it cost?

Nothing. Swock is free and has no ads, in-app purchases or subscription.

### Is Swock open source?

No. Swock is proprietary and its source code is private. This public repository holds the
documentation: this FAQ, the [help page](SUPPORT.md), the [Privacy Policy](privacy-policy.md) and
the [Terms of Service](terms-of-service.md). You can still check that Swock has no internet
permission; see [Can I check this myself?](#can-i-check-this-myself)

### Is Swock a treatment for addiction?

No. Swock is a tool that adds friction to scrolling. It is not a medical device, a treatment for
addiction or a replacement for professional help. If you are struggling with how you use social
media, consider talking to a mental health professional.

---

## Setting up

### Which phones does Swock work on?

Phones with Android 13 or newer. Swock relies on a touch feature Android added in version 13, so
it cannot run on older versions. It also doesn't work reliably in emulators.

### Where do I download it?

From [GitHub Releases](https://github.com/Made-in-Jurgistan/swock-public/releases). Download the
APK file, open it on your phone and tap **Install**. The [README](README.md#install-and-set-up)
walks through every step.

### Why do I have to turn Swock on in Settings myself?

Android doesn't let any app switch on its own accessibility service. Only you can do it. Swock
shows the steps in a pop-up first, then opens the right Settings screen for you.

### I see "Restricted setting" and the switch won't turn on. What now?

That message is expected when you install Swock from a downloaded file, and a few extra taps fix
it. Android 13 and newer lock some settings for apps installed this way. Swock notices
this and guides you through three steps:

1. **Step 1 of 3: Find Swock.** Try the switch once. "Android says “Restricted setting”. That’s
   normal! Tap OK." Then "Press Back to return to Swock."
2. **Step 2 of 3: Allow Swock.** Tap **Open App info**, then "Tap ⋮ (three dots) in the top
   right corner." → "Tap Allow restricted settings." → "Confirm with your PIN, pattern or
   fingerprint." → "Press Back to return to Swock."
3. **Step 3 of 3: Turn on Swock.** Tap **Open settings**, then "Scroll down and tap Installed
   apps. (Some phones say Downloaded apps or Installed services.)" → "Tap Swock." → "Turn on the
   switch, then tap Allow." → "Press Back to return to Swock."

Each time you come back from Settings, Swock shows the next step by itself. The **Allow
restricted settings** option only appears after you have seen the "Restricted setting" message
in step 1. If you installed Swock another way, for example with adb, you only need the last
step.

### I tapped "Not now". How do I get the steps back?

Tap the button on the setup card in Swock. The pop-up opens again.

---

## Using Swock

### Can I still watch videos normally?

Yes. The video in front of you keeps playing, and you can pause, like, comment and share. Only
the swipe to the next or previous video is blocked.

### What else still works on the video player?

Almost everything. Taps and long-presses work, though a tap registers when you lift your finger,
so it responds a moment later than usual. Sideways swipes and two-finger gestures go straight to
the app. Opening the comments or share panel pauses blocking until you close it. If your phone
uses gesture navigation, swiping in from the left or right edge takes you back.

### Does Swock change anything outside the video player?

No. On search, profiles, home feeds, in other apps and on your home screen, Swock doesn't touch
your input at all.

### How can I tell Swock is working?

Look for the shield badge. While Swock is blocking swipes, a small badge that says "Swipe
blocked" appears at the top of the screen, as long as **Show indicator** is on. In Swock itself,
the status card says **Protecting** while it blocks and **Active** while it waits for a supported
app.

### What if I want to swipe to the next video?

Turn Swock off, fully or for one app. You can:

1. turn off **Swipe Blocking** in Swock,
2. switch off that app under **Protected Apps**, or
3. turn off Swock in Android's accessibility settings.

Swock makes getting to the next video take a deliberate step. It is not built to be impossible
to get around.

### Can I stop myself from just turning it off?

Not yet. Swock is an early version, an MVP (minimum viable product), and today anyone holding the
phone can turn blocking off in Swock, turn off the service in Android's accessibility settings,
or uninstall the app. PIN or password protection for turning off blocking in Swock is planned for a later version. Android's own settings and uninstalling
stay available either way, because no app can lock those.

### Can I turn Swock off for just one app?

Yes. Use the switches under **Protected Apps**. All supported apps are on when you install
Swock.

### Does Swock drain the battery?

Swock only does work while one of the 8 supported apps is open. Android sends it updates from
those apps and no others, and Swock checks the screen when one of them changes. While it is
protecting a player, it also checks every 0.4 seconds whether you are still there. With any other
app open, Swock receives no updates.

### Does it work in split-screen?

Partly. Swock only checks the app you are currently using, not the other half of the screen.

### Does it work with TalkBack?

Swock can run alongside TalkBack. It only uses Android's touch exploration mode while it
protects a video player, and it never switches that mode off for TalkBack. If something doesn't
work as expected, please
[report it](https://github.com/Made-in-Jurgistan/swock-public/issues).

### What happens if I uninstall Swock?

Blocking stops straight away and your Swock settings are deleted with the app. Nothing is left
anywhere else, because Swock never sent anything off your phone.

---

## Supported apps

### Which apps does Swock support?

Eight: TikTok, TikTok Lite, YouTube (Shorts), Instagram (Reels), Snapchat (Spotlight), Facebook
(Reels), Facebook Lite and Twitch (Clips). The [README](README.md#supported-apps) lists where
exactly Swock blocks the swipe in each.

### Does Swock block Instagram Stories?

No. Swock only blocks the Reels player. Stories use up and down swipes to close and reply, so
they are left alone.

### What about Snapchat Stories?

They may be blocked. In Snapchat, the Stories viewer shares screen signals with Spotlight, so
Swock can treat it the same way.

### Does Swock work if my apps are in another language?

For YouTube and Instagram, yes. For TikTok and Facebook, maybe not. Swock recognises those two
partly by English labels such as "For You", "Following" and "Reels, tab". If the app is set to
another language, Swock may not spot the player, and the swipe then works as normal.

### Will Swock keep working when an app updates?

Not always. Swock recognises each player by how the app's screen is built. If an
update changes that, Swock may stop recognising the player until Swock is updated. Please
[let us know](https://github.com/Made-in-Jurgistan/swock-public/issues) when that happens.

### Can you add another app?

Possibly. [Open an issue](https://github.com/Made-in-Jurgistan/swock-public/issues) with the app's
name and, if you can, a screenshot of its short-video player. Swock can only support an app if it
can reliably tell the short-video player apart from the app's other screens. Otherwise it would
have to block swipes everywhere in that app.

---

## Privacy and the accessibility permission

### Does Swock collect my data?

No. Swock has no internet permission and no analytics, tracking or crash reporting. Everything
happens on your phone. The [Privacy Policy](privacy-policy.md) has the details.

### What is an accessibility service, and why does Swock need one?

It is a kind of Android permission meant for tools that help people use their phone. It lets an
app look at what's on screen and respond to touches. It is also the Android feature that lets an app without root
access can filter touches in other apps. Swock uses it to recognise a Shorts or Reels player and
to stop the up and down swipe there.

### What can Swock see?

Only the layout of the 8 supported apps. Android sends Swock updates from those apps and no
others. Swock looks at the screen's building blocks, such as element names and labels, to decide
two things: is a short-video player showing, and is a comments or share panel open? It does not
save, log or send any text, passwords or personal information, and it forgets what it looked at
once it has decided.

### Android warns that Swock can see and control my screen. Should I worry?

The warning is real, but it is the same one Android shows for every accessibility service,
because the permission gives an app wide access. Swock uses it only to recognise video players and block one
swipe. Because Swock has no internet permission, it has no way to send what it sees anywhere.

### Does Swock sell or share my data?

No. Swock doesn't collect any data, so there is nothing to sell or share.

### Where are my settings stored?

On your phone, in storage only Swock can read. That covers the **Swipe Blocking** switch,
**Show indicator** and the per-app switches. They are left out of Android backups and transfers
to a new phone.

### Can I check this myself?

Yes. Any APK inspection tool, for example `aapt dump permissions` or an APK analyser app, shows
that Swock does not ask for the internet permission. Without it, Android does not let an app open
network connections.

---

## Swock and other tools

| Tool | What it limits |
|:-----|:---------------|
| Swock | The swipe to the next video on a Shorts or Reels player |
| App timers | How long you can use an app each day |
| App blockers | Whether you can open an app, or parts of it, at all |
| Delay-before-open tools | Opening an app, by adding a pause or task first |

### How is Swock different from app timers and app blockers?

Swock doesn't limit time or lock you out. Timers pause an app once your time is up, and blockers
keep you out of an app altogether. With Swock you can open the app and use it, but the swipe to
the next video on the player does nothing.

### How is it different from tools that add a delay before an app opens?

Those tools add a pause when you open an app. Swock works inside the app, at the moment you
would swipe to the next video.

### How is it different from just using willpower?

With Swock on, swiping doesn't move you on, so you don't have to decide not to swipe each
time. To swipe again, you switch Swock off.

### Can I use Swock alongside other digital wellbeing tools?

Yes. Swock only acts on the up and down swipe in the video players of the 8 supported apps, so
it can run alongside screen time apps and app blockers.

---

Still stuck? See [Help and troubleshooting](SUPPORT.md), or
[open an issue](https://github.com/Made-in-Jurgistan/swock-public/issues).

<div align="center">

<sub>© 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
