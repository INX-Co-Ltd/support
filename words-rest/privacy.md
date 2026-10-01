# Privacy Policy

**Last Updated: October 1, 2026**
**Version: 1.2**

INX Company Limited ("we", "our", "us") operates the Words-Rest application (Korean title: 문장의 숲). This Privacy Policy explains how we collect, use, and protect your information when you use our app.

Words-Rest is a **local-first** app for photographing a sentence you met in a book, a film, or on the street and keeping just that sentence as a paper clipping. Text recognition runs **on your device** (Apple's Vision framework on iPhone, Google ML Kit on Android). We do **not** operate servers that receive your photos, sentences, notes, or location, and we do **not** display advertisements. Your photos and sentences live on your own device and — only if you turn the option on — in **your personal iCloud account** (iPhone) or **your personal Google Drive** (Android). The app has no user accounts.

This policy covers both the iOS and the Android app. The sections below describe the iOS app; where the Android app works differently, see **[Android App](#android-app)**. To delete your data on either platform, see **[Deleting Your Data](#deleting-your-data)**.

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

- We do **not** collect your name, email address, phone number, or any account information — the app has no accounts or login. (On Android, Keep in Google Drive asks for permission through your Google account; the app does not receive your name or email address.)
- We do **not** display advertisements and do **not** include any advertising SDKs, the Apple Advertising Identifier (IDFA), or App Tracking Transparency tracking.
- The iOS app does **not** use any analytics or crash-reporting SDKs. (On Android, the text-recognition library Google ML Kit sends diagnostic data to Google — see [Android App](#android-app).)
- We do **not** operate servers that receive or store your photos, sentences, notes, or location.
- We do **not** sell or rent your information to anyone.

## Legal Basis for Processing

Under the EU General Data Protection Regulation (GDPR) and the Korean Personal Information Protection Act (PIPA), we rely on the following legal bases for the limited processing that occurs on your device and through Apple's services:

- **Consent** — Camera, photo-library add access, location (weather and capture place), motion, and the optional iCloud / Google Drive storage switch. You may withdraw consent at any time through device settings or by turning the option off in the app.
- **Performance of contract** — Processing necessary to deliver the app's features on your device (recognizing text in the photo you chose, storing your clippings).
- **Legitimate interests** — Ensuring the integrity of your saved data (for example, recovering a backup copy of the library file after an interrupted save).

## Data Retention

- **Photos, clippings, text, placements, notes, and settings** are retained on your device until you delete them in the app or uninstall the app. Uninstalling removes all local data.
- If **Keep in iCloud** is on, the same data is retained in your personal iCloud container until you delete it in the app, turn the option off (which moves it back to the device), or remove the app's data in iOS Settings › Apple Account › iCloud. We have no ability to delete or access data in your iCloud container.
- On Android, if **Keep in Google Drive** is on, the same data is kept in the private app folder of your Google Drive until you delete it in the app or turn the option off (which deletes the Drive copy). We have no ability to access or delete it.
- **Capture place** (rounded coordinates and place name) is stored with the photo's text record and removed when the last clipping from that photo is deleted.
- **Weather data** is held in memory for at most 30 minutes and never written to storage.
- **Location** used for weather is processed in memory for the request and is not persisted by the app.

## Data Storage and Security

- All content, settings, and preferences are stored locally in the app's own storage on your device or, if you enable it, in your personal iCloud container. No data is stored on our servers.
- Data on your device is protected by iOS device encryption. **iCloud** data is encrypted in transit and at rest by Apple — see [Apple's iCloud security overview](https://support.apple.com/en-us/HT202303).
- The only network connections the iOS app makes are to Apple services (WeatherKit, MapKit, iCloud, and the Apple Weather attribution image), all over HTTPS. The Android app's connections are listed in [Android App](#android-app).

## Third-Party Services (Subprocessors)

On iPhone, all network activity flows directly from your device to Apple's services. The following services may receive data from your device when you use the corresponding feature (for the Android app, see [Android App](#android-app)):

| Service | Provider | Purpose | Data Transferred | When |
|---|---|---|---|---|
| Apple WeatherKit | Apple Inc. (USA) | Weather decoration on the home and capture screens | Coarse location (about 100 m) | Only when location permission is granted and weather is set to Auto |
| Apple Maps (MapKit reverse geocoding) | Apple Inc. (USA) | Readable place name for a camera photo | Coordinates of the capture | Only for camera photos, when location permission is granted |
| Apple iCloud (iCloud Drive) | Apple Inc. (USA) | Optional storage of your collection in your own iCloud | Your photos, clippings, text, placements, and notes | Only if you turn on Keep in iCloud |
| Apple Photos | Apple Inc. (USA) | Saving a photo back to your library | The photo you chose to save (stays on your device) | Only when you tap Save to Photos |
| Apple Weather attribution image | Apple Inc. (USA) | Display of the official Apple Weather mark in Settings | None (a static image download) | When the Settings screen is shown |

Apple's handling of this data is governed by the [Apple Privacy Policy](https://www.apple.com/privacy/).

## International Data Transfers

Words-Rest is distributed worldwide. When you use weather, capture place, or iCloud, data may be processed by Apple in the United States and other jurisdictions where Apple operates its infrastructure. On Android, Google (ML Kit diagnostics, place names, Google Drive) and Cloudflare (weather token delivery) may also process data in the United States and other jurisdictions. We do not transfer your data to any party other than the services described in this policy.

## Your Rights

Depending on your jurisdiction (EU/UK under GDPR, California under CCPA/CPRA, Korea under PIPA), you may have the following rights regarding your personal information:

- **Access** — Because we store nothing on our servers, you can review all of your information directly in the app on your device.
- **Rectification** — You can edit a clipping's text and notes, and move or delete clippings, directly in the app.
- **Erasure** — Delete individual clippings and notes in the app, or uninstall the app to remove all local data. If Keep in iCloud or Keep in Google Drive is on, turn it off. Step-by-step instructions are in [Deleting Your Data](#deleting-your-data).
- **Portability** — You can save any photo back to your photo library from its detail screen, and your sentences are readable in the app. A full export of your collection is not yet available; if you need a copy of your data, contact us at [cs@i-nx.com](mailto:cs@i-nx.com) and we will help you find a way to exercise this right.
- **Withdraw consent** — Revoke permissions (Camera, Photos, Location, Motion) in your device settings at any time, or turn Keep in iCloud / Keep in Google Drive off in the app.
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

## Android App {#android-app}

The Android app has the same features as the iPhone app but handles some of them differently. Collections on iPhone and Android are not connected to each other.

### Text Recognition (Google ML Kit)

- Sentences are recognized **on your device** by Google ML Kit, whose recognition model is bundled inside the app. Your photos and recognized text are **not** sent to Google or to us.
- ML Kit itself sends **diagnostic and usage information** to Google: a device or per-installation identifier, the app's package name and version, performance metrics such as latency, device information (manufacturer, model, OS version), and feature event types and error codes. It is sent over HTTPS and not shared with third parties — see [ML Kit Android data disclosure](https://developers.google.com/ml-kit/android-data-disclosure). We cannot turn this off from the app.

### Weather

- With location permission and weather set to Auto, the app first asks **our weather token server** for a short-lived access token, then sends your coordinates, **rounded to about 100 m**, directly to **Apple WeatherKit** to get the current weather. As on iPhone, the result is held in memory for at most 30 minutes and never stored; a fixed weather preview requests nothing.
- The token server receives **no location, photos, or text**, and its code keeps no record of requests (only an error name if issuing a token fails). It runs on **Cloudflare**, which processes your IP address to deliver the request under the [Cloudflare Privacy Policy](https://www.cloudflare.com/privacypolicy/).
- The Settings screen shows the Apple Weather mark fetched from Apple's servers; no user information is sent with that request.

### Capture Place

- With location permission, when you photograph a sentence **with the camera**, the app sends the coordinates of that moment to your device's built-in address service (**Google Play services Geocoder**) to obtain a readable place name, and stores the coordinates **rounded to about 100 m** together with that name on your device. Photos chosen from your gallery never trigger a location request. Google's processing is governed by the [Google Privacy Policy](https://policies.google.com/privacy).
- When you open the place map in a clipping's detail screen, **Apple MapKit JS** shows a map around the stored coordinates; map requests (such as the map area and your IP address) go to Apple and its map providers under the [Apple Privacy Policy](https://www.apple.com/privacy/). Photos, text, and notes are never sent to the map service.

### Keep in Google Drive

- **Keep in Google Drive** (Settings › Storage) is **off by default**. When you turn it on and allow access with your Google account, your photos, clippings, text, placements, notes, and capture places (rounded coordinates and names) are copied to the **private app folder** of your own Google Drive, so you can carry on after you switch phones. The app asks only for access to that folder (`drive.appdata`); it cannot see your other Drive files, and the folder does not appear in your Drive file list.
- The copy travels directly between your device and Google over HTTPS and counts against your Google storage. **We cannot access it.**
- Turning the option off **deletes the copy in Google Drive** and revokes the app's access; your collection stays on the phone. Google's handling of your account data is governed by the [Google Privacy Policy](https://policies.google.com/privacy).

### Android Permissions

| Permission | Used for | If you deny it |
|---|---|---|
| Location (while using the app; precise or approximate, your choice) | Weather and capture place (coordinates are rounded to about 100 m) | No weather decoration and no capture place; with approximate location only, place names cover a wider area. Everything else works. |
| Internet | Weather, place names, the place map, Google Drive, and ML Kit diagnostics | — (granted at install) |
| Vibration | Feedback when you shake clippings | — (granted at install) |
| Storage (Android 9 only) | Saving a photo to your gallery | Saving to the gallery is unavailable on Android 9 |

The app takes photos through your device's camera app and picks photos with the system photo picker, so it does not request camera or photo permissions. Other entries you may see in the permission list (network state, wake lock, and similar) are declared by the Google Play services and ML Kit libraries the app includes.

### Android Services

| Service | Provider | Purpose | Data Transferred | When |
|---|---|---|---|---|
| Google ML Kit | Google LLC (USA) | Diagnostics of the on-device text-recognition library | Device or installation identifier, app version, performance metrics, device information, error codes | Whenever text recognition runs |
| INX weather token server (on Cloudflare) | INX Company Limited / Cloudflare, Inc. (USA) | Short-lived token for weather requests | No personal content; your IP address is processed by Cloudflare for delivery | When weather is set to Auto |
| Apple WeatherKit | Apple Inc. (USA) | Weather decoration | Coordinates rounded to about 100 m | When location permission is granted and weather is set to Auto |
| Google Play services Geocoder | Google LLC (USA) | Readable place name for a camera photo | Coordinates of the capture | Camera photos, when location permission is granted |
| Apple MapKit JS | Apple Inc. (USA) | Place map in a clipping's detail screen | Map area, IP address | When you open the place map |
| Google Drive | Google LLC (USA) | Optional copy of your collection in your own Drive | Photos, clippings, text, placements, notes, capture places | Only if you turn on Keep in Google Drive |

### Google Play Data Safety

Under Google Play's definition (data sent off the device), the app's Data safety section lists **precise location**, **photos** and **other user-generated content** (when Keep in Google Drive is on), and **diagnostics, other app performance data, and device or other IDs** (ML Kit) as collected. None of it is shared, and all of it is encrypted in transit. This refers to the transfers described above; it does not mean we keep, sell, or give this information to anyone.

## Deleting Your Data {#deleting-your-data}

Words-Rest (by INX Company Limited) has no user accounts, and **we keep none of your data on our servers**, so there is nothing to request from us — you delete your data yourself, on your device or in your own cloud storage:

1. **A clipping or a note** — open it in the app and delete it. Its clipped image is removed, and the original photo and capture place are removed when the last clipping from that photo is deleted.
2. **Everything on the device** — uninstall the app. All local data is removed.
3. **iPhone, Keep in iCloud** — turn the option off in Settings › Storage (the collection moves back to the device and the iCloud copy is removed), or delete the app's data in iOS Settings › Apple Account › iCloud.
4. **Android, Keep in Google Drive** — turn the option off in Settings › Storage. The copy in your Google Drive is deleted and the app's access is revoked. You can also delete it on the web: Google Drive › Settings › Manage apps › Words-Rest › Options › **Delete hidden app data** (and Disconnect from Drive). If you do, the next time the app opens it turns the option off on that phone and says so in Settings; it does not upload again unless you turn the option back on.

Deleted data cannot be restored. Weather results and location used for requests are never stored, and our weather token server keeps no record of requests, so nothing remains after deletion. If you need help, contact us at [cs@i-nx.com](mailto:cs@i-nx.com).

## Children's Privacy

Words-Rest does not knowingly collect any personal information from children under the age of 14 (Korean standard), 13 (US COPPA standard), or 16 (EU GDPR standard, depending on member state). If you believe a child has provided information through our app, please contact us and we will assist where possible.

## Open Source Attribution

The iOS version of Words-Rest is built only on Apple's system frameworks and contains no third-party code. The Android version includes open-source and Google libraries; their notices are in the app under Settings › About.

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
| 1.2 | 2026-10-01 | Added the Android app (Google ML Kit diagnostics, weather token server, place names via Google Play services, Keep in Google Drive, Android permissions, Google Play Data safety) and a Deleting Your Data section for both platforms. iOS data flows unchanged. |
