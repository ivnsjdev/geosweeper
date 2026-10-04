# Privacy Policy for GeoSweeper

**Effective date:** 26 September 2026

**Last updated:** 4 October 2026

## The short version

GeoSweeper does not collect, transmit, sell, or share any personal information. Every
board you play, every setting you pick, and every country you've cleared is stored only on
your device. Nothing is uploaded to us, and there is no account to create in the first
place. The only network traffic GeoSweeper ever generates is StoreKit talking to Apple when
you make or restore a purchase, and pages you deliberately open from a link inside the app
(this site, or Apple's own legal pages) — both are covered below, and neither carries
anything else with it.

## Who we are

GeoSweeper is developed by Ivan Cayabyab. Questions about this policy or the app can be
sent to ivnsjdev@gmail.com.

## What the app stores, and where

Everything below lives only on your device, in one of three places: `UserDefaults` (small
settings values), a JSON file in the app's own Application Support folder, or a local
SQLite database.

| What | Primary storage | Sent automatically to us? |
|---|---|---|
| Display settings — board theme, neon color, explosion effect, blast sound, map projection (globe or flat), sound and haptics on/off | `UserDefaults` | No |
| Language you've chosen inside the app | `UserDefaults` | No |
| Rating-prompt bookkeeping — the dates GeoSweeper has asked iOS to show the native rating sheet, and which milestone triggered the last one | `UserDefaults` | No |
| Free-games counters — how many of your 10 free map countries and 10 free Classic games you've used | `UserDefaults` | No |
| Per-country record — wins, losses, best time, and when you unlocked it, for every country you've played | A JSON file (`progress.json`) in the app's Application Support folder | No |
| Classic mode history — the board size, difficulty, mine count, time, and win-or-loss of every finished Classic game | A JSON file (`Classic/history.json`) in the app's Application Support folder | No |
| Infinite Tower progress — the row you've reached, your saved viewport, and which rows you've cleared | A local SQLite database | No |

None of this is transmitted, sold, or shared with anyone, including us. StoreKit's own
traffic (below) and the external links you tap (also below) carry none of it. An iOS device
backup may include these files as part of backing up the app as a whole — that backup is
initiated by you or by iOS, never by GeoSweeper, and it stays wherever you send it (iCloud
or your computer), not with us.

## No account, no sign-in, no cloud

GeoSweeper never asks for a name, email address, phone number, date of birth, or any other
identifying information — there is nothing to sign in with, because there is no account.
Your progress does not sync through iCloud, CloudKit, or any other service: it lives only
on the device you're playing on. Play the same country on a second device and it starts
fresh there, because there is no server copy anywhere to sync from.

## Anything deliberately not persisted

The board you're in the middle of — every tile you've opened, every flag you've placed — is
held only in memory while you play. This is true in all three worlds: the map, Classic mode,
and Infinite Tower. Close the app mid-game and that board is gone; it is never written to
disk, and there is no autosave to resume an unfinished board from. Only a *finished* game (a
win or a loss) updates the per-country record or the Classic history described above.

## The one thing that sounds like it isn't local

The map opens on your own country the first time you launch the app. This comes from your
device's **region setting** (the country tied to your language and locale, the same one iOS
uses to pick a keyboard and a calendar) — not from GPS, Wi-Fi, or any other form of location
tracking. GeoSweeper does not request location access and could not read your coordinates
even if it wanted to.

## Permissions

GeoSweeper requests no system permissions whatsoever. It never asks for the camera, photo
library, microphone, location, contacts, calendar, health data, motion data, or push
notifications, and no permission prompt of any kind will ever appear. This matches the
app's `Info.plist` exactly: there is not a single usage-description entry in it.

## Purchases

GeoSweeper is free to download, and each of its three worlds has its own free trial. Your
first 10 countries on the map — any tier, Beginner included — are free to play, and once
you've played a country it stays replayable for good, even after that trial is spent.
Classic mode gives you 10 free games the same way. Infinite Tower is free up to row 10.
Beyond those points, there are three independent purchases, all one-time, non-consumable,
and offered through Apple's StoreKit and processed entirely by Apple:

- **All Countries** — a one-time, non-consumable purchase that permanently unlocks the
  Intermediate, Expert, and Mega tiers across all 204 countries. Nothing about this renews.
- **Classic Lifetime** — a one-time, non-consumable purchase that permanently unlocks
  unlimited Classic games once your 10 free ones are spent. Nothing about this renews.
- **Infinite Tower Lifetime** — a one-time, non-consumable purchase that permanently unlocks
  climbing past row 10. Nothing about this renews either, and GeoSweeper offers no
  subscription of any kind.

Apple, not GeoSweeper, processes every payment. No card number, billing address, or Apple
Account credential is ever visible to us — StoreKit only tells the app what it needs to
show a paywall and grant access: the price to display, and whether you currently own each
item. Those answers stay on your device; GeoSweeper does not run a purchase server of its
own and has nowhere to send them. Restoring purchases asks Apple to re-confirm what your
Apple Account owns and applies the answer locally — it does not create or transmit any new
record.

See also Apple's [App Store & Privacy](https://www.apple.com/legal/privacy/data/en/appstore/),
the [Media Services Terms](https://www.apple.com/legal/internet-services/itunes/), and the
[Standard EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/), which
govern the purchase itself.

## Support communications

If you email ivnsjdev@gmail.com, we receive your email address, whatever you write, and any
attachment you choose to add. We use it only to answer you and to fix the problem you wrote
in about — our lawful basis is our legitimate interest in responding to people who contact
us. That mailbox is a standard Gmail account, processed by Google LLC under
[Google's Privacy Policy](https://policies.google.com/privacy), and hosted on infrastructure
that may be located outside your own country, which is why that transfer is disclosed here.
We keep support emails for up to 24 months and then delete them; you can ask us to delete a
specific email sooner at any time by writing to the same address.

## External links

GeoSweeper's paywalls link to this site's own privacy policy and to Apple's Standard EULA;
Settings can link to the App Store's write-a-review page. No user data or app-specific
identifier is appended to any of these links — they are plain URLs, the same for everyone.

## Nothing to wager

GeoSweeper has no in-app currency, no loot, no prize draws, and no feature where an outcome
is staked or wagered. Every purchase is a fixed, disclosed price for permanent or
time-boxed access to content; nothing can be won, lost, or gambled.

## What we do NOT do

- No analytics, crash reporting, or telemetry of any kind
- No advertising, no ad networks, and no advertising identifiers
- No cross-app or cross-site tracking, and no data brokers
- No accounts, no sign-in, no passwords
- No camera, photo library, microphone, contacts, precise or coarse location, or health data
- No training of machine-learning models on your data
- No third-party SDKs of any kind — the only code in this app is our own

This matches the "Data Not Collected" label GeoSweeper carries on the App Store.

## Retention and deletion

Deleting the app deletes every file it stored on your device — settings, your per-country
record, Classic history, and Infinite Tower progress — immediately and completely, because
there was never a server copy for us to hold onto or to delete on our end. An iCloud device
backup made before deletion may still contain a copy; that backup is entirely under your control
through **Settings → your name → iCloud → Manage Account Storage** on your device. Support
emails are retained and deleted separately, as described above.

## Your rights

Because GeoSweeper keeps no copy of your in-app data, the access, correction, export, and
deletion rights that GDPR, UK GDPR, and the CCPA/CPRA describe are ones you already exercise
directly, on your own device — there is no record here for us to produce or erase on your
behalf. The one place we do hold something is a support email you've sent us, and you can
ask to see, correct, or delete that at any time by writing to ivnsjdev@gmail.com. We do not
sell or share personal information for cross-context behavioral advertising, and never have.
If you believe we have mishandled your data, you have the right to lodge a complaint with
your local data protection authority.

## Children

GeoSweeper carries an age rating suitable for a general audience and is not directed at
children specifically. We do not knowingly collect personal information from anyone,
including children under 13, and there is nothing in the app that could — no chat, no
sharing, no social feature, no advertising, and no account for a third party to reach a
child through.

## Changes to this policy

If this policy changes, the date at the top will change with it, and a material change to
what GeoSweeper does with data will also be noted in that update's release notes.

## Contact

ivnsjdev@gmail.com
