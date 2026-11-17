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

## B8: Home Assistant and menu search

- **Menu → Search** finds available functions as you type, shows their menu path and follows your user level. Group or outing selection appears where needed.
- **Groups and sharing → Home Assistant** shares your selected own daily figures through a dedicated, revocable key.
- Optional own leadership status covers today, the last 7 and the last 30 days, separating measured activity and goal achievement. No other members' names or figures are exported.
- The new sharing setup and Home Assistant integration support English and Norwegian. The rest of the Android app is not fully translated.
- [Home Assistant setup and beta limitations](https://github.com/trondtorsoe/Tur---HA-integrasjon).

B8 is an optional beta. The server must be updated with its matching package before the new Home Assistant connection works. Stable 0.20 users are not forced to update.

## Installation and updates

**[Download Tur 0.20 B8 APK](https://drive.google.com/file/d/1XXxspnAR8W0Kc5zFWoHol59_F2ru-6PH/view).** The APK is hosted on Google Drive. The matching B8 server package must be installed by the server administrator before Home Assistant sharing works. No APK is stored directly in this repository yet. Install updates over the existing app to preserve local records; do not uninstall first. Read release notes and known limitations before installing a beta.

## Privacy and this repository

This repository is for public documentation, release notes and APK distribution. App and server source code remain private. Do not upload personal activity data, GPS tracks, credentials, keys, databases or production logs here, including in public issues.
