# PhonePe

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

**Areas:** Payments · Payment Gateway · UPI · QR · EDC · App Store · Fintech · India

## PhonePe on APIs.io

Everything profiled for PhonePe is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/phonepe/](https://apis.io/providers/phonepe/)** — or go straight to one of the APIs or properties below.

### APIs (21)

- [PhonePe Payment Gateway API](https://apis.io/apis/phonepe/pg/) — Server-to-server REST API for creating PhonePe checkout orders, kicking off UPI / card / wallet / netbanking flows, and retrieving payment status. Issues…
- [PhonePe Refunds API](https://apis.io/apis/phonepe/refunds/) — Initiates refunds against completed PhonePe transactions and retrieves refund status. Supports partial and full refunds.
- [PhonePe Check Payment Status API](https://apis.io/apis/phonepe/status/) — Polling endpoint to retrieve the current status of a payment order by merchant order ID. Used to reconcile in-store and online flows after buyer authorisation.
- [PhonePe S2S Callback / Webhook](https://apis.io/apis/phonepe/webhook/) — Server-to-server callback that PhonePe POSTs to a merchant-configured URL on terminal payment events. Payloads are signed (X-VERIFY) so the merchant can…
- [PhonePe Dynamic QR Solution](https://apis.io/apis/phonepe/dynamic-qr/) — Generates per-order dynamic QR codes for in-store collection, with order-linked status retrieval and callbacks. Targeted at retail counters and…
- [PhonePe Integrated Static QR](https://apis.io/apis/phonepe/static-qr/) — Onboards a merchant store with a static PhonePe QR code that maps collected funds to the merchant account. Lower-touch alternative to dynamic QR for…
- [PhonePe Collect Call Solution](https://apis.io/apis/phonepe/collect-call/) — Merchant-initiated UPI collect-request flow: the merchant raises a payment request to a customer's UPI handle, the customer approves in their UPI app, and…
- [PhonePe Integrated EDC Solution](https://apis.io/apis/phonepe/edc/) — Integration with PhonePe's EDC (Electronic Data Capture / POS) terminals, allowing merchant systems to push order amounts to the terminal and receive…
- [PhonePe Android SDK](https://apis.io/apis/phonepe/android-sdk/) — Native Android SDK that embeds the PhonePe checkout experience inside a merchant app, supporting the full PG flow across UPI and other payment methods.
- [PhonePe iOS SDK](https://apis.io/apis/phonepe/ios-sdk/) — Native iOS SDK that embeds the PhonePe checkout experience inside a merchant iOS app.
- [PhonePe Flutter SDK](https://apis.io/apis/phonepe/flutter-sdk/) — Flutter plugin wrapping the PhonePe Android and iOS SDKs for cross-platform mobile checkout.
- [PhonePe React Native SDK](https://apis.io/apis/phonepe/react-native-sdk/) — React Native plugin wrapping the PhonePe Android and iOS SDKs for cross-platform mobile checkout.
- [PhonePe Ionic SDK](https://apis.io/apis/phonepe/ionic-sdk/) — Ionic plugin wrapping the PhonePe Android and iOS SDKs for hybrid mobile checkout.
- [PhonePe Java Backend SDK](https://apis.io/apis/phonepe/java-sdk/) — Server-side Java SDK that wraps the PhonePe PG REST API, handling X-VERIFY signing, request modelling, and response parsing.
- [PhonePe Python Backend SDK](https://apis.io/apis/phonepe/python-sdk/) — Server-side Python SDK wrapping the PhonePe PG REST API.
- [PhonePe Node.js Backend SDK](https://apis.io/apis/phonepe/node-sdk/) — Server-side Node.js SDK wrapping the PhonePe PG REST API.
- [PhonePe PHP Backend SDK](https://apis.io/apis/phonepe/php-sdk/) — Server-side PHP SDK wrapping the PhonePe PG REST API.
- [Indus AppStore Developer Platform](https://apis.io/apis/phonepe/indus-appstore/) — PhonePe's Indus AppStore is an India-first native Android app marketplace with a developer console for app submission, listings, releases, and analytics,…
- [PhonePe Checkout API](https://apis.io/apis/phonepe/phonepe-checkout-api/) — Create payment orders.
- [PhonePe Order Status API](https://apis.io/apis/phonepe/phonepe-order-status-api/) — Retrieve the status of a payment order.
- [PhonePe Refunds API](https://apis.io/apis/phonepe/phonepe-refunds-api/) — Initiate and track refunds.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Phonepe Agentic Access](https://apis.io/agentic-access/phonepe/phonepe-agentic-access/)

#### Collections (4)

Postman and Open Collection request collections.

- [PhonePe Payment Gateway API](https://apis.io/collections/phonepe/open-phonepe/)
- [PhonePe Payment Gateway Checkout API](https://apis.io/collections/phonepe/open-phonepe-checkout-api/)
- [PhonePe Payment Gateway Checkout Order Status API](https://apis.io/collections/phonepe/open-phonepe-order-status-api/)
- [PhonePe Payment Gateway Checkout Refunds API](https://apis.io/collections/phonepe/open-phonepe-refunds-api/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Phonepe Authentication](https://apis.io/security/phonepe/phonepe-authentication/)
- [Phonepe Domain Security](https://apis.io/security/phonepe/phonepe-domain-security/)
- [Phonepe Vulnerability Disclosure](https://apis.io/security/phonepe/phonepe-vulnerability-disclosure/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Phonepe Plans Pricing](https://apis.io/plans/phonepe/phonepe-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Phonepe Rate Limits](https://apis.io/rate-limits/phonepe/phonepe-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Phonepe Finops](https://apis.io/finops/phonepe/phonepe-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.phonepe.com/business-solutions/)
- [Documentation](https://developer.phonepe.com/)
- [Blog](https://www.phonepe.com/press/)

## API Evangelist rating

**Kin Score 24.7** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 60.7 |
| Contract quality | 50.6 |
| Contract governance | 0.0 |
| Operational transparency | 10.5 |
| Developer ergonomics | 23.8 |
| Access clarity | 5.3 |

**Agent readiness 19.6** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 16.1** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/phonepe/](https://apis.io/providers/phonepe/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for PhonePe: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/phonepe/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
