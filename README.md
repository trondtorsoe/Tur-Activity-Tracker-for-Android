# Tur – Activity Tracker for Android

[English](README.md) | [Norsk](README.nb.md)

> **BETA — under active development. This is not a thoroughly tested product. Expect bugs, incomplete features and changes.**

Tur records everyday activity and outings on Android, helps you follow your progress and lets you choose what to share with others.

## Activity and outings

- Automatic activity recording using the phone's sensors, with background recording subject to Android permissions and battery restrictions.
- Steps and daily activity totals, activity distance, elevation gain and training minutes.
- Recorded outings with GPS maps, speed and elevation information where available.
- Activity goals, calculated activity points and progress over time.
- History organised by day, week, month and year, with summaries and charts.
- Manual activity entries for exercise without the phone, with editing and deletion.

## Groups and optional sharing

- Create groups, invite people and compare shared activity and goal achievement.
- Share selected outings and activity periods; app installation links and group invitations are separate.
- Personal viewing links work without joining a group. Choose expiry, name visibility and optional GPS sharing.
- Group viewing links show a member as Anonymous unless name display has been approved. GPS permission is separate.
- Viewing links can be revoked. A recipient's saved copy cannot be recalled.
- GPS start/end masking reduces location exposure but does not guarantee anonymity.

## B7 beta features

These features are described by the current B7 source package. This does not mean the package has been installed on the production server or tested on a physical phone.

- Half-hour activity breakdowns follow existing activity-sharing choices. Compatible clients and server software are required; stable 0.20 does not send half-hour breakdowns.
- Car, train, boat and bus transport legs retain route and travel details without contributing activity credit.
- Combine compatible saved legs into a journey, including different activities and transport. Original legs remain available and are counted once in activity totals.
- A dedicated Share my activity entry and separate name/GPS consent for viewing links.

## Installation and updates

APK files and release-specific notes will be added when ready. **No APK has been published in this repository yet.** Install updates over the existing app to preserve local records; do not uninstall first. Read release notes and known limitations before installing a beta.

## Home Assistant — in development

A dedicated key-based integration is being developed in [Tur Home Assistant](https://github.com/trondtorsoe/Tur---HA-integrasjon). It is not ready to install. Planned sharing is read-only access to your own approved activity figures, without group data or GPS. MQTT work is deferred.

English documentation does not mean the entire Android interface has been translated. Norwegian and English support is planned first for the new integration and key setup.

## Privacy and this repository

This repository is for public documentation, release notes and APK distribution. App and server source code remain private. Do not upload personal activity data, GPS tracks, credentials, keys, databases or production logs here, including in public issues.

Only the separate Home Assistant integration source code is intended for public publication.
