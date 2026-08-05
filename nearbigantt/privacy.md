# Privacy Policy

**Last Updated: August 5, 2026**
**Version: 1.3**

INX Company Limited ("we", "our", "us") operates the NearbiGantt application. This Privacy Policy explains how we collect, use, and protect your information when you use our app.

NearbiGantt is a **local-first** team task management app with a Gantt timeline, designed for local networks. We do **not** operate any servers that receive your personal information, we do **not** display advertisements, and we do **not** run first-party analytics or crash-reporting SDKs. Your data lives on your own device and, while your device is signed in to iCloud, in **your personal iCloud account** managed by Apple — with one narrow exception: a small set of coordination records (profile cards, share invitations, notification triggers) is written to the **public database** of the app's CloudKit container, described under "iCloud Data (CloudKit)" below.

## Information We Collect

### Profile Information

- When you set up the app, you provide a **display name** and may optionally add an **email address** and a **profile photo**.
- This profile information identifies you to teammates with whom you share projects, tasks, or chats.
- It is stored on your device and, while your device is signed in to iCloud, in your personal iCloud container (`iCloud.com.inx.nearbigantt`). When you share a task with a nearby teammate — or accept one — your display name, your app-specific identifiers, and, **if you entered one, your email address** are sent to that teammate's device along with the shared item, together with your tag list and plan badges, and are stored in their contact entry for you.
- **Profile card (public database).** So that teammates can see your current name, photo, and plan badge even before a share is fully established, the app also publishes a single profile record — your display name, profile photo, your app-specific iCloud record identifier, and two on/off purchase-tier flags — to the **public database** of the app's CloudKit container whenever your iCloud transport is on. This record can be read by other NearbiGantt users who hold your record identifier (in practice: people you share or chat with, including invited-but-not-yet-accepted members); the app itself offers no directory or name search and only ever reads the record of an identifier it already holds. Turning iCloud transport off in Settings stops the app from publishing or refreshing this record; the app re-publishes it whenever it launches or your profile changes while iCloud transport is on. The record itself remains in the public database until we remove it — you can request its removal at [cs@i-nx.com](mailto:cs@i-nx.com) (turn iCloud transport off first so it is not re-published).
- We do **not** receive or store your profile on any server we operate.

### Content You Create

- Projects, tasks, to-dos, comments/memos, group-chat messages, and any photos or files you attach are stored on your device and, while signed in to iCloud, in your personal iCloud container.
- When you choose to share a project, task, or chat with a teammate, the relevant content is synced through Apple's CloudKit sharing or sent directly to nearby devices (see "Local Network Sharing" below). It is never routed through a server we control. The **invitation records** that establish an iCloud share travel through the app's public CloudKit database and include the shared task's **title** (and, in the acceptance response, the recipient's chosen **project name**) alongside both parties' identifiers; invitations addressed to you are accepted automatically without a prompt, and an acceptance response carrying your identifier and display name is posted automatically.
- Chat message text is stored **unencrypted** by NearbiGantt (it relies on Apple's iCloud encryption in transit and at rest, not an additional end-to-end layer). Once a message or shared item is delivered, a copy exists in your teammate's device and iCloud — so, as with email or any messaging app, deleting your own copy or resetting your device does not remove the copy already delivered to them. For shared tasks, your teammate can delete their own copy if you ask. **Individual chat messages, however, cannot be deleted by either side** — you can clear or leave a conversation, which hides it on your own devices but does not delete the underlying messages.
- Attachments are sent as you selected them: images at or below the compression threshold, any image sent with "Send original" enabled, and **document files (always sent as the original)** keep their **embedded metadata** (such as capture time, capture location, or document author) when delivered to teammates. The same applies to profile photos below the avatar size cap, which pass through unmodified into your profile card. Remove metadata before attaching if you do not want to share it.

### iCloud Data (CloudKit)

- While your device is signed in to iCloud, your projects, tasks, profile, and chats are stored in your personal iCloud container and kept in step across your own devices signed in to the same Apple ID. This mirroring runs whenever the device is signed in to iCloud — the in-app transport picker governs the sharing channels described below, not this personal mirror. To stop it, turn iCloud off for NearbiGantt in your device's iCloud settings, or sign the device out of iCloud. This data is managed entirely by Apple's iCloud service and is encrypted in transit and at rest by Apple. We do **not** have access to the data in your personal iCloud container.
- **Public database.** The same CloudKit container (`iCloud.com.inx.nearbigantt`, owned by us and hosted by Apple) also has a **public database** that the app uses as a coordination channel between different users' accounts. Records written there: your **profile card** (see "Profile Information"), **share and chat invitations and responses** (both parties' identifiers, sender display name, shared task title, chosen project name, share links, and — for a chat-room invitation — the identifier **and display name of every member of that chat room**), and **notification trigger records** (see "Push Notifications"). Public-database records can be read by other NearbiGantt users; we administer this database and can technically access it — we access these records only to operate and troubleshoot the coordination channel, to respond to an abuse report, or where the law requires. Apart from the profile photo in your profile card, no task bodies, to-dos, comments, chat message text, or file attachments are ever written to the public database.
- **Retention of public-database records.** Notification trigger records are pruned by the sending device, and share-response records by the responding device, once they are more than about 24 hours old — this clean-up is best-effort and runs only while that device has the app open with iCloud transport on, so records can persist longer if the device is not used again. Share and chat invitation records are deleted when the recipient's app consumes them (or by a "Reset to First Launch" on the device that created them); an invitation that is never accepted may remain in the public database indefinitely. The profile card persists until removed on request.

### Calendar Access

- With your permission, NearbiGantt reads and creates events in your **Apple Calendar** so they appear alongside your tasks in the timeline.
- Calendar data is handled by Apple's EventKit on your device. It is **not** transmitted to us or to any third party.
- You can grant or revoke Calendar access at any time in your device settings. The app works without it.

### Public Holidays

- To show public holidays on your timeline, NearbiGantt uses your device's own system holiday calendar where available. Whenever the system calendar returns nothing for the selected region — because the region is not covered, because you turned "System Holidays" off in Settings, or because Calendar access is denied — the app fetches holiday dates from a third-party public API (Nager.Date, `date.nager.at`). Only a **country/region code and a year** are sent in the request itself — no profile data, app identifiers, or content you created; as with any direct connection to a third-party service, Nager.Date technically receives your device's IP address. In Settings you can choose which region's holidays are shown.

### Photos

- When you choose a profile photo or attach an image, the app uses Apple's system photo picker. Only the specific image you select is imported into the app — we do **not** access your photo library otherwise, and the app does **not** request full photo-library permission.

### Local Network Sharing

- NearbiGantt can discover nearby teammates and share content with them over the local network using Apple's **MultipeerConnectivity** framework (Bonjour service `_nearbigantt-sh`).
- The app requests **Local Network** permission to discover and connect with nearby devices.
- While Nearby transport is on, the app **advertises your presence** on the local network: the advertisement includes your **display name** (also embedded in the network service name, alongside a short device-identifier fragment), your app-specific iCloud record identifier, and a SHA-256 hash of that identifier (used for de-duplicating the same person's multiple devices). Any device on the same network running standard network-discovery software can observe this advertisement. Turning Nearby transport off in Settings stops it.
- Connections between nearby NearbiGantt devices are established **automatically**, without a prompt. Receiving a shared task still requires your explicit in-app Accept; a **chat-conversation invitation** from a nearby teammate, however, is joined automatically. **Comment updates (including the comment text and any attached photo or file), project updates, task deletions (which carry the task title), and share-revoke/reinstate signals are broadcast to all currently connected nearby devices** — devices that do not already hold the related item discard them on arrival.
- All communication on this path happens **directly between nearby devices** and is **not routed through any external server**. If a direct connection cannot be established, the app delivers the share through Apple's CloudKit instead (see "iCloud Data").

### Push Notifications

- With your permission, the app shows notifications about shared items, comments, and messages, delivered through Apple's Push Notification service (via CloudKit subscriptions).
- To make a notification reach you while your app is closed, the **sender's** device writes a short-lived **notification trigger record** to the app's public CloudKit database. It contains the sender's display name, both users' app-specific iCloud identifiers, the event kind, and the item identifier — **never** the message or comment text. See "Retention of public-database records" above for how long these persist.
- The app registers with Apple's push service at launch, independently of the notification permission — this is what allows silent CloudKit pushes to drive background sync. Disabling notifications in your device settings stops visible alerts, but background sync continues while the device is signed in to iCloud. Turning iCloud transport off in Settings stops the app's public-database coordination records and new push-subscription registration; it does **not** stop the personal iCloud mirror or subscriptions registered earlier. To stop iCloud processing entirely, turn iCloud off for NearbiGantt in your device's iCloud settings or sign out of iCloud.

### In-App Purchases

- NearbiGantt offers two optional in-app purchases: **NearbiGantt Starter Pack**, a **one-time purchase** that unlocks unlimited projects and tasks, task sharing, and comment writing; and **NearbiGantt Pro Monthly**, an **auto-renewing monthly subscription** that adds chat message writing, task descriptions and parent issues, photo and file attachments, encrypted backup & restore, and data export. The app is free to use with a basic tier.
- All purchase and renewal transactions are processed entirely by **Apple's App Store / StoreKit**. We do **not** collect or store any payment information; the app reads only the entitlement state needed to unlock features on your device.
- So that teammates' apps can render your plan badge and show or hide plan-dependent fields, the app shares **two on/off entitlement flags** (whether you hold the monthly plan, and whether you hold the one-time purchase) with the people you share or chat with — over the local network, in the public-database profile card described above, and as a visibility flag stamped on each shared task record itself. Transaction identifiers, amounts, and payment details are never shared with anyone.

## Information We Do NOT Collect

- We do **not** display advertisements and do **not** include any advertising SDKs, the Apple Advertising Identifier (IDFA), or App Tracking Transparency tracking.
- We do **not** use any first-party analytics or crash-reporting SDKs.
- We do **not** operate any servers that receive your personal data. (The coordination records described under "iCloud Data" live in Apple-hosted CloudKit, not on a server of ours.)
- We do **not** access your location.
- We do **not** sell or rent your information to anyone.

## Legal Basis for Processing

Under the EU General Data Protection Regulation (GDPR) and the Korean Personal Information Protection Act (PIPA), we rely on the following legal bases for any limited processing that occurs:

- **Consent** — Calendar access, Local Network access, and visible push-notification alerts. You may withdraw consent at any time through device settings.
- **Performance of contract** — Processing necessary to deliver the app and the features you purchased (e.g., subscription verification via Apple StoreKit; syncing the content you choose to share with teammates; the coordination records that make sharing and notifications work while iCloud transport is on; and the background sync channel that keeps your own devices in step while the device is signed in to iCloud).
- **Legitimate interests** — Ensuring the security and integrity of the app (e.g., de-duplicating entries across a user's own devices).

## Data Retention

- **Projects, tasks, profile, chats, settings, and preferences** are retained on your device (and, while signed in to iCloud, your personal iCloud container) until you delete them — noting that individual chat messages cannot be deleted singly (see "Content You Create"). We have no ability to delete or access the data in your personal iCloud container.
- **Public-database records** are retained as described under "iCloud Data (CloudKit) → Retention".
- The app provides a **"Reset to First Launch"** option that erases your projects, tasks, comments, chats, and contacts on the device and propagates those deletions to your iCloud container so your own devices converge. Your **profile (display name, email, and photo) and display settings are kept** — the in-app confirmation says so before you reset, and display settings may be restored from iCloud afterwards; use "Reset Profile" to clear the profile fields. The reset does **not** remove the public-database profile card, and does not delete backup files you have created (see "Data Storage and Security").
- **Calendar events** you create through the app remain in your Apple Calendar until you remove them there.

## Data Storage and Security

- All content, settings, and preferences are stored locally on your device or in your personal iCloud container — except the coordination records described under "iCloud Data (CloudKit)", which live in the app's public CloudKit database.
- No data is stored on our servers.
- **iCloud** data is encrypted in transit and at rest by Apple. See [Apple's iCloud security overview](https://support.apple.com/en-us/HT202303).
- **Local network** sharing happens directly between devices on the same network and is not sent to any external server.
- **Backups** you create are written to the app's Documents/Backups folder on your device and remain there (surviving "Reset to First Launch") until you delete them. Backup files are encrypted against casual reading; treat the file itself as sensitive when you move or share it.

## Third-Party Services (Subprocessors)

Because NearbiGantt does not operate its own servers, network activity flows directly from your device to Apple's services — with one exception: a third-party public API used to display regional public holidays (see below). The following services may receive data from your device when you use the corresponding feature:

| Service | Provider | Purpose | Data Transferred | When |
|---|---|---|---|---|
| Apple iCloud (CloudKit) | Apple Inc. (USA) | Sync and sharing of your projects, tasks, profile, and chats; public-database coordination records (profile card, invitations, notification triggers) | The content you create / choose to share; for the public database: display name, profile photo, app-specific iCloud identifiers, purchase-tier flags, shared task titles, chosen project names, chat-room member names | While the device is signed in to iCloud; new public-database records are written only while iCloud transport is on (clean-up deletions of your own existing records can run in any mode) |
| Apple Push Notification service | Apple Inc. (USA) | Delivery of notifications and silent sync pushes | Notification trigger metadata: sender display name, both users' app-specific iCloud identifiers, event kind, item identifier — no message content | While the device is signed in to iCloud (independent of the notification permission) |
| Apple App Store / StoreKit | Apple Inc. (USA) | In-app purchase and subscription processing | Purchase transactions (processed by Apple; the app reads entitlement state) | When you buy or restore a NearbiGantt purchase |
| Apple Calendar (EventKit) | Apple Inc. (USA) | Show/create events in your timeline | Calendar events on your device | Only when Calendar access is granted |
| Nager.Date (`date.nager.at`) | Nager.Date (third-party public API) | Public holiday dates for a region | A country/region code and a year (plus, inherently, your device's IP address) — no profile data, app identifiers, or content | Whenever the device's system holiday calendar returns nothing for the selected region (not covered, System Holidays off, or Calendar access denied) |

Apple's handling of this data is governed by the [Apple Privacy Policy](https://www.apple.com/privacy/).

## International Data Transfers

NearbiGantt is distributed worldwide. When you use iCloud, push notifications, or in-app purchases, data may be processed by Apple in the United States and other jurisdictions where Apple operates its infrastructure. Other than Apple's services described above, the only external request is to the public holiday API (Nager.Date), which receives a country/region code, a year, and — inherently — your device's IP address, but never your profile data or content.

## Your Rights

Depending on your jurisdiction (EU/UK under GDPR, California under CCPA/CPRA, Korea under PIPA), you may have the following rights regarding your personal information:

- **Access** — Because we store nothing on our servers, you can review all of your information directly in the app on your device.
- **Rectification** — You can edit your profile and all in-app data directly. ("Reset Profile" clears your name, email, and photo.)
- **Erasure** — Use **"Reset to First Launch"** in the app to delete your content (it also propagates the deletion to your iCloud; your profile and display settings are kept — use "Reset Profile" to clear the profile), or uninstall the app to remove all local data. To have your public-database profile card removed, contact us at [cs@i-nx.com](mailto:cs@i-nx.com).
- **Portability** — The app can export your tasks, comments, and conversations as CSV archives and create full backup files you can keep or move. These export and backup features are part of the Pro Monthly subscription; if you need a copy of your data and do not hold the subscription, contact us at [cs@i-nx.com](mailto:cs@i-nx.com) and we will help you find a way to exercise this right.
- **Withdraw consent** — Revoke permissions (Calendar, Local Network, Notifications) in your device settings at any time. Revoking the notification permission stops visible alerts only; to stop iCloud processing, turn iCloud off for NearbiGantt in your device's iCloud settings or sign out of iCloud (the in-app transport picker governs sharing channels, not the personal iCloud mirror).
- **Object / restrict processing** — Contact us at [cs@i-nx.com](mailto:cs@i-nx.com).
- **Lodge a complaint** — You may contact your local data protection authority. In Korea, that is the Personal Information Protection Commission ([pipc.go.kr](https://www.pipc.go.kr)).

Because NearbiGantt operates without developer-side accounts or servers, most rights are exercised directly on your device.

## Privacy Manifest and App Store Privacy Details

NearbiGantt includes an Apple Privacy Manifest (`PrivacyInfo.xcprivacy`). The app does **not** track you across other companies' apps or websites, and declares no advertising or tracking data.

Additional manifest details:
- **Tracking**: None. No advertising identifiers, no tracking domains.
- **Accessed APIs**: UserDefaults — used solely for normal app operation (storing your preferences and the widget's shared snapshot within the app's App Group).

Most contact, identifier, and user-content data the app handles stays on your devices and in your own iCloud account. The exceptions are set out above: copies of content you share are delivered to your teammates' devices and iCloud, and the narrow coordination records described under "iCloud Data (CloudKit)" live in the app's public CloudKit database. None of it is collected onto servers we operate.

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
| 1.3 | 2026-08-05 | Source-audit alignment: disclosed the public CloudKit database (profile card with name/photo/plan flags, share & chat invitation records including chat-room member names, notification trigger records) with an honest retention section, and scoped the "we cannot access" statement to the personal container; clarified that the personal iCloud mirror runs whenever the device is signed in to iCloud (the in-app transport picker governs sharing channels) and how to stop it; corrected the "Reset to First Launch" scope (profile including email, and display settings, are kept); clarified that individual chat messages cannot be deleted; described the local-network advertisement contents, automatic connections, broadcast scope (including comment text/attachments and task-deletion titles), and that a shared task carries the sender's email and plan flags; explained that push registration is independent of the notification permission; added attachment/profile-photo metadata pass-through, backup retention, Nager.Date IP disclosure, holiday-fallback conditions, and a Portability entry. |
| 1.2 | 2026-07-24 | Renamed the one-time in-app purchase from "NearbiGantt Unlimited" to "NearbiGantt Starter Pack" (display name only; the product itself and its App Store identifier are unchanged). |
| 1.1 | 2026-07-23 | Clarified that chat message text is stored unencrypted (no additional end-to-end layer) and that a delivered copy persists on the recipient's device and iCloud beyond the sender's deletion. |
| 1.0 | 2026-07-21 | Initial Privacy Policy for NearbiGantt. |
