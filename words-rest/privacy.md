# Privacy Policy

**Last Updated: September 16, 2026**
**Version: 1.1**

INX Company Limited ("we", "our", "us") operates the Words-Rest application (Korean title: 문장의 숲). This Privacy Policy explains how we collect, use, and protect your information when you use our app.

Words-Rest is a **local-first** app for photographing a sentence you met in a book, a film, or on the street and keeping just that sentence as a paper clipping. Text recognition runs **on your device** using Apple's Vision framework. We do **not** operate any servers that receive your personal information, we do **not** display advertisements, and we do **not** run any analytics or crash-reporting SDKs. Your photos and sentences live on your own device and — only if you turn the option on — in **your personal iCloud account** managed by Apple. The app has no user accounts.

This policy covers the iOS app. (An Android version is planned; it will carry its own notices when released.)

## Information We Collect

### Photos and Sentences You Capture

- When you photograph a page or pick a photo from your library, the app finds the sentences in it on your device, and stores the **original photo**, the **clipped image** of each sentence you keep, the **recognized text**, where you place each clipping, and any short **notes** you write.
- All of this is stored in the app's own storage on your device. If you turn on **Keep in iCloud** (Settings › Storage, off by default), it moves to your personal iCloud Drive container instead — see "iCloud Data" below.
- Recognized text and photos are **never sent to us** or to any third party. Text recognition does not leave the device.

### Location Data

- With your permission ("While Using the App"), the app reads your **coarse location (about 100 m accuracy)** for two purposes only:
  - **Weather decoration.** Your coordinates are sent to **Apple Weather (WeatherKit)** so the rain, snow, sun, and clouds on the home and capture screens match the real weather. The result is held in memory for at most 30 minutes while the app runs and is never stored. Weather data is provided by Apple Weather — see [Apple Weather attribution](https://weatherkit.apple.com/legal-attribution.html).
  - **Capture place.** When you photograph a sentence **with the camera**, the app sends the coordinates to **Apple Maps (MapKit reverse geocoding)** to obtain a readable place name, and stores the coordinates **rounded to about 100 m** together with that name alongside the photo's text record on your device. Photos chosen from your library never trigger a location request.
- If you choose a fixed weather preview in Settings (Sun, Rain, Snow, Clouds, Night), the app requests **no location and no weather** at all.
- Location is handled by Apple under [Apple's Privacy Policy](https://www.apple.com/privacy/). We do **not** receive, store, or forward your location. You can deny location access at any time in your device settings; the app works fully without it.

### iCloud Data

- **Keep in iCloud** is **off by default**. When you turn it on, your photos, clippings, text, placements, and notes are moved into your personal iCloud Drive container (`iCloud.com.mimiru.agoodline`), so other devices signed in to the same Apple Account open the same collection. Turning it off moves everything back to the device.
- The app uses **only the private part** of that container. There is no public database, no sharing between different users, and no coordination records of any kind.
- This data is managed entirely by Apple's iCloud service, is encrypted in transit and at rest by Apple, and counts against your own iCloud storage. We do **not** have access to it.

### Camera and Photo Library

- **Camera** is used only when you choose to photograph a sentence.
- To pick an existing photo, the app uses Apple's system photo picker. Only the specific image you select is imported — the app does **not** read your photo library otherwise.
- When you save a photo back to your library from a clipping's detail screen, the app requests **add-only** access; it never requests read access to your library.

### Motion

- With your permission, the app reads device motion so clippings sway and tumble when you shake or tilt the phone. Motion data is used on the device in the moment and is never stored or transmitted. The app works without it.

### Apple Weather Attribution Image

- The Settings screen shows Apple's official " Weather" mark, fetched from Apple's servers in the language you chose. No user information is sent with that request.

## Information We Do NOT Collect

- We do **not** collect your name, email address, phone number, or any account information — the app has no accounts or login.
- We do **not** display advertisements and do **not** include any advertising SDKs, the Apple Advertising Identifier (IDFA), or App Tracking Transparency tracking.
- We do **not** use any analytics or crash-reporting SDKs.
- We do **not** operate any servers that receive your data.
- We do **not** sell or rent your information to anyone.

## Legal Basis for Processing

Under the EU General Data Protection Regulation (GDPR) and the Korean Personal Information Protection Act (PIPA), we rely on the following legal bases for the limited processing that occurs on your device and through Apple's services:

- **Consent** — Camera, photo-library add access, location (weather and capture place), motion, and the optional iCloud storage switch. You may withdraw consent at any time through device settings or by turning the option off in the app.
- **Performance of contract** — Processing necessary to deliver the app's features on your device (recognizing text in the photo you chose, storing your clippings).
- **Legitimate interests** — Ensuring the integrity of your saved data (for example, recovering a backup copy of the library file after an interrupted save).

## Data Retention

- **Photos, clippings, text, placements, notes, and settings** are retained on your device until you delete them in the app or uninstall the app. Uninstalling removes all local data.
- If **Keep in iCloud** is on, the same data is retained in your personal iCloud container until you delete it in the app, turn the option off (which moves it back to the device), or remove the app's data in iOS Settings › Apple Account › iCloud. We have no ability to delete or access data in your iCloud container.
- **Capture place** (rounded coordinates and place name) is stored with the photo's text record and removed when the last clipping from that photo is deleted.
- **Weather data** is held in memory for at most 30 minutes and never written to storage.
- **Location** used for weather is processed in memory for the request and is not persisted by the app.

## Data Storage and Security

- All content, settings, and preferences are stored locally in the app's own storage on your device or, if you enable it, in your personal iCloud container. No data is stored on our servers.
- Data on your device is protected by iOS device encryption. **iCloud** data is encrypted in transit and at rest by Apple — see [Apple's iCloud security overview](https://support.apple.com/en-us/HT202303).
- The only network connections the app makes are to Apple services (WeatherKit, MapKit, iCloud, and the Apple Weather attribution image), all over HTTPS.

## Third-Party Services (Subprocessors)

Because Words-Rest does not operate its own servers, all network activity flows directly from your device to Apple's services. The following services may receive data from your device when you use the corresponding feature:

| Service | Provider | Purpose | Data Transferred | When |
|---|---|---|---|---|
| Apple WeatherKit | Apple Inc. (USA) | Weather decoration on the home and capture screens | Coarse location (about 100 m) | Only when location permission is granted and weather is set to Automatic |
| Apple Maps (MapKit reverse geocoding) | Apple Inc. (USA) | Readable place name for a camera photo | Coordinates of the capture | Only for camera photos, when location permission is granted |
| Apple iCloud (iCloud Drive) | Apple Inc. (USA) | Optional storage of your collection in your own iCloud | Your photos, clippings, text, placements, and notes | Only if you turn on Keep in iCloud |
| Apple Photos | Apple Inc. (USA) | Saving a photo back to your library | The photo you chose to save (stays on your device) | Only when you tap Save to Photos |
| Apple Weather attribution image | Apple Inc. (USA) | Display of the official Apple Weather mark in Settings | None (a static image download) | When the Settings screen is shown |

Apple's handling of this data is governed by the [Apple Privacy Policy](https://www.apple.com/privacy/).

## International Data Transfers

Words-Rest is distributed worldwide. When you use weather, capture place, or iCloud, data may be processed by Apple in the United States and other jurisdictions where Apple operates its infrastructure. We do not transfer your data to any party other than Apple's services described above.

## Your Rights

Depending on your jurisdiction (EU/UK under GDPR, California under CCPA/CPRA, Korea under PIPA), you may have the following rights regarding your personal information:

- **Access** — Because we store nothing on our servers, you can review all of your information directly in the app on your device.
- **Rectification** — You can edit a clipping's text and notes, and move or delete clippings, directly in the app.
- **Erasure** — Delete individual clippings and notes in the app, or uninstall the app to remove all local data. If Keep in iCloud is on, turn it off (the data moves back to the device) or delete the app's data in iOS Settings › Apple Account › iCloud.
- **Portability** — You can save any photo back to your photo library from its detail screen, and your sentences are readable in the app. A full export of your collection is not yet available; if you need a copy of your data, contact us at [cs@i-nx.com](mailto:cs@i-nx.com) and we will help you find a way to exercise this right.
- **Withdraw consent** — Revoke permissions (Camera, Photos, Location, Motion) in your device settings at any time, or turn Keep in iCloud off in the app.
- **Object / restrict processing** — Contact us at [cs@i-nx.com](mailto:cs@i-nx.com).
- **Lodge a complaint** — You may contact your local data protection authority. In Korea, that is the Personal Information Protection Commission ([pipc.go.kr](https://www.pipc.go.kr)).

Because Words-Rest operates without user accounts or servers, most rights are exercised directly on your device.

## Automated Decision-Making

Words-Rest does not engage in automated decision-making, profiling, or any processing that produces legal or similarly significant effects on users. On-device text recognition only proposes sentences found in the photo you chose; it makes no decisions about you.

## Privacy Manifest and App Store Privacy Details

Words-Rest includes an Apple Privacy Manifest (`PrivacyInfo.xcprivacy`). Its App Store "App Privacy" label is **Data Not Collected**.

Why: Apple defines "collection" as data transmitted off the device that the developer or its third parties can access beyond the time needed to serve the request in real time. We operate no servers and include no third-party SDKs, so there is nothing we or a third party can access. Your approximate location is sent to Apple's WeatherKit and MapKit only so that those iOS system services can answer a real-time request (current weather, place name); we receive only the answer. Apple's own processing is governed by Apple's privacy policy. Your photos, text, notes and places stay on your device and, if you enable it, in your own iCloud account, which we cannot read.

Additional manifest details:
- **Tracking**: None. No advertising identifiers, no tracking domains.
- **Accessed APIs**: UserDefaults (storing your preferences) and file timestamps within the app's own storage (checking saved image files) — used solely for normal app operation.

Your photos, recognized text, notes, and placements stay on your device and, if you choose, in your own iCloud account; none of it is collected onto servers we operate.

## Children's Privacy

Words-Rest does not knowingly collect any personal information from children under the age of 14 (Korean standard), 13 (US COPPA standard), or 16 (EU GDPR standard, depending on member state). If you believe a child has provided information through our app, please contact us and we will assist where possible.

## Open Source Attribution

The iOS version of Words-Rest is built only on Apple's system frameworks and contains no third-party code.

## Changes to This Policy

We may update this Privacy Policy from time to time. Material changes will be reflected by updating the "Last Updated" date and the "Version" field above, and will be described in the Revision History section below.

## Contact Us

If you have questions about this Privacy Policy, or wish to exercise any of your rights:

- **Email**: [cs@i-nx.com](mailto:cs@i-nx.com)
- **Developer**: INX Company Limited

## Revision History

| Version | Date | Changes |
|---|---|---|
| 1.0 | 2026-09-16 | Initial Privacy Policy for Words-Rest (문장의 숲). |
| 1.1 | 2026-09-16 | App Store privacy label stated as "Data Not Collected"; the Privacy Manifest declares no collected data types (location is processed by Apple system services in real time only). Data flows unchanged. |
