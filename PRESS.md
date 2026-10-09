<div align="center">

<img src="swock_logo.png" width="120" alt="Swock">

# Press Kit

</div>

Facts, ready-to-use descriptions and assets for journalists, reviewers and creators writing about
Swock. Everything here can be quoted or reused.

## Contents

- [Quick facts](#quick-facts)
- [Descriptions](#descriptions)
- [Boilerplate](#boilerplate)
- [How Swock works](#how-swock-works)
- [Privacy](#privacy)
- [How Swock compares with other tools](#how-swock-compares-with-other-tools)
- [Questions journalists ask](#questions-journalists-ask)
- [Research](#research)
- [Logo and assets](#logo-and-assets)
- [Media contact](#media-contact)
- [Describing Swock accurately](#describing-swock-accurately)

---

## Quick facts

| | |
|:--|:--|
| **Name** | Swock |
| **What it does** | Blocks the swipe to the next video in short-video apps |
| **Developer** | Made in Jurgistan |
| **Platform** | Android 13 or newer |
| **Version** | 1.0.0 |
| **Status** | MVP (minimum viable product) |
| **Supported apps** | 8: TikTok, TikTok Lite, YouTube (Shorts), Instagram (Reels), Snapchat (Spotlight), Facebook (Reels), Facebook Lite, Twitch (Clips) |
| **App size** | About 2.3 MB |
| **Price** | Free |
| **Ads or in-app purchases** | None |
| **Data collected** | None |
| **Internet permission** | None |
| **Root required** | No |
| **License** | Proprietary, all rights reserved (not open source) |
| **Download** | [GitHub Releases](https://github.com/Made-in-Jurgistan/swock-public/releases) |
| **Website** | [github.com/Made-in-Jurgistan/swock-public](https://github.com/Made-in-Jurgistan/swock-public) |

---

## Descriptions

### One line

> Swock is an Android app that blocks the swipe to the next video in short-video apps, without
> blocking the apps themselves.

### Short

> Swock blocks the up and down swipe that loads the next video in TikTok, YouTube Shorts,
> Instagram Reels and five other short-video apps. The video in front of you keeps playing, and
> you can still tap, like, comment, share and swipe sideways. Swock needs no root access, has no
> internet permission and collects no data.

### Long

> Swock is a digital wellbeing app for Android. It acts on a single gesture in short-video apps:
> the up and down swipe on the video player that loads the next or previous video.
>
> When you open the Shorts or Reels player in one of 8 supported apps (TikTok, TikTok Lite,
> YouTube, Instagram, Snapchat, Facebook, Facebook Lite and Twitch), Swock recognises it and stops
> that swipe. The rest of the app keeps working: the video plays, taps work, sideways swipes
> work, and you can like and comment. Opening the comments or share panel pauses blocking. On
> every other screen, and in every other app, Swock leaves touches alone.
>
> Swock runs entirely on the phone. It has no internet permission and no analytics, tracking or
> crash reporting, and it needs no root access.
>
> Swock is an MVP (minimum viable product). Today anyone holding the phone can turn blocking off.
> PIN or password protection for turning off blocking in Swock is planned for a later version.

---

## Boilerplate

> **About Made in Jurgistan.** Made in Jurgistan is an independent software developer and the
> maker of Swock, an Android app that blocks the swipe to the next video in short-video apps.
> Swock is free, collects no data and runs entirely on the phone.

---

## How Swock works

Swock uses an Android **accessibility service**. This is a kind of Android permission meant for
tools that help people use their phone; it lets an app look at what's on screen and respond to
touches. Android doesn't let apps switch this on themselves, so the user turns it on once in
Settings, with Swock showing each step.

Once it is on, Swock:

1. **Recognises** when you are on a short-video player in a supported app, such as TikTok's For
   You feed, YouTube Shorts or Instagram Reels. Instagram Stories and the apps' other screens are
   not affected.
2. **Stops** the up and down swipe that would move to another video.
3. **Passes on** every other touch. Taps and long-presses go through as soon as you lift your
   finger, and sideways swipes and two-finger gestures go straight to the app. On phones with
   gesture navigation, swiping in from the edge still goes back.

When you leave the player, close the app or open the comments, Swock stops filtering touches. An
optional shield badge reading "Swipe blocked" shows while blocking is active.

---

## Privacy

| Question | Answer |
|:---------|:-------|
| Does Swock collect personal data? | No |
| Does it use analytics or tracking? | No |
| Can it go online? | No. It does not ask for the internet permission. |
| Does it store anything in the cloud? | No. Its settings stay on the phone and are left out of Android backups. |
| Does it read the screen? | It looks at the screen layout of the 8 supported apps, on the phone, to recognise video players. It does not save, log or send any text, passwords or personal information. |
| Does it sell or share data? | No. There is no data to sell or share. |

Full details are in the [Privacy Policy](privacy-policy.md).

---

## How Swock compares with other tools

| Tool | What it limits | Works on a single gesture? |
|:-----|:---------------|:---------------------------|
| **Swock** | The swipe to the next video on Shorts and Reels players | Yes |
| App timers | How long you can use an app | No |
| App blockers | Whether you can open an app, or parts of it | No |
| Delay-before-open tools | Opening an app, by adding a pause or task first | No |

Swock doesn't limit time and doesn't lock anyone out. People can open the app, watch a video,
like, comment and share. The swipe on the player just doesn't load the next video.

---

## Questions journalists ask

### Is Swock anti-TikTok?

No. It isn't aimed at any one platform and works the same way in all 8 supported apps. It
doesn't stop anyone using those apps. It removes one swipe on their short-video players.

### Is Swock an addiction treatment?

No. Swock is a digital wellbeing tool, not a medical device or treatment. Anyone struggling with
serious compulsive use should talk to a mental health professional.

### Does Swock spy on what people do?

No. Swock has no internet access and collects no data. It looks at the layout of the screen, on
the phone, to work out whether a video player is showing, and then forgets it. No text,
passwords or personal information is stored or sent.

### Why isn't Swock open source?

Swock is proprietary and its source code is private. How it handles data is set out in the
public [Privacy Policy](privacy-policy.md), and anyone can inspect the APK to confirm that it
does not ask for the internet permission.

### How does Swock make money?

It doesn't. Swock is free, with no ads and no in-app purchases.

### Can people get around Swock?

Yes. Anyone holding the phone can turn Swock off, fully or for one app, at any time, or uninstall
it. It makes getting to the next video a deliberate step rather than an impossible one. PIN or password protection for turning off blocking in Swock is planned for a later version.
Android's own settings and uninstalling stay available either way, because no app can lock those.

### Why Android only?

Swock relies on a touch-filtering feature that Android added in version 13. There is no iPhone
version.

---

## Research

These peer-reviewed studies look at short-form video and endless scrolling. **None of them
tested Swock.** Correlational findings show a link, not a cause. When citing them, please keep
that distinction.

1. **Nguyen, L., Walters, J., Paul, S., Monreal Ijurco, S., Rainey, G. E., Parekh, N., Blair, G.,
   & Darrah, M. (2025).** Feeds, feelings, and focus: A systematic review and meta-analysis
   examining the cognitive and mental health correlates of short-form video use. *Psychological
   Bulletin, 151*(9), 1125–1146.
   [doi:10.1037/bul0000498](https://doi.org/10.1037/bul0000498)

   A meta-analysis of 71 studies with 98,299 participants. Heavier short-form video use was
   associated with poorer cognition (r = −.34), most strongly attention (r = −.38) and inhibitory
   control (r = −.41), and with poorer mental health (r = −.21), most strongly stress (r = −.34)
   and anxiety (r = −.33). Use was not associated with body image or self-esteem. The findings
   are correlational.

2. **Luo, W., Zhao, X., Jiang, B., Fu, Q., & Zheng, J. (2025).** Swiping disrupts switching:
   Preliminary evidence for reduced cue-based preparation following short-form video exposure.
   *Behavioral Sciences, 15*(8), 1070.
   [doi:10.3390/bs15081070](https://doi.org/10.3390/bs15081070)

   A randomized experiment with 72 participants, who watched 30 minutes of TikTok-style content,
   a neutral documentary, or no video, then did a task-switching test. The documentary and
   no-video groups benefited from extra preparation time; the short-video group did not. Quick
   responses did not differ between groups. The authors describe the evidence as preliminary.

3. **Ma, L., & Jiang, Q. (2024).** Swiping more, thinking less: Using TikTok hinders analytic
   thinking. *Cyberpsychology: Journal of Psychosocial Research on Cyberspace, 18*(3), Article 1.
   [doi:10.5817/CP2024-3-1](https://doi.org/10.5817/CP2024-3-1)

   Two experiments with young adults. In the first (67 participants), 30 minutes of TikTok was
   followed by lower scores on a reasoning test than reading an e-book. In the second (178
   participants), swiping through the feed, rather than the video content, reduced people's
   tendency to think analytically.

4. **Park, J., & Jung, Y. (2024).** Unveiling the dynamics of binge-scrolling: A comprehensive
   analysis of short-form video consumption using a Stimulus-Organism-Response model.
   *Telematics and Informatics, 95*, 102200.
   [doi:10.1016/j.tele.2024.102200](https://doi.org/10.1016/j.tele.2024.102200)

   A mixed-methods study that linked infinite scrolling with a reduced sense of self-control among
   short-form video users, which in turn was linked with regret.

5. **Ruiz, N., Molina León, G., & Heuer, H. (2024).** Design frictions on social media: Balancing
   reduced mindless scrolling and user satisfaction. In *Proceedings of Mensch und Computer
   2024* (pp. 442–447).
   [doi:10.1145/3670653.3677495](https://doi.org/10.1145/3670653.3677495)

   A study with 30 participants comparing infinite scroll with an interface that required a
   reaction to each post before the next one appeared. People using the slower interface
   remembered the posts significantly better, though most found it frustrating.

---

## Logo and assets

| Asset | Format | Where |
|:------|:-------|:------|
| App logo | PNG | [`swock_logo.png`](swock_logo.png) in this repository |

For other assets, interviews or questions, use the contact below.

---

## Media contact

Contact the developer through
[GitHub Issues](https://github.com/Made-in-Jurgistan/swock-public/issues) on the public
repository, or via the [Made in Jurgistan](https://github.com/Made-in-Jurgistan) GitHub profile.

---

## Describing Swock accurately

When you write about Swock, please:

1. link to the public repository: `https://github.com/Made-in-Jurgistan/swock-public`,
2. describe the privacy accurately: Swock collects no data and has no internet access, and
3. describe the scope accurately: Swock blocks one swipe, not the app.

Please avoid calling Swock:

- an "app blocker" or "TikTok blocker", because it blocks a gesture, not an app,
- a medical treatment or addiction cure, or
- impossible to get around, because it can be turned off at any time.

More background: [README](README.md) · [FAQ](FAQ.md) · [Privacy Policy](privacy-policy.md) ·
[Terms of Service](terms-of-service.md)

<div align="center">

<sub>© 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
