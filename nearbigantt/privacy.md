# Privacy Policy

**Last Updated: July 24, 2026**
**Version: 1.2**

INX Company Limited ("we", "our", "us") operates the NearbiGantt application. This Privacy Policy explains how we collect, use, and protect your information when you use our app.

NearbiGantt is a **local-first** team task management app with a Gantt timeline, designed for local networks. We do **not** operate any servers that receive your personal information, we do **not** display advertisements, and we do **not** run first-party analytics or crash-reporting SDKs. Your data lives on your own device and, when you enable sync, in **your personal iCloud account** managed by Apple.

## Information We Collect

### Profile Information

- When you set up the app, you provide a **display name** and may optionally add an **email address** and a **profile photo**.
- This profile information identifies you to teammates with whom you share projects, tasks, or chats.
- It is stored on your device and, when iCloud sync is enabled, in your personal iCloud container (`iCloud.com.inx.nearbigantt`). When you share content with a teammate, the profile fields needed to display "who shared this" are included with the shared item.
- We do **not** receive or store your profile on any server we operate.

### Content You Create

- Projects, tasks, to-dos, comments/memos, group-chat messages, and any photos or files you attach are stored on your device and, if you enable iCloud sync, in your personal iCloud container.
- When you choose to share a project, task, or chat with a teammate, the relevant content is synced through Apple's CloudKit sharing or sent directly to nearby devices (see "Local Network Sharing" below). It is never routed through a server we control.
- Chat message text is stored **unencrypted** by NearbiGantt (it relies on Apple's iCloud encryption in transit and at rest, not an additional end-to-end layer). Once a message or shared item is delivered, a copy exists in your teammate's device and iCloud — so, as with email or any messaging app, deleting your own copy or resetting your device does not remove the copy already delivered to them. Ask your teammate to delete their copy if you need it removed on their side.

### iCloud Data (CloudKit)

- If you enable iCloud sync, your projects, tasks, profile, and chats are stored in your personal iCloud container and kept in step across your own devices signed in to the same Apple ID.
- This data is managed entirely by Apple's iCloud service and is encrypted in transit and at rest by Apple. We do **not** have access to your iCloud data.

### Calendar Access

- With your permission, NearbiGantt reads and creates events in your **Apple Calendar** so they appear alongside your tasks in the timeline.
- Calendar data is handled by Apple's EventKit on your device. It is **not** transmitted to us or to any third party.
- You can grant or revoke Calendar access at any time in your device settings. The app works without it.

### Public Holidays

- To show public holidays on your timeline, NearbiGantt uses your device's own system holiday calendar where available. For a region your device does not cover, it fetches holiday dates from a third-party public API (Nager.Date, `date.nager.at`). Only a **country/region code and a year** are sent — never your personal data, identifiers, or content. You can turn holiday display off in Settings.

### Photos

- When you choose a profile photo or attach an image, the app uses Apple's system photo picker. Only the specific image you select is imported into the app — we do **not** access your photo library otherwise, and the app does **not** request full photo-library permission.

### Local Network Sharing

- NearbiGantt can discover nearby teammates and share tasks and team holidays over the local network using Apple's **MultipeerConnectivity** framework (Bonjour service `_nearbigantt-sh`).
- The app requests **Local Network** permission to discover and connect with nearby devices.
- All communication happens **directly between nearby devices** and is **not routed through any external server**.
- To avoid creating duplicate entries when the same person uses more than one device, the app broadcasts a one-way **SHA-256 hash** of your iCloud account identifier over the local network. This hash is not reversible to your identity and is used only for de-duplication.

### Push Notifications

- With your permission, the app uses Apple's Push Notification service (via CloudKit subscriptions) to notify you about shared items, comments, and messages.
- Notification delivery is handled by Apple. You can disable notifications at any time in your device settings.

### In-App Purchases

- NearbiGantt offers two optional in-app purchases: **NearbiGantt Package**, a **one-time purchase** that unlocks unlimited projects and tasks, task sharing, and comment writing; and **NearbiGantt Pro Monthly**, an **auto-renewing monthly subscription** that adds chat message writing, task descriptions and parent issues, photo and file attachments, encrypted backup & restore, and data export. The app is free to use with a basic tier.
- All purchase and renewal transactions are processed entirely by **Apple's App Store / StoreKit**. We do **not** collect or store any payment information; we receive only anonymized transaction identifiers needed to verify your entitlement on your device.

## Information We Do NOT Collect

- We do **not** display advertisements and do **not** include any advertising SDKs, the Apple Advertising Identifier (IDFA), or App Tracking Transparency tracking.
- We do **not** use any first-party analytics or crash-reporting SDKs.
- We do **not** operate any servers that receive your personal data.
- We do **not** access your location.
- We do **not** sell or rent your information to anyone.

## Legal Basis for Processing

Under the EU General Data Protection Regulation (GDPR) and the Korean Personal Information Protection Act (PIPA), we rely on the following legal bases for any limited processing that occurs:

- **Consent** — Calendar access, Local Network access, and push notifications. You may withdraw consent at any time through device settings.
- **Performance of contract** — Processing necessary to deliver the app and the features you purchased (e.g., subscription verification via Apple StoreKit, and syncing the content you choose to share with teammates).
- **Legitimate interests** — Ensuring the security and integrity of the app (e.g., de-duplicating entries across a user's own devices).

## Data Retention

- **Projects, tasks, profile, chats, settings, and preferences** are retained on your device (and, if you opt in, your personal iCloud container) until you delete them. We have no ability to delete or access this data on our end.
- The app provides a **"Reset to First Launch"** option that erases every entity and app preference on the device; these deletions also propagate to your iCloud container so your own devices converge.
- **Calendar events** you create through the app remain in your Apple Calendar until you remove them there.

## Data Storage and Security

- All content, settings, and preferences are stored locally on your device or in your personal iCloud container.
- No data is stored on our servers.
- **iCloud** data is encrypted in transit and at rest by Apple. See [Apple's iCloud security overview](https://support.apple.com/en-us/HT202303).
- **Local network** sharing happens directly between devices on the same network and is not sent to any external server.

## Third-Party Services (Subprocessors)

Because NearbiGantt does not operate its own servers, network activity flows directly from your device to Apple's services — with one exception: a third-party public API used to display regional public holidays (see below). The following services may receive data from your device when you use the corresponding feature:

| Service | Provider | Purpose | Data Transferred | When |
|---|---|---|---|---|
| Apple iCloud (CloudKit) | Apple Inc. (USA) | Sync and sharing of your projects, tasks, profile, and chats | The content you create / choose to share | Only if you enable iCloud sync or share content |
| Apple Push Notification service | Apple Inc. (USA) | Delivery of notifications | Notification payloads for shared items, comments, messages | When notifications are enabled |
| Apple App Store / StoreKit | Apple Inc. (USA) | In-app purchase and subscription processing | Anonymized transaction identifiers | When you buy or restore a NearbiGantt purchase |
| Apple Calendar (EventKit) | Apple Inc. (USA) | Show/create events in your timeline | Calendar events on your device | Only when Calendar access is granted |
| Nager.Date (`date.nager.at`) | Nager.Date (third-party public API) | Public holiday dates for a region | A country/region code and a year — **no** personal data, identifiers, or content | When holiday display is on for a region your device's system calendar does not already cover |

Apple's handling of this data is governed by the [Apple Privacy Policy](https://www.apple.com/privacy/).

## International Data Transfers

NearbiGantt is distributed worldwide. When you use iCloud, push notifications, or in-app purchases, data may be processed by Apple in the United States and other jurisdictions where Apple operates its infrastructure. Other than Apple's services described above, the only external request is to the public holiday API (Nager.Date), which receives a country/region code and a year — never your personal data or content.

## Your Rights

Depending on your jurisdiction (EU/UK under GDPR, California under CCPA/CPRA, Korea under PIPA), you may have the following rights regarding your personal information:

- **Access** — Because we store nothing on our servers, you can review all of your information directly in the app on your device.
- **Rectification** — You can edit your profile and all in-app data directly. ("Reset Profile" clears your name, email, and photo.)
- **Erasure** — Use **"Reset to First Launch"** in the app to delete your data (it also propagates the deletion to your iCloud), or uninstall the app to remove all local data.
- **Withdraw consent** — Revoke permissions (Calendar, Local Network, Notifications) in your device settings at any time.
- **Object / restrict processing** — Contact us at [cs@i-nx.com](mailto:cs@i-nx.com).
- **Lodge a complaint** — You may contact your local data protection authority. In Korea, that is the Personal Information Protection Commission ([pipc.go.kr](https://www.pipc.go.kr)).

Because NearbiGantt operates without developer-side accounts or servers, most rights are exercised directly on your device.

## Privacy Manifest and App Store Privacy Details

NearbiGantt includes an Apple Privacy Manifest (`PrivacyInfo.xcprivacy`). The app does **not** track you across other companies' apps or websites, and declares no advertising or tracking data.

Additional manifest details:
- **Tracking**: None. No advertising identifiers, no tracking domains.
- **Accessed APIs**: UserDefaults — used solely for normal app operation (storing your preferences and the widget's shared snapshot within the app's App Group).

Any contact, identifier, or user-content data the app handles (e.g., your profile or tasks) stays in your own iCloud account and is not collected by us.

## Children's Privacy

NearbiGantt does not knowingly collect any personal information from children under the age of 14 (Korean standard), 13 (US COPPA standard), or 16 (EU GDPR standard, depending on member state). If you believe a child has provided information through our app, please contact us and we will assist where possible.

## Changes to This Policy

We may update this Privacy Policy from time to time. Material changes will be reflected by updating the "Last Updated" date and the "Version" field above, and will be described in the Revision History section below.

## Contact Us

If you have questions about this Privacy Policy, or wish to exercise any of your rights:

- **Email**: [cs@i-nx.com](mailto:cs@i-nx.com)
- **Developer**: INX Company Limited

## Revision History

| Version | Date | Changes |
|---|---|---|
| 1.2 | 2026-07-24 | Renamed the one-time in-app purchase from "NearbiGantt Unlimited" to "NearbiGantt Package" (display name only; the product itself and its App Store identifier are unchanged). |
| 1.1 | 2026-07-23 | Clarified that chat message text is stored unencrypted (no additional end-to-end layer) and that a delivered copy persists on the recipient's device and iCloud beyond the sender's deletion. |
| 1.0 | 2026-07-21 | Initial Privacy Policy for NearbiGantt. |
