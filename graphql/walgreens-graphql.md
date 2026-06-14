# Walgreens GraphQL Schema

## Overview

This conceptual GraphQL schema represents the Walgreens API surface, covering the four public REST APIs available through the Walgreens Developer Program: Store Locator, Prescription Refill, Vaccine Scheduling, and Photo Prints. The schema also models the broader Walgreens retail, pharmacy, and health/wellness domain including loyalty rewards, insurance, product inventory, and health records.

## Provider

- **Name:** Walgreens
- **Developer Portal:** https://developer.walgreens.com/
- **Base URL:** https://services.walgreens.com
- **API Type:** REST (conceptual GraphQL representation)

## APIs Covered

| API | Documentation | Purpose |
|-----|---------------|---------|
| Store Locator API | https://developer.walgreens.com/api/storelocator/rest | Find stores by location, filter by services |
| Prescription Refill API | https://developer.walgreens.com/api/rx/rest | Manage prescription refills and transfers |
| Vaccine Scheduling API | https://developer.walgreens.com/api/scheduling/v1 | Book immunization appointments |
| Photo Prints API | https://developer.walgreens.com/api/photoprints/native | Order same-day photo prints |

## Schema Summary

The schema defines 65+ named types across the following domains:

### Store & Location
- `Store`, `PharmacyStore`, `StoreDetails`, `StoreHours`, `PharmacyHours`
- `StoreServices`, `StoreCoordinates`, `StoreAddress`

### Pharmacy & Prescriptions
- `Prescription`, `PrescriptionOrder`, `RefillRequest`, `AutoRefill`
- `PrescriptionStatus`, `RxTransfer`, `MailOrder`, `PBMClaim`

### Health Services & Vaccines
- `HealthClinic`, `MinuteClinic`, `VaccineClinic`
- `VaccineRecord`, `ImmunizationRecord`, `HealthRecord`
- `VaccineAppointment`, `AppointmentSlot`, `Patient`

### Insurance & Benefits
- `Insurance`, `InsurancePlan`, `InsuranceMember`

### Retail Products & Inventory
- `StoreInventory`, `ProductInventory`, `ProductDetails`, `ProductCategory`, `ProductImage`
- `HealthProduct`, `BeautyProduct`, `PersonalCareProduct`, `OTCProduct`, `BabyProduct`, `PetProduct`
- `Price`, `SalePrice`, `ClearancePrice`

### Photo Services
- `Photo`, `PrintOrder`, `PhotoBook`, `Photocard`, `Canvas`, `Mug`, `Ornament`
- `PhotoCenter`, `PhotoProduct`

### Loyalty & Rewards
- `MyWalgreens`, `WRewards`, `CashReward`, `RewardOffer`, `Balance`
- `Coupon`, `PaperCoupon`, `DigitalCoupon`

### Authentication
- `APIKey`, `Token`, `Webhook`

## Key Queries

```graphql
# Find stores near a location
query FindStores($lat: Float!, $lng: Float!, $radius: Int) {
  storesNearby(latitude: $lat, longitude: $lng, radiusMiles: $radius) {
    storeNumber
    name
    address { street city state zip }
    hours { open close dayOfWeek }
    services { hasPharmacy has24HourPharmacy hasDriveThru hasPhotoCenter hasHealthClinic }
  }
}

# Get prescription refill status
query GetPrescription($rxNumber: ID!) {
  prescription(rxNumber: $rxNumber) {
    rxNumber
    medicationName
    status { code description lastUpdated }
    refillsRemaining
    prescriber { name phone }
  }
}

# Check vaccine appointment availability
query CheckVaccineAvailability($storeId: ID!, $vaccineType: String!, $date: String!) {
  vaccineSlots(storeId: $storeId, vaccineType: $vaccineType, date: $date) {
    slotId
    startTime
    endTime
    available
  }
}

# Get photo print order status
query GetPhotoOrder($orderId: ID!) {
  photoOrder(orderId: $orderId) {
    orderId
    status
    pickupStore { storeNumber address { city state } }
    estimatedReadyTime
    items { productType quantity price }
  }
}
```

## Key Mutations

```graphql
# Request a prescription refill
mutation RefillPrescription($input: RefillRequestInput!) {
  refillPrescription(input: $input) {
    success
    confirmationNumber
    estimatedReadyDate
    pickupStore { storeNumber name }
  }
}

# Book a vaccine appointment
mutation BookVaccineAppointment($input: VaccineAppointmentInput!) {
  bookVaccineAppointment(input: $input) {
    confirmationNumber
    appointmentDate
    appointmentTime
    store { storeNumber address { street city state zip } }
    vaccine { name manufacturer }
  }
}

# Place a photo print order
mutation PlacePhotoOrder($input: PhotoOrderInput!) {
  placePhotoOrder(input: $input) {
    orderId
    confirmationNumber
    totalPrice
    pickupStore { storeNumber }
    estimatedReadyTime
  }
}
```

## Authentication

The Walgreens API uses API key authentication via the `apiKey` query parameter or `x-api-key` request header. OAuth tokens are used for user-specific operations involving prescription and loyalty account data.

- **Developer Registration:** https://developer.walgreens.com/user/register
- **API Key Management:** https://developer.walgreens.com/user/me/apps

## Notes

This is a conceptual GraphQL schema derived from the publicly documented Walgreens REST APIs. Walgreens does not currently offer a native GraphQL endpoint. This schema represents the domain model that could be served by a GraphQL layer over the existing REST APIs.
