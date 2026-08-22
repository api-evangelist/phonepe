# PhonePe (phonepe)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

PhonePe is India's largest UPI payments network, owned by Walmart. Its PhonePe Business / Developer platform exposes the PhonePe Payment Gateway (PG) APIs for collecting payments, refunds, and status checks across UPI, cards, netbanking, and wallets, alongside in-store solutions (Static QR, Dynamic QR, Collect Call, Integrated EDC). Backend integrations are wrapped in official Java, Python, Node.js, and PHP server SDKs, with mobile SDKs for Android, iOS, Flutter, React Native, and Ionic. PhonePe also operates the Indus AppStore, a developer platform for native app distribution in India.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/phonepe/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/phonepe/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Producer
- **Access:** 3rd-Party

## Tags

- Payments
- Payment Gateway
- UPI
- QR
- EDC
- App Store
- Fintech
- India

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-05-23

## APIs

### PhonePe Payment Gateway API

Server-to-server REST API for creating PhonePe checkout orders, kicking off UPI / card / wallet / netbanking flows, and retrieving payment status. Issues redirect or intent URLs for the buyer to authorize and returns settlement-ready transaction state on completion.

- **Human URL:** [https://developer.phonepe.com/v1/docs/intro](https://developer.phonepe.com/v1/docs/intro)
- **Base URL:** `https://api.phonepe.com/apis/pg`

#### Tags

- Payments
- Checkout
- Payment Gateway

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/intro)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe Refunds API

Initiates refunds against completed PhonePe transactions and retrieves refund status. Supports partial and full refunds.

- **Human URL:** [https://developer.phonepe.com/v1/docs/refund-api](https://developer.phonepe.com/v1/docs/refund-api)
- **Base URL:** `https://api.phonepe.com/apis/pg`

#### Tags

- Refunds
- Payments

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/refund-api)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe Check Payment Status API

Polling endpoint to retrieve the current status of a payment order by merchant order ID. Used to reconcile in-store and online flows after buyer authorisation.

- **Human URL:** [https://developer.phonepe.com/v1/docs/check-status-api](https://developer.phonepe.com/v1/docs/check-status-api)
- **Base URL:** `https://api.phonepe.com/apis/pg`

#### Tags

- Status
- Reconciliation

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/check-status-api)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe S2S Callback / Webhook

Server-to-server callback that PhonePe POSTs to a merchant-configured URL on terminal payment events. Payloads are signed (X-VERIFY) so the merchant can verify authenticity before acting on the result.

- **Human URL:** [https://developer.phonepe.com/v1/docs/webhook](https://developer.phonepe.com/v1/docs/webhook)
- **Base URL:** `customer-configured`

#### Tags

- Webhooks
- Callbacks
- Events

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/webhook)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe Dynamic QR Solution

Generates per-order dynamic QR codes for in-store collection, with order-linked status retrieval and callbacks. Targeted at retail counters and quick-service merchants.

- **Human URL:** [https://developer.phonepe.com/v1/docs/dynamic-qr](https://developer.phonepe.com/v1/docs/dynamic-qr)
- **Base URL:** `https://api.phonepe.com/apis/pg`

#### Tags

- QR
- In Store
- UPI

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/dynamic-qr)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe Integrated Static QR

Onboards a merchant store with a static PhonePe QR code that maps collected funds to the merchant account. Lower-touch alternative to dynamic QR for fixed-price kiosks and stalls.

- **Human URL:** [https://developer.phonepe.com/v1/docs/static-qr](https://developer.phonepe.com/v1/docs/static-qr)
- **Base URL:** `https://api.phonepe.com/apis/pg`

#### Tags

- QR
- In Store
- Static

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/static-qr)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe Collect Call Solution

Merchant-initiated UPI collect-request flow: the merchant raises a payment request to a customer's UPI handle, the customer approves in their UPI app, and the merchant is notified on completion.

- **Human URL:** [https://developer.phonepe.com/v1/docs/collect-call](https://developer.phonepe.com/v1/docs/collect-call)
- **Base URL:** `https://api.phonepe.com/apis/pg`

#### Tags

- UPI
- Collect
- In Store

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/collect-call)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe Integrated EDC Solution

Integration with PhonePe's EDC (Electronic Data Capture / POS) terminals, allowing merchant systems to push order amounts to the terminal and receive completion events.

- **Human URL:** [https://developer.phonepe.com/v1/docs/edc](https://developer.phonepe.com/v1/docs/edc)
- **Base URL:** `https://api.phonepe.com/apis/pg`

#### Tags

- EDC
- POS
- In Store

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/edc)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe Android SDK

Native Android SDK that embeds the PhonePe checkout experience inside a merchant app, supporting the full PG flow across UPI and other payment methods.

- **Human URL:** [https://developer.phonepe.com/v1/docs/android-pg-sdk](https://developer.phonepe.com/v1/docs/android-pg-sdk)
- **Base URL:** `https://developer.phonepe.com/v1/docs/android-pg-sdk`

#### Tags

- SDK
- Android
- Mobile

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/android-pg-sdk)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe iOS SDK

Native iOS SDK that embeds the PhonePe checkout experience inside a merchant iOS app.

- **Human URL:** [https://developer.phonepe.com/v1/docs/ios-pg-sdk](https://developer.phonepe.com/v1/docs/ios-pg-sdk)
- **Base URL:** `https://developer.phonepe.com/v1/docs/ios-pg-sdk`

#### Tags

- SDK
- iOS
- Mobile

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/ios-pg-sdk)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe Flutter SDK

Flutter plugin wrapping the PhonePe Android and iOS SDKs for cross-platform mobile checkout.

- **Human URL:** [https://developer.phonepe.com/v1/docs/flutter-pg-sdk](https://developer.phonepe.com/v1/docs/flutter-pg-sdk)
- **Base URL:** `https://developer.phonepe.com/v1/docs/flutter-pg-sdk`

#### Tags

- SDK
- Flutter
- Mobile

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/flutter-pg-sdk)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe React Native SDK

React Native plugin wrapping the PhonePe Android and iOS SDKs for cross-platform mobile checkout.

- **Human URL:** [https://developer.phonepe.com/v1/docs/react-native-pg-sdk](https://developer.phonepe.com/v1/docs/react-native-pg-sdk)
- **Base URL:** `https://developer.phonepe.com/v1/docs/react-native-pg-sdk`

#### Tags

- SDK
- React Native
- Mobile

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/react-native-pg-sdk)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe Ionic SDK

Ionic plugin wrapping the PhonePe Android and iOS SDKs for hybrid mobile checkout.

- **Human URL:** [https://developer.phonepe.com/v1/docs/ionic-pg-sdk](https://developer.phonepe.com/v1/docs/ionic-pg-sdk)
- **Base URL:** `https://developer.phonepe.com/v1/docs/ionic-pg-sdk`

#### Tags

- SDK
- Ionic
- Mobile

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/ionic-pg-sdk)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe Java Backend SDK

Server-side Java SDK that wraps the PhonePe PG REST API, handling X-VERIFY signing, request modelling, and response parsing.

- **Human URL:** [https://developer.phonepe.com/v1/docs/java-backend-sdk](https://developer.phonepe.com/v1/docs/java-backend-sdk)
- **Base URL:** `https://developer.phonepe.com/v1/docs/java-backend-sdk`

#### Tags

- SDK
- Java
- Backend

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/java-backend-sdk)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe Python Backend SDK

Server-side Python SDK wrapping the PhonePe PG REST API.

- **Human URL:** [https://developer.phonepe.com/v1/docs/python-backend-sdk](https://developer.phonepe.com/v1/docs/python-backend-sdk)
- **Base URL:** `https://developer.phonepe.com/v1/docs/python-backend-sdk`

#### Tags

- SDK
- Python
- Backend

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/python-backend-sdk)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe Node.js Backend SDK

Server-side Node.js SDK wrapping the PhonePe PG REST API.

- **Human URL:** [https://developer.phonepe.com/v1/docs/node-backend-sdk](https://developer.phonepe.com/v1/docs/node-backend-sdk)
- **Base URL:** `https://developer.phonepe.com/v1/docs/node-backend-sdk`

#### Tags

- SDK
- Node.js
- Backend

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/node-backend-sdk)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### PhonePe PHP Backend SDK

Server-side PHP SDK wrapping the PhonePe PG REST API.

- **Human URL:** [https://developer.phonepe.com/v1/docs/php-backend-sdk](https://developer.phonepe.com/v1/docs/php-backend-sdk)
- **Base URL:** `https://developer.phonepe.com/v1/docs/php-backend-sdk`

#### Tags

- SDK
- PHP
- Backend

#### Properties

- [Documentation](https://developer.phonepe.com/v1/docs/php-backend-sdk)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Indus AppStore Developer Platform

PhonePe's Indus AppStore is an India-first native Android app marketplace with a developer console for app submission, listings, releases, and analytics, positioning itself as a local alternative to Google Play in India.

- **Human URL:** [https://www.indusappstore.com/developer/](https://www.indusappstore.com/developer/)
- **Base URL:** `https://www.indusappstore.com/developer/`

#### Tags

- App Store
- Distribution
- Android

#### Properties

- [Website](https://www.indusappstore.com/developer/)
- [Postman Collection](collections/phonepe.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/phonepe.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.phonepe.com/business-solutions/)
- [Documentation](https://developer.phonepe.com/)
- [LinkedIn](https://www.linkedin.com/company/phonepe)
- [Git Hub](https://github.com/PhonePe)
- [App Store](https://www.indusappstore.com/)

## Maintainers

**FN:** API Evangelist
**URL:** https://apievangelist.com
