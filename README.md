# PhonePe (phonepe)

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
