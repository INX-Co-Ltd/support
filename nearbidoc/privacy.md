# Privacy Policy

**Last Updated: April 10, 2026**
**Version: 1.1**

INX Company Limited ("we", "our", "us") operates the nearbidoc application. This Privacy Policy explains how we collect, use, and protect your information when you use our app.

nearbidoc is designed as a **privacy-first, local-first** application. We do not operate any servers that receive your personal information, and we do not run analytics, tracking, or advertising SDKs.

## Information We Collect

### Location Data
- We access your approximate location **only** to provide weather-aware greetings on the home screen.
- Your approximate location is sent to **Apple Weather (WeatherKit)** to retrieve current weather conditions. This data is handled by Apple under [Apple's Privacy Policy](https://www.apple.com/privacy/). We do not receive, store, or forward your location data to any other party.
- Weather data is provided by Apple Weather. See [Apple Weather attribution](https://weatherkit.apple.com/legal-attribution.html) for details.
- You can deny location access at any time in your device settings. The app works fully without it.

### iCloud Data
- Documents you create are stored in your personal iCloud container if you choose iCloud storage.
- This data is managed entirely by Apple's iCloud service. We do not have access to your iCloud data.

### AI API Keys and Prompts
- If you use the AI writing assistant feature, you provide your own API keys (Claude, OpenAI, Gemini, GitHub Models).
- API keys are stored locally in your device's Keychain. They are **never transmitted to our servers**.
- API requests are sent directly from your device to the respective AI provider.
- **Important**: The content of your prompts (document text you send to the AI) is transmitted to the AI provider you select. Each provider applies its own data handling policy, which may include temporary retention for abuse prevention, safety review, or model improvement. For example, Anthropic may retain prompt data for up to 30 days and, depending on your account settings with Anthropic, may use prompts to improve their models. Review the provider's privacy policy (linked in the "Third-Party Services" section below) before sending sensitive or confidential content through the AI assistant.

## Information We Do NOT Collect

- We do **not** collect personal information, usage analytics, or crash reports.
- We do **not** use any third-party analytics or tracking SDKs.
- We do **not** have user accounts or login systems.
- We do **not** operate any servers that receive your data.
- We do **not** display advertisements or integrate any advertising SDKs.

## Legal Basis for Processing

Under the EU General Data Protection Regulation (GDPR) and the Korean Personal Information Protection Act (PIPA), we rely on the following legal bases for any limited processing that occurs:

- **Consent** — Location access for weather greetings, and use of the optional AI writing assistant. You may withdraw consent at any time through device settings or by not using the feature.
- **Performance of contract** — Processing necessary to deliver the app you purchased (e.g., in-app purchase verification via Apple StoreKit).
- **Legitimate interests** — Ensuring the security and integrity of the app (e.g., Keychain storage of sensitive credentials).

## Data Retention

- **Documents, settings, and preferences** are retained on your device (and, if you opt-in, your personal iCloud container) until you delete them. We have no ability to delete or access this data on our end.
- **Location data** is processed in memory for a single weather request and is not persisted by the app.
- **AI prompts** are transmitted directly to the AI provider you selected and are not logged, stored, or retained by us.
- **Weather data** is cached on-device for up to 30 minutes to reduce redundant API calls.

## Peer-to-Peer Collaboration

- Real-time collaboration uses Apple's local networking (MultipeerConnectivity, Network.framework, and Core Bluetooth).
- The app requests **Local Network** and **Bluetooth** permissions to discover and connect with nearby devices.
- All communication happens directly between nearby devices. Document data shared during collaboration is **not routed through any external server**.
- Apple's MultipeerConnectivity framework provides TLS-based transport security between peers by default.

## In-App Purchases

- Purchase transactions are processed entirely by Apple's App Store. We do not collect or store any payment information.

## Data Storage and Security

- All documents, settings, and preferences are stored locally on your device or in your personal iCloud container.
- No data is stored on our servers.
- **API keys** (Claude, OpenAI, Gemini, GitHub Models) are stored in the Apple **Keychain**, which is protected by device-level encryption.
- **Network transport** to AI providers uses HTTPS (TLS 1.2+).
- **iCloud** data is encrypted in transit and at rest by Apple. See [Apple's iCloud security overview](https://support.apple.com/en-us/HT202303).

## Third-Party Services (Subprocessors)

Because nearbidoc does not operate its own servers, all network activity flows directly from your device to the third-party services you choose to use. The following services may receive data from your device when you use the corresponding feature:

| Service | Provider | Purpose | Data Transferred | When |
|---|---|---|---|---|
| Apple WeatherKit | Apple Inc. (USA) | Weather greetings | Coarse location (reduced accuracy) | Only when location permission is granted |
| Apple iCloud | Apple Inc. (USA) | Optional document sync | Documents you create | Only if you enable iCloud storage |
| Apple App Store / StoreKit | Apple Inc. (USA) | In-app purchase processing | Anonymized transaction IDs | When you purchase Pro features |
| Anthropic Claude | Anthropic PBC (USA) | AI writing assistant | Your prompt text | Only when you invoke the AI feature with a Claude key |
| OpenAI | OpenAI OpCo, LLC (USA) | AI writing assistant | Your prompt text | Only when you invoke the AI feature with an OpenAI key |
| Google Gemini | Google LLC (USA) | AI writing assistant | Your prompt text | Only when you invoke the AI feature with a Gemini key |
| GitHub Models | Microsoft Corporation (USA) | AI writing assistant | Your prompt text | Only when you invoke the AI feature with a GitHub token |

Each provider has its own privacy policy governing how it handles data it receives:
- [Apple Privacy Policy](https://www.apple.com/privacy/)
- [Anthropic Privacy Policy](https://www.anthropic.com/legal/privacy)
- [OpenAI Privacy Policy](https://openai.com/policies/privacy-policy/)
- [Google Privacy Policy](https://policies.google.com/privacy)
- [Microsoft Privacy Statement](https://privacy.microsoft.com/en-us/privacystatement)

## International Data Transfers

nearbidoc is distributed worldwide. When you use the features listed in the Third-Party Services table above, data may be transferred to the United States and other jurisdictions where those providers operate their infrastructure. By enabling the corresponding feature (location, iCloud, AI assistant), you acknowledge that the relevant data is transferred to the selected provider outside your country of residence.

We do not transfer your data to any party other than those third-party services that you have actively chosen to use.

## Your Rights

Depending on your jurisdiction (EU/UK under GDPR, California under CCPA/CPRA, Korea under PIPA), you may have the following rights regarding your personal information:

- **Access** — Request a copy of the information we hold about you. (Because we store nothing on our servers, this is effectively achieved by browsing the app's files and settings on your device.)
- **Rectification** — Correct inaccurate information. You can edit all in-app data directly.
- **Erasure** — Delete your information. You can delete files, clear app storage, or uninstall the app to remove all local data.
- **Portability** — Obtain your data in a portable format. The app lets you export documents as Markdown, PDF, DOCX, and HWP.
- **Withdraw consent** — Revoke permissions (location, Bluetooth, Local Network) in your device settings at any time.
- **Object / restrict processing** — Contact us at cs@i-nx.com.
- **Lodge a complaint** — You may contact your local data protection authority. In Korea, that is the Personal Information Protection Commission ([pipc.go.kr](https://www.pipc.go.kr)).

Because nearbidoc operates without user accounts or servers, most rights are exercised directly on your device.

## Automated Decision-Making

nearbidoc does not engage in automated decision-making, profiling, or any processing that produces legal or similarly significant effects on users. The AI writing assistant, when enabled, produces text suggestions for your documents; it does not make decisions about you or assign you to any category.

## Children's Privacy

nearbidoc is intended for use by university students and adults. We do not knowingly collect any personal information from children under the age of 14 (Korean standard) or 13 (US COPPA standard) / 16 (EU GDPR standard, depending on member state). If you believe a child has provided information through our app, please contact us and we will assist where possible.

## Open Source Attribution

nearbidoc is built on open source software. Components include (non-exhaustive): Tiptap, ProseMirror, Yjs, y-prosemirror, markdown-it, docx, esbuild, Yams, and others. Full license notices are available in the app under **Settings → About → Open Source Licenses**, and in our source repository.

## Changes to This Policy

We may update this Privacy Policy from time to time. Material changes will be reflected by updating the "Last Updated" date and the "Version" field above, and will be described in the Revision History section below.

## Contact Us

If you have questions about this Privacy Policy, or wish to exercise any of your rights:

- **Email**: cs@i-nx.com
- **Developer**: INX Company Limited

## Revision History

| Version | Date | Changes |
|---|---|---|
| 1.1 | 2026-04-10 | Added Legal Basis for Processing, Data Retention, Third-Party Services (Subprocessors), International Data Transfers, Your Rights, Open Source Attribution, and Revision History sections. Expanded Security and Children's Privacy sections. |
| 1.0 | 2026-04-06 | Initial Privacy Policy. |
