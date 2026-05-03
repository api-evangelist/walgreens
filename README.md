# Walgreens

Walgreens is one of the largest pharmacy-led health and wellbeing companies in the United States, operating over 8,000 locations nationwide. The Walgreens Developer Program provides APIs enabling third-party applications to integrate pharmacy prescription management, vaccine scheduling, retail shopping, store locations, and product inventory.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/walgreens/refs/heads/main/apis.yml)

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
- **Modified:** 2026-05-03

## APIs

| API | Description |
|---|---|
| [Store Locator API](https://developer.walgreens.com/api/storelocator/rest) | Search 8,000+ Walgreens locations by address, zip, or coordinates with service filtering |
| [Prescription Refill API](https://developer.walgreens.com/api/rx/rest) | Process prescription refills and transfers via barcode or image scan |
| [Vaccine Scheduling API](https://developer.walgreens.com/api/scheduling/v1) | Book immunization appointments with eligibility, timeslots, patient registration, and confirmation |
| [Photo Prints API](https://developer.walgreens.com/api/photoprints/native) | Order same-day photo prints at 8,000+ Walgreens stores |

## OpenAPI Specifications

- [walgreens-store-locator-openapi.yml](openapi/walgreens-store-locator-openapi.yml) — Store search, details, and number list
- [walgreens-prescription-refill-openapi.yml](openapi/walgreens-prescription-refill-openapi.yml) — Prescription refill and transfer flows
- [walgreens-vaccine-scheduling-openapi.yml](openapi/walgreens-vaccine-scheduling-openapi.yml) — Complete 5-step vaccine appointment workflow

## JSON Schemas

- [walgreens-store-schema.json](json-schema/walgreens-store-schema.json) — Walgreens store location data model
- [walgreens-vaccine-appointment-schema.json](json-schema/walgreens-vaccine-appointment-schema.json) — Vaccine appointment engagement model

## JSON Structure

- [walgreens-store-structure.json](json-structure/walgreens-store-structure.json) — Store data structure documentation

## JSON-LD Context

- [walgreens-context.jsonld](json-ld/walgreens-context.jsonld) — Linked data context mapping Walgreens vocabulary to schema.org

## Examples

- [walgreens-search-stores-example.json](examples/walgreens-search-stores-example.json) — Search stores by location
- [walgreens-check-vaccine-eligibility-example.json](examples/walgreens-check-vaccine-eligibility-example.json) — Check vaccine eligibility
- [walgreens-get-vaccine-timeslots-example.json](examples/walgreens-get-vaccine-timeslots-example.json) — Get available appointment times
- [walgreens-hold-vaccine-appointment-example.json](examples/walgreens-hold-vaccine-appointment-example.json) — Hold an appointment slot

## Spectral Rules

- [walgreens-rules.yml](rules/walgreens-rules.yml) — Spectral ruleset enforcing Walgreens API conventions

## Naftiko Capabilities

### Shared Definitions

- [capabilities/shared/store-locator.yaml](capabilities/shared/store-locator.yaml) — Store Locator API consumed definitions
- [capabilities/shared/vaccine-scheduling.yaml](capabilities/shared/vaccine-scheduling.yaml) — Vaccine Scheduling API consumed definitions

### Workflow Capabilities

- [capabilities/pharmacy-and-healthcare.yaml](capabilities/pharmacy-and-healthcare.yaml) — Unified pharmacy and healthcare workflow combining store locator and vaccine scheduling (6 REST endpoints, 6 MCP tools)

## Vocabulary

- [walgreens-vocabulary.yml](vocabulary/walgreens-vocabulary.yml) — Pharmacy, vaccine, and retail operations vocabulary

## Common Properties

- [Website](https://www.walgreens.com)
- [Developer Portal](https://developer.walgreens.com)
- [API Catalog](https://developer.walgreens.com/apis)
- [Blog](https://developer.walgreens.com/blog)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
