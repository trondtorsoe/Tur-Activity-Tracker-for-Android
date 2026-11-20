# Tur – Activity Tracker for Android

[English](README.md) | [Norsk](README.nb.md)

**Latest stable Android release: 0.23 (version code 84).** The separate Home Assistant integration remains beta (0.20.2b3); Homey 0.1.1 is a local test package.

Tur records everyday activity and outings on Android, helps you follow your progress and lets you choose what to share.

## Tur 0.23 release notes

- The sponsor overview shows status, views, clicks and a weekly chart. Administrators can share reports, preview and select campaign images, create sponsor pages and receive image suggestions.
- Sponsors can use campaign tracking (UTM) with an optional campaign name. Existing UTM values are preserved. Administrators can preview sponsor links.
- The sponsor banner has smoother transitions, improved spacing and manual browsing. Hidden sponsors can be shown again. Visibility for beta users is configurable per sponsor.
- Administrators can share a single internal build via a 24-hour link. The recipient confirms installation in Android.
- Tur’s release history collects the changes from 0.22 B1–B14.

## Tur 0.22 release notes

- Sponsored campaigns rotate on the home screen. Closing the compact sponsor row hides it for 24 hours. Administrators can configure multiple sponsors, choose stable and beta visibility independently, and share date-based reports with CSV downloads.
- Release history combines changes from the 0.21 beta series and shows entries relevant to your role. Menu search and tips lead to the feature.
- The beta series added private outing photo albums, updated activity selection and registration, number wheels, language selection, group cards and sharing settings, location maps and participant colours, revocable outing links, remote setup help with codes, and targeted stable or beta update offers.

## Install and update

**[Download Tur 0.23 APK](Tur-0.23.apk?raw=true)**

Install **Tur.apk** over your existing app. Do not uninstall first: local records and settings should be retained. 0.23 has a higher version code than 0.22 B14.

You can also use **Settings → Check for app updates** in Tur. App updates do not require a PC. Server administrators can select the signed **tur-oppdater.py** under **Administration → Server update** in the phone app, or use the supplied **LastOpp-Tur.ps1** from their synced Drive folder. Server administration requires an administrator key; ordinary users do not need to update the server.

## New in 0.21

- The home icon opens the main menu at the upper left; menu search is at the upper right. Search includes nested functions such as feedback and shows their full menu path.
- Advanced view can be enabled by tapping the **Tur** heading inside the open main menu ten times, then waiting for the prompt.
- All 56 feature tips show a menu path. **Show more / Show less** expands explanations and a simple path illustration. Read timestamps and hidden-tip choices survive content revisions.
- Outing details have **Back to outing list** and a poodle toggle labelled **Uten hund / Med hund** (Without dog / With dog). The matching poodle appears in tips and on dog outings in the list. The flag survives recording updates and does not change points or measurements.
- Ongoing movement below 500 metres belongs under **Movement**, rather than recent outings.
- Home Assistant sharing supports selected figures, app group names, and revocable keys. Expected rejection of an invalid or revoked key no longer creates a server program-error report.

## Activity, outings and journeys

- Automatic recording with phone sensors; background recording depends on Android permissions and battery restrictions.
- Steps and daily totals, activity distance, known ascent, training minutes, goals and calculated points.
- GPS routes, speed and elevation information where available; history by day, week, month and year.
- Manual exercise entries with editing and deletion.
- Car, train, boat and bus transport legs retain travel details without activity credit.
- Combine compatible saved activity and transport legs into a journey. Originals remain available and count once in activity totals.
- Half-hour activity breakdowns follow existing sharing choices and require compatible clients and fresh uploaded data.

## Groups and optional sharing

Create groups, invite others, and compare shared measured activity and goal achievement separately. App installation links and group invitations are separate functions.

Share selected outings or periods through revocable viewing links. Personal links do not require group membership. Name visibility and GPS sharing need separate permission; group links show Anonymous unless name display is approved. Start/end masking reduces location exposure but does not guarantee anonymity. Revoking a link cannot recall a copy already saved by a recipient.

## Home Assistant and Homey

In Tur: **Groups and sharing → Home Assistant**. Choose your own figures, create a read-only key and paste it into the integration. Optional own leadership covers today, the last 7 and last 30 days; other members' names and figures are not exported.

[Home Assistant setup and current test status](https://github.com/trondtorsoe/Tur---HA-integrasjon). Requires Home Assistant 2026.11 or newer. Tur is currently installed from its repository link, not listed in the default Marketplace catalog. Integration 0.20.2b3 has been tested with Tur app/server 0.21; integration and Android version numbers are independent.

Homey 0.1.1 is a separate local test package with an installation guide, not a published Homey App Store app. Physical Homey testing remains outstanding. The HA/Homey sharing setup and HA integration support English and Norwegian; the Android app is not fully translated.

## Verification and limitations

The 0.21 release passed 217 server tests, 14 Android database/menu tests, Android Java regression checks including 129 search entries and all 56 tips, 11 tests against actual Home Assistant 2026.11 over local TLS, and 17 Homey tests against the 0.21 server. APK signing and alignment, signed server-package integrity, and upgrade preservation were checked.

User-confirmed HA behaviour includes matching figures, sharing-choice changes, app group names and icon, key replacement and revocation, and no new unknown placeholder sensors. Manual confirmation of 7/30-day comparisons, later automatic sensor creation, restart/rename history preservation and local aliases remains outstanding. These checks do not constitute physical testing of every Android screen or Homey hardware.

## Privacy and this repository

This repository contains public documentation and download links. App and server source remain private. Do not post personal activity data, GPS tracks, credentials, keys, databases or production logs, including in public issues.
