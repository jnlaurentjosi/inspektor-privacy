# Privacy Policy for Inspektor: Make Your Bed

**Effective date: August 12, 2026**

Inspektor: Make Your Bed ("Inspektor", "the app") is a morning alarm and AI room-inspection app for iOS. You photograph your room, an AI model analyses the photos, and you receive a cleanliness score and a fictional "military sergeant" verdict.

This policy explains what data the app handles, where it goes, and what your rights are. It is written to be read, not skimmed. The short version comes first.

## The short version

**Inspektor has no accounts, no sign-up, no login, and no user database.** We do not know your name or your email address, and we cannot link any inspection to a person. Everything the app knows about you (your photos, your scores, your streaks, your alarm times) lives on your iPhone, and only on your iPhone. Deleting the app deletes all of it.

The one thing that leaves your device is the photos you choose to submit for inspection. They are sent, over an encrypted connection, through a small relay server we operate and on to Anthropic (the company behind the Claude AI model) so the analysis can be produced. Our relay does not store your photos or your results; it keeps only short-lived technical logs (see section 3). Anthropic processes your photos to return the analysis and automatically deletes API inputs and outputs from its systems within 30 days; it does not use them to train its AI models.

The score you receive is generated automatically by an AI model. It is a coaching score inside a habit app: it has no legal or similarly significant effect on you (see section 4).

There are no ads, no third-party analytics SDKs, no tracking, and no sale of data. Ever.

## 1. Who we are

Inspektor is published and operated by:

**Jean-Nicolas Laurent Josi**, independent developer (indépendant / zelfstandige)
Based in Belgium
Contact: **jnlaurentjosi@gmail.com**

For the purposes of the EU General Data Protection Regulation (GDPR), Jean-Nicolas Laurent Josi is the data controller for the limited processing described in this policy. We have declared trader status under the EU Digital Services Act; our trader contact details are displayed on the app's App Store page.

We have not designated a Data Protection Officer, because the scale and nature of our processing do not require one under Art. 37 GDPR. Privacy questions go directly to the developer at the address above.

## 2. What data the app handles, and why

| Data | What happens to it | Why | Leaves your device? |
|---|---|---|---|
| **Room photos** (typically 2 per inspection, plus an optional "benchmark" photo of your room at its best) | Sent over HTTPS through our relay server to Anthropic's Claude API to generate your inspection score and verdict. Stored **only on your device** afterwards, as part of your inspection history. | To provide the core AI inspection feature. | Yes, transiently, for analysis only (see section 3). |
| **Inspection history** (scores, verdicts, deltas, dates) | Stored locally on your device. | So you can see your progress, streaks, and ranks. | No. |
| **Alarm and habit data** (wake-up times, duty days, streaks, ranks, onboarding answers) | Stored locally on your device. | To run alarms, streaks, and the rank ladder. | No. |
| **Subscription data** (App Store receipt, product identifier, a randomly generated pseudonymous app user ID) | Processed by Apple (payment) and RevenueCat (subscription management). We never see your name, email, or payment card details. | To activate and manage your subscription and free trial. | Yes, to Apple and RevenueCat. |
| **Relay server logs** (timestamp, IP address, technical request metadata; never your photos or results) | Kept briefly on our relay server for security and troubleshooting, then automatically deleted within 7 days. | To keep the service secure and detect abuse. | Yes (generated when your device contacts our relay). |
| **Local notifications** (alarms, reminders) | Scheduled entirely on your device by iOS. | To wake you up and remind you. | No. |

That is the complete list. The app collects no contact details, no location data, no contacts, no health data, no advertising identifiers, and no browsing data.

A note on IP addresses: like every internet service, our relay sees the IP address your device connects from, and an IP address can be personal data under the GDPR. We use it only in the short-lived security logs described above. We never use it to identify you, profile you, or link inspections together, and it is deleted within 7 days.

## 3. Your photos and AI analysis

Photos are the most sensitive thing the app touches, so here is exactly what happens.

**Before any photo is taken**, the app shows a dedicated consent screen during onboarding explaining that photos you submit will be sent for AI analysis. The inspection feature only works if you agree. You can decline, and you can withdraw your consent at any time (see section 9).

**When you submit an inspection**, your photos travel over an encrypted HTTPS connection through a minimal relay server that we operate. This relay exists for one reason: it keeps our AI service credentials off your device, which protects the service from abuse. The relay forwards your photos to Anthropic's Claude API and forwards the analysis back to your app. **The relay does not store your photos or your inspection results.** It keeps only the short-lived technical logs described in section 2, which never contain your photos, and which are deleted within 7 days.

**Anthropic** processes the photos solely to return the analysis to you. Under Anthropic's commercial API terms, API inputs and outputs are **not used to train Anthropic's AI models**, and Anthropic automatically deletes API inputs and outputs from its systems **within 30 days** of processing. Anthropic may retain data for longer only in the exceptional case where content is flagged by its safety systems as violating its usage policy. You can read Anthropic's commercial terms and privacy documentation at [anthropic.com](https://www.anthropic.com) and [privacy.claude.com](https://privacy.claude.com).

**After the analysis**, your photos and results are stored only on your device, in the app's local storage. We operate no database of user content and have no way to view, retrieve, or restore your photos.

**Please photograph your room, not your life.** Photos of a room can incidentally capture things that reveal more than tidiness: documents on a desk, medication on a nightstand, religious or political items, medical equipment, photos of other people. We ask you to frame your room only and to keep such items (and other people) out of frame. The AI model is instructed to assess tidiness and order only. If something sensitive is captured incidentally despite this, it is processed transiently as described above, is never stored on any server we operate, and is deleted from Anthropic's systems within 30 days. We do not seek, extract, or use any such information.

## 4. Automated analysis, not automated decisions

Your inspection score and verdict are generated automatically by an AI model, without human review. We want to be explicit about what that means and does not mean.

The score is a coaching signal inside a habit-building app. It does not produce legal effects for you and does not similarly significantly affect you: it does not affect your access to any service, price, credit, employment, or anything comparable. It affects only your in-app streaks, ranks, and the tone of a fictional sergeant. This means the restrictions on solely automated decision-making in Art. 22 GDPR do not apply. We tell you this anyway, because Art. 13(2)(f) GDPR asks controllers to be transparent about automated processing, and because you deserve to know that no human looks at your photos on our side: the entire analysis is machine-performed, transiently, as described in section 3.

For the purposes of the EU Artificial Intelligence Act's transparency requirements: yes, you are interacting with an AI system. The app says so plainly, during onboarding and throughout the experience. The sergeants are fictional characters voiced by an AI model; the scoring is AI-generated.

## 5. Third parties we work with

We deliberately work with as few third parties as possible. There are three.

**Anthropic, PBC (United States)** provides the Claude AI model that analyses your photos, acting as our processor under a data processing agreement incorporating the European Commission's Standard Contractual Clauses. Photos are processed to return your inspection result, are not used for AI training under Anthropic's commercial terms, and are automatically deleted within 30 days as described in section 3.

**RevenueCat, Inc. (United States)** provides subscription infrastructure, acting as our processor under a data processing agreement incorporating the Standard Contractual Clauses. RevenueCat receives your App Store purchase receipt, the product you purchased, and a randomly generated pseudonymous app user ID created on your device. It does not receive your name, email address, or payment details. RevenueCat's privacy policy is at [revenuecat.com/privacy](https://www.revenuecat.com/privacy).

**Apple Inc.** distributes the app and handles all payments through the App Store, under your existing agreement with Apple and Apple's own privacy policy. We additionally see aggregated, anonymised App Store analytics that Apple provides to all developers (based on users who have opted in to sharing analytics with developers in iOS settings).

The app is built with the Expo / React Native framework. To our knowledge, no framework telemetry runs from users' devices in our production app; the framework's tooling operates at build time on our own machines.

We do not use advertising networks, third-party analytics SDKs, social logins, or data brokers. We do not sell or share personal data for advertising, and the app performs no "tracking" as defined by Apple's App Tracking Transparency framework.

## 6. Legal bases (GDPR)

For users in the EU/EEA, UK, and Switzerland, we rely on the following legal bases:

- **Consent** (Art. 6(1)(a) GDPR), for sending your photos for AI analysis. You give this consent on the dedicated screen during onboarding, before any photo is taken. You can withdraw it at any time with the "AI analysis" switch in the app's Settings, which disables the inspection feature; withdrawing is exactly as easy as consenting was. Withdrawal does not affect the lawfulness of processing before withdrawal.
- **Performance of a contract** (Art. 6(1)(b) GDPR), for processing subscription and purchase data needed to provide your paid subscription.
- **Legitimate interests** (Art. 6(1)(f) GDPR), for the short-lived technical logs on our relay server, used to keep the service secure and functioning. Our interest is protecting the service from abuse; the impact on you is minimal because no content is stored and logs are deleted within 7 days.

Data stored only on your device (inspection history, alarms, streaks) is under your control; we never access it.

## 7. International transfers

Anthropic and RevenueCat are based in the United States, so the limited data described above is transferred outside the EU/EEA.

**For EU/EEA users**, these transfers are safeguarded by the **Standard Contractual Clauses (SCCs)** approved by the European Commission, incorporated into the data processing agreements we have with each provider, together with technical measures including encryption in transit. Where a provider is additionally certified under the **EU–U.S. Data Privacy Framework**, transfers to that provider may also rely on the European Commission's adequacy decision for the Framework.

**For UK users**, the same transfers are safeguarded by the UK International Data Transfer Addendum to the SCCs (or the UK IDTA), and, where the provider is certified under the **UK Extension to the EU–U.S. Data Privacy Framework**, by the UK's adequacy regulations for that Extension.

**For Swiss users**, the transfers are safeguarded by the SCCs as adapted for Swiss law in line with the guidance of the Swiss Federal Data Protection and Information Commissioner (FDPIC), and, where applicable, by the **Swiss–U.S. Data Privacy Framework**.

## 8. Retention

- **On your device:** photos, inspection history, and all habit data remain until you delete them in the app or delete the app itself. Deleting the app deletes everything.
- **Our relay server:** photos and results are never stored. Technical security logs are automatically deleted within **7 days**.
- **Anthropic:** API inputs and outputs are automatically deleted within 30 days, with the safety exception described in section 3.
- **RevenueCat:** retains subscription records for as long as needed to manage subscriptions and meet its legal obligations, as described in its own privacy policy.
- **Apple:** retains purchase records under its own policies, as for any App Store purchase.

## 9. Your rights

Under the GDPR you have rights of access, rectification, erasure, restriction, portability, and objection, and the right to withdraw consent at any time.

Here is the honest picture of how those rights work with an app built like this one:

- **Withdrawing consent for AI analysis** takes one tap: Settings → "AI analysis". Turning it off disables the inspection feature until you turn it back on. You can also simply delete the app.
- **For your photos and inspection data**, you already hold the data and the controls. Everything is on your device: you can view it, export it (your photos are ordinary images), and erase it instantly by deleting your history or the app. We could not fulfil an access or erasure request on our side even if we wanted to, because we hold no user content and cannot identify which data would be yours. GDPR recognises this situation: where a controller cannot identify a data subject, certain rights obligations do not apply (Art. 11 GDPR).
- **For subscription data**, contact us at jnlaurentjosi@gmail.com and we will coordinate with RevenueCat, or you can contact RevenueCat directly. Payment data is held by Apple and subject to your rights under Apple's policies.
- **For anything else**, email us at **jnlaurentjosi@gmail.com**. We respond within one month.

You also have the right to lodge a complaint with a supervisory authority. As we are based in Belgium, our lead authority is the Belgian Data Protection Authority (Autorité de protection des données / Gegevensbeschermingsautoriteit), [dataprotectionauthority.be](https://www.dataprotectionauthority.be). UK users may complain to the Information Commissioner's Office (ICO), Swiss users to the FDPIC, and any user may contact the authority in their own country.

**For users in the United States:** we do not sell personal information, do not share it for cross-context behavioural advertising, and do not meet the business thresholds of the California Consumer Privacy Act. The descriptions in this policy apply to you all the same.

## 10. Children

Inspektor is not directed at children under 13, and we do not knowingly collect personal data from children. The app has no accounts and no way for anyone, child or adult, to submit personal details to us. If you believe a child has used the app in a way that concerns you, contact us and we will help.

## 11. Security

- All network traffic uses HTTPS/TLS encryption.
- There is no user database to breach: we store no user content on any server.
- Our AI service credentials are kept off your device, on our relay server, precisely to prevent abuse.
- Data on your device is protected by iOS's built-in protections (device passcode, encryption at rest).

No system is perfectly secure, but the most effective security measure in this app is architectural: the data we never collect is data that can never leak from us.

## 12. Changes to this policy

If we change this policy, we will post the updated version at this address with a new effective date. If a change materially affects how your photos are processed, we will ask for your consent again in the app before the change applies to you.

## 13. Contact

**Jean-Nicolas Laurent Josi**
Independent developer, Belgium
**jnlaurentjosi@gmail.com**

We read every email.
