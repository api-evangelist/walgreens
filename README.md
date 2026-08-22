# Walgreens (walgreens)

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

Walgreens is one of the largest pharmacy-led health and wellbeing companies in the United States, operating over 8,000 locations nationwide. The Walgreens Developer Program provides APIs enabling third-party applications to integrate pharmacy prescription management, vaccine scheduling, retail shopping, store locations, and product inventory. The APIs support seamless healthcare delivery, prescription refills, immunization appointments, and retail e-commerce integrations for mobile and web applications.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Producer
- **Access:** 3rd-Party

## Tags

- Pharmacy
- Healthcare
- Retail
- Prescriptions
- Vaccines

## Timestamps

- **Created:** 2025-03-01
- **Modified:** 2026-05-19

## APIs

### Walgreens Store Locator API

Returns dynamic store location data and service information for 8,000+ Walgreens and Duane Reade locations across the United States. Supports search by geolocation, address, or zip code with filtering by store services such as 24-hour pharmacy, drive-thru, healthcare clinic, photo lab, flu shots, and immunization services.

- **Human URL:** [https://developer.walgreens.com/api/storelocator/rest](https://developer.walgreens.com/api/storelocator/rest)
- **Base URL:** `https://services.walgreens.com`

#### Tags

- Store Locator
- Retail
- Pharmacy
- Geolocation

#### Properties

- [Documentation](https://developer.walgreens.com/api/storelocator/rest)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/openapi/walgreens-store-locator-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [JSON Schema](https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/json-schema/walgreens-store-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Postman Collection](collections/walgreens-prescription-refill.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/walgreens-prescription-refill.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/walgreens-store-locator.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/walgreens-store-locator.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/walgreens-vaccine-scheduling.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/walgreens-vaccine-scheduling.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Walgreens Prescription Refill API

Enables medication management application developers to process prescription refills or transfers to any Walgreens pharmacy location. Supports both barcode scanning for refill initiation and image-based prescription transfers. Processes refills from 8,200+ Walgreens pharmacies with mobile-optimized WebView checkout flows.

- **Human URL:** [https://developer.walgreens.com/api/rx/rest](https://developer.walgreens.com/api/rx/rest)
- **Base URL:** `https://services.walgreens.com`

#### Tags

- Pharmacy
- Prescriptions
- Healthcare
- Mobile

#### Properties

- [Documentation](https://developer.walgreens.com/api/rx/rest)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/openapi/walgreens-prescription-refill-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/walgreens-prescription-refill.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/walgreens-prescription-refill.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/walgreens-store-locator.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/walgreens-store-locator.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/walgreens-vaccine-scheduling.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/walgreens-vaccine-scheduling.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Walgreens Vaccine Scheduling API

Allows developers to integrate vaccine and immunization appointment booking capabilities including eligibility checking, timeslot availability, appointment holds, patient registration, and booking confirmation across all Walgreens locations in the United States and Puerto Rico. Supports 19+ vaccine types including COVID-19, influenza, RSV, and travel immunizations.

- **Human URL:** [https://developer.walgreens.com/api/scheduling/v1](https://developer.walgreens.com/api/scheduling/v1)
- **Base URL:** `https://services.walgreens.com`

#### Tags

- Vaccines
- Healthcare
- Scheduling
- Immunizations

#### Properties

- [Documentation](https://developer.walgreens.com/api/scheduling/v1)
- [OpenAPI](https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/openapi/walgreens-vaccine-scheduling-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [JSON Schema](https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/json-schema/walgreens-vaccine-appointment-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Postman Collection](collections/walgreens-prescription-refill.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/walgreens-prescription-refill.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/walgreens-store-locator.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/walgreens-store-locator.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/walgreens-vaccine-scheduling.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/walgreens-vaccine-scheduling.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Walgreens Photo Prints API

Enables developers to offer photo printing services at 8,000+ Walgreens and Duane Reade stores for same-day pickup. Supports native JSON API integration with potential revenue share commissions for qualifying partners. Prints can be ordered from mobile and web applications.

- **Human URL:** [https://developer.walgreens.com/api/photoprints/native](https://developer.walgreens.com/api/photoprints/native)
- **Base URL:** `https://services.walgreens.com`

#### Tags

- Photo Printing
- Retail
- Mobile

#### Properties

- [Documentation](https://developer.walgreens.com/api/photoprints/native)
- [Postman Collection](collections/walgreens-prescription-refill.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/walgreens-prescription-refill.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/walgreens-store-locator.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/walgreens-store-locator.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/walgreens-vaccine-scheduling.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/walgreens-vaccine-scheduling.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/Walgreens-LSG)
- [LinkedIn](https://www.linkedin.com/company/walgreens)
- [Website](https://www.walgreens.com)
- [Portal](https://developer.walgreens.com)
- [Documentation](https://developer.walgreens.com/apis)
- [Blog](https://developer.walgreens.com/blog)
- [Sign Up](https://developer.walgreens.com/user/register)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
