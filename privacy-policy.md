<div align="center">

<img src="swock_logo.png" width="100" alt="Swock">

# Privacy Policy

**Swock — Swipe Blocker for Short Videos**

**Last updated: 2026-08-08**

</div>

---

## Contents

- [Overview](#overview)
- [Data collection](#data-collection)
- [Permissions](#permissions)
- [Accessibility service](#accessibility-service)
- [Play Integrity API](#play-integrity-api)
- [Data storage](#data-storage)
- [Third-party services](#third-party-services)
- [Children's privacy](#childrens-privacy)
- [Changes to this policy](#changes-to-this-policy)
- [Contact](#contact)

---

## Overview

<div align="center">

**Swock collects no data.**

**No network access. No analytics. No telemetry. Everything runs locally on your device.**

</div>

This privacy policy describes what information Swock does and does not collect, how it uses
permissions, and your rights regarding your data.

---

## Data collection

| Data type | Collected? | Purpose |
|:----------|:-----------|:--------|
| Personal information | **No** | — |
| Device identifiers | **No** | — |
| Usage analytics | **No** | — |
| Crash reports | **No** | — |
| Network traffic | **No** | No INTERNET permission |
| Accessibility node content | Processed locally, not stored or transmitted | Screen classification |
| Touch events | Processed locally, not stored or transmitted | Gesture classification |
| App preferences | Stored locally on device | User settings (enabled apps, toggles) |

Swock does not transmit any data off your device. There is no backend server, no cloud
synchronisation, and no third-party data sharing.

---

## Permissions

| Permission | Type | Required? | Purpose |
|:-----------|:-----|:----------|:--------|
| `BIND_ACCESSIBILITY_SERVICE` | System | Yes | Intercept touch gestures |
| `INTERNET` | Normal | **No** | Not declared — Swock has no network access |
| `ACCESS_NETWORK_STATE` | Normal | **No** | Not declared |
| `READ/WRITE_EXTERNAL_STORAGE` | Dangerous | **No** | Not declared |
| `CAMERA` | Dangerous | **No** | Not declared |
| `RECORD_AUDIO` | Dangerous | **No** | Not declared |
| `ACCESS_FINE_LOCATION` | Dangerous | **No** | Not declared |

Swock declares only the accessibility service permission. No dangerous or network permissions
are requested.

---

## Accessibility service

Swock uses the Android Accessibility Service to intercept touch gestures in short-form video
apps.

**What the service does:**
- Receives raw touch event data and inspects the accessibility node tree of the foreground app
  to classify whether the current screen is a Shorts/Reels player

**What the service does not do:**
- Does not read, log, store, or transmit text content, credentials, personal data, or any other
  information from the accessibility node tree
- Node tree inspection is used solely to determine screen type (Shorts feed vs. other screens)
  and is discarded immediately after classification

**Touch data:**
- Raw touch events are classified in real-time (swipe vs. tap vs. horizontal swipe) and then
  discarded. No touch data is stored or transmitted.

**Scope:**
- The service only activates for apps the user has explicitly enabled in Swock's settings
- It does not monitor apps the user has not selected

---

## Play Integrity API

Swock uses the Google Play Integrity API to verify that the app has not been tampered with or
repackaged. This API sends the following to Google's servers:

| Data sent to Google | Purpose |
|:--------------------|:--------|
| App package name | Verify app identity |
| Nonce (cryptographically random value) | Prevent replay attacks |
| Device integrity signals | Verify genuine Android device |

Google's Play Integrity API is governed by
[Google's Privacy Policy](https://policies.google.com/privacy). The integrity token is requested
on app launch and contains no personal information. Swock does not currently have a backend
server to verify the token — the request is made to Google's services directly from the app.

---

## Data storage

All user preferences are stored locally on the device using Android's DataStore. This data never
leaves the device.

| Data stored | Location | Encrypted? |
|:------------|:---------|:-----------|
| Master toggle (enabled/disabled) | App-private DataStore | No (not sensitive) |
| Enabled app packages | App-private DataStore | No (not sensitive) |
| Show indicator toggle | App-private DataStore | No (not sensitive) |

No data is stored in external storage, shared preferences accessible by other apps, or any
cloud service.

---

## Third-party services

| Service | Purpose | Data shared |
|:--------|:--------|:------------|
| Google Play Integrity API | App integrity verification | Nonce, package name, device signals — see [Google's privacy policy](https://policies.google.com/privacy) |
| Google Play Store | App distribution | Governed by Google's terms |

No other third-party services are used. No analytics SDKs, no advertising SDKs, no crash
reporting SDKs are included.

---

## Children's privacy

Swock is not directed at children under 13 and does not knowingly collect any personal
information from children. Since Swock collects no data from any user, no special protections
for children's data are required.

---

## Changes to this policy

The copyright holder may update this privacy policy from time to time. Changes will be posted in
this document with an updated "Last updated" date. Continued use of Swock after changes
constitutes acceptance of the revised policy.

---

## Contact

For privacy questions or concerns, contact the maintainer via
[GitHub](https://github.com/Made-in-Jurgistan/swock-public/issues).

---

<div align="center">

<sub>© 2026 Made in Jurgistan. All rights reserved.</sub>

</div>
