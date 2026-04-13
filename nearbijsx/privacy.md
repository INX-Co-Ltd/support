# Privacy Policy

**Last Updated: April 10, 2026**
**Version: 1.1**

INX Company Limited ("we", "our", "us") operates the NearbiJSX application. This Privacy Policy explains how we collect, use, and protect your information when you use our app.

NearbiJSX is a **local-first** application for running and managing Claude-generated JSX artifacts. We do not operate any servers that receive your personal information, and we do not run first-party analytics or crash reporting SDKs. On iOS and iPadOS, the free tier of the app displays advertisements through third-party ad networks, as described below.

## Information We Collect

### Advertising Identifiers (Device ID / IDFA)

- On **iOS and iPadOS**, the free tier of our app displays advertisements through **Google AdMob** and **Unity Ads**. The macOS version does **not** include any advertising SDKs.
- These third-party ad networks may collect your device's advertising identifier (IDFA) to serve relevant ads and measure ad performance.
- Before collecting the IDFA, the app will ask for your permission through Apple's App Tracking Transparency (ATT) prompt. You can deny this request at any time.
- If you deny tracking, ads will still be shown but they will not be personalized.
- Ad networks also use **SKAdNetwork** for privacy-preserving ad attribution without identifying you personally.
- **NearbiJSX Pro** (in-app purchase) removes all advertisements.

### Location Data

- We access your approximate location **only** to provide weather-aware greetings on the home screen.
- Your approximate location is sent to **Apple Weather (WeatherKit)** to retrieve current weather conditions. This data is handled by Apple under [Apple's Privacy Policy](https://www.apple.com/privacy/). We do not receive, store, or forward your location data to any other party.
- Weather data is provided by Apple Weather. See [Apple Weather attribution](https://weatherkit.apple.com/legal-attribution.html) for details.
- On iOS/iPadOS, location is requested only while using the app. On macOS, the app may request persistent location access to provide weather greetings.
- You can deny location access at any time in your device settings. The app works fully without it.

### iCloud Data

- JSX files you create are stored in your personal iCloud container (`iCloud.com.nearbijsx`) if you choose iCloud storage.
- This data is managed entirely by Apple's iCloud service. We do not have access to your iCloud data.

### AI API Keys and Prompts

- If you use the AI assistance feature, you provide your own API keys (Claude, OpenAI, Gemini, GitHub Models).
- API keys are stored locally in your device's Keychain. They are **never transmitted to our servers**.
- API requests are sent directly from your device to the respective AI provider.
- **Important**: The content of your prompts (JSX code and instructions you send to the AI) is transmitted to the AI provider you select. Each provider applies its own data handling policy, which may include temporary retention for abuse prevention, safety review, or model improvement. For example, Anthropic may retain prompt data for up to 30 days and, depending on your account settings with Anthropic, may use prompts to improve their models. Review the provider's privacy policy (linked in the "Third-Party Services" section below) before sending sensitive or confidential content through the AI feature.

## Information We Do NOT Collect

- We do **not** collect personal information such as name, email, phone number, or address.
- We do **not** use any first-party analytics or crash reporting SDKs.
- We do **not** have user accounts or login systems.
- We do **not** operate any servers that receive your data.

## Legal Basis for Processing

Under the EU General Data Protection Regulation (GDPR) and the Korean Personal Information Protection Act (PIPA), we rely on the following legal bases for any limited processing that occurs:

- **Consent** — Location access for weather greetings, App Tracking Transparency (IDFA) for personalized advertising, and use of the optional AI assistance feature. You may withdraw consent at any time through device settings or by not using the feature.
- **Performance of contract** — Processing necessary to deliver the app you purchased (e.g., in-app purchase verification via Apple StoreKit).
- **Legitimate interests** — Ensuring the security and integrity of the app (e.g., Keychain storage of sensitive credentials), and serving non-personalized advertising to free users on iOS/iPadOS.

## Data Retention

- **JSX files, settings, and preferences** are retained on your device (and, if you opt-in, your personal iCloud container) until you delete them. We have no ability to delete or access this data on our end.
- **App deletion** preserves the local `Documents/NearbiJSX/` folder until you manually remove it, so your JSX files are not lost if you reinstall the app.
- **Location data** is processed in memory for a single weather request and is not persisted by the app.
- **AI prompts** are transmitted directly to the AI provider you selected and are not logged, stored, or retained by us.
- **Weather data** is cached on-device for up to 30 minutes to reduce redundant API calls.

## Local Network Sharing

- NearbiJSX supports sharing JSX files with nearby devices over the local network using Apple's MultipeerConnectivity framework.
- The app requests **Local Network** permission to discover and connect with nearby devices.
- All communication happens directly between nearby devices. File data shared during this process is **not routed through any external server**.
- Apple's MultipeerConnectivity framework provides TLS-based transport security between peers by default.

## In-App Purchases

- Purchase transactions (NearbiJSX Pro) are processed entirely by Apple's App Store. We do not collect or store any payment information.
- Pro users do not see advertisements.

## File Access

- NearbiJSX enables file sharing with your computer via the Finder (macOS) or the Files app (iOS/iPadOS). Files stored in the app's Documents folder are accessible through these system tools.

## Data Storage and Security

- All JSX files, settings, and preferences are stored locally on your device or in your personal iCloud container.
- No data is stored on our servers.
- **API keys** (Claude, OpenAI, Gemini, GitHub Models) are stored in the Apple **Keychain**, which is protected by device-level encryption.
- **Network transport** to AI providers and ad networks uses HTTPS (TLS 1.2+).
- **iCloud** data is encrypted in transit and at rest by Apple. See [Apple's iCloud security overview](https://support.apple.com/en-us/HT202303).

## Third-Party Services (Subprocessors)

Because NearbiJSX does not operate its own servers, all network activity flows directly from your device to the third-party services you choose to use or that the free tier requires. The following services may receive data from your device when you use the corresponding feature:

| Service | Provider | Purpose | Data Transferred | When |
|---|---|---|---|---|
| Google AdMob | Google LLC (USA) | Advertising (iOS/iPadOS only) | IDFA (if ATT granted), device info, ad interaction | Free-tier users on iOS/iPadOS |
| Unity Ads | Unity Technologies ApS (Denmark / USA) | Advertising (iOS/iPadOS only) | IDFA (if ATT granted), device info, ad interaction | Free-tier users on iOS/iPadOS |
| Apple WeatherKit | Apple Inc. (USA) | Weather greetings | Coarse location (reduced accuracy) | Only when location permission is granted |
| Apple iCloud | Apple Inc. (USA) | Optional JSX file sync | JSX files you create | Only if you enable iCloud storage |
| Apple App Store / StoreKit | Apple Inc. (USA) | In-app purchase processing | Anonymized transaction IDs | When you purchase NearbiJSX Pro |
| Anthropic Claude | Anthropic PBC (USA) | AI assistance | Your prompt text | Only when you invoke the AI feature with a Claude key |
| OpenAI | OpenAI OpCo, LLC (USA) | AI assistance | Your prompt text | Only when you invoke the AI feature with an OpenAI key |
| Google Gemini | Google LLC (USA) | AI assistance | Your prompt text | Only when you invoke the AI feature with a Gemini key |
| GitHub Models | Microsoft Corporation (USA) | AI assistance | Your prompt text | Only when you invoke the AI feature with a GitHub token |

Each provider has its own privacy policy governing how it handles data it receives:
- [Apple Privacy Policy](https://www.apple.com/privacy/)
- [Google AdMob / Google Privacy Policy](https://policies.google.com/privacy)
- [Unity Ads Privacy Policy](https://unity.com/legal/privacy-policy)
- [Anthropic Privacy Policy](https://www.anthropic.com/legal/privacy)
- [OpenAI Privacy Policy](https://openai.com/policies/privacy-policy/)
- [Microsoft Privacy Statement](https://privacy.microsoft.com/en-us/privacystatement)

## International Data Transfers

NearbiJSX is distributed worldwide. When you use the features listed in the Third-Party Services table above, data may be transferred to the United States and other jurisdictions where those providers operate their infrastructure. By enabling the corresponding feature (location, iCloud, AI assistance, personalized ads), you acknowledge that the relevant data is transferred to the selected provider outside your country of residence.

We do not transfer your data to any party other than those third-party services that you have actively chosen to use or that the free tier of the app requires for ad delivery.

## Your Rights

Depending on your jurisdiction (EU/UK under GDPR, California under CCPA/CPRA, Korea under PIPA), you may have the following rights regarding your personal information:

- **Access** — Request a copy of the information we hold about you. (Because we store nothing on our servers, this is effectively achieved by browsing the app's files and settings on your device.)
- **Rectification** — Correct inaccurate information. You can edit all in-app data directly.
- **Erasure** — Delete your information. You can delete files, clear app storage, or uninstall the app to remove all local data.
- **Portability** — Obtain your data in a portable format. The app lets you export JSX files directly.
- **Withdraw consent** — Revoke permissions (location, Local Network, App Tracking) in your device settings at any time.
- **Object / restrict processing** — Contact us at cs@i-nx.com.
- **Lodge a complaint** — You may contact your local data protection authority. In Korea, that is the Personal Information Protection Commission ([pipc.go.kr](https://www.pipc.go.kr)).

Because NearbiJSX operates without user accounts or servers, most rights are exercised directly on your device.

## Automated Decision-Making

NearbiJSX does not engage in automated decision-making, profiling, or any processing that produces legal or similarly significant effects on users. The AI assistance feature, when enabled, produces code and text suggestions for your JSX artifacts; it does not make decisions about you or assign you to any category.

## Privacy Manifest

NearbiJSX includes an Apple Privacy Manifest (`PrivacyInfo.xcprivacy`) that declares:
- **Tracking domains**: Ad-related domains used by Google AdMob for ad delivery.
- **Collected data types**: Device advertising identifier (for ads) and coarse location (for weather).
- **Accessed APIs**: UserDefaults, file timestamps, and disk space — used solely for normal app operation.

## Children's Privacy

NearbiJSX does not knowingly collect any personal information from children under the age of 14 (Korean standard) or 13 (US COPPA standard) / 16 (EU GDPR standard, depending on member state). If you believe a child has provided information through our app, please contact us and we will assist where possible.

## Open Source Attribution

NearbiJSX is built on open source software. The JSX rendering engine bundles (non-exhaustive): React 18, react-runner, Sucrase, Tailwind CSS, shadcn/ui, Lucide React, Recharts, Lodash, D3.js, Three.js, Papaparse, SheetJS, and MathJS. Full license notices are available in the app under **Settings → About → Open Source Licenses**.

## Changes to This Policy

We may update this Privacy Policy from time to time. Material changes will be reflected by updating the "Last Updated" date and the "Version" field above, and will be described in the Revision History section below.

## Contact Us

If you have questions about this Privacy Policy, or wish to exercise any of your rights:

- **Email**: cs@i-nx.com
- **Developer**: INX Company Limited

## Revision History

| Version | Date | Changes |
|---|---|---|
| 1.1 | 2026-04-10 | Added Legal Basis for Processing, Data Retention, Third-Party Services (Subprocessors), International Data Transfers, Your Rights, Automated Decision-Making, Open Source Attribution, and Revision History sections. Clarified that advertising SDKs are iOS/iPadOS-only. Expanded Security and Children's Privacy sections. |
| 1.0 | 2026-04-06 | Initial Privacy Policy. |
