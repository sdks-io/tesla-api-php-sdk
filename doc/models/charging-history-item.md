
# Charging History Item

*This model accepts additional fields of type array.*

## Structure

`ChargingHistoryItem`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `sessionId` | `int` | Required | - | getSessionId(): int | setSessionId(int sessionId): void |
| `vin` | `string` | Required | - | getVin(): string | setVin(string vin): void |
| `siteLocationName` | `?string` | Optional | - | getSiteLocationName(): ?string | setSiteLocationName(?string siteLocationName): void |
| `chargeStartDateTime` | `?DateTime` | Optional | - | getChargeStartDateTime(): ?\DateTime | setChargeStartDateTime(?\DateTime chargeStartDateTime): void |
| `chargeStopDateTime` | `?DateTime` | Optional | - | getChargeStopDateTime(): ?\DateTime | setChargeStopDateTime(?\DateTime chargeStopDateTime): void |
| `unlatchDateTime` | `?DateTime` | Optional | - | getUnlatchDateTime(): ?\DateTime | setUnlatchDateTime(?\DateTime unlatchDateTime): void |
| `countryCode` | `?string` | Optional | - | getCountryCode(): ?string | setCountryCode(?string countryCode): void |
| `fees` | [`?(ChargingFee[])`](../../doc/models/charging-fee.md) | Optional | - | getFees(): ?array | setFees(?array fees): void |
| `billingType` | `?string` | Optional | - | getBillingType(): ?string | setBillingType(?string billingType): void |
| `invoices` | [`?(ChargingInvoice[])`](../../doc/models/charging-invoice.md) | Optional | - | getInvoices(): ?array | setInvoices(?array invoices): void |
| `vehicleMakeType` | `?string` | Optional | - | getVehicleMakeType(): ?string | setVehicleMakeType(?string vehicleMakeType): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "sessionId": 16,
  "vin": "vin0",
  "siteLocationName": "siteLocationName8",
  "chargeStartDateTime": "2016-03-13T12:52:32.123Z",
  "chargeStopDateTime": "2016-03-13T12:52:32.123Z",
  "unlatchDateTime": "2016-03-13T12:52:32.123Z",
  "countryCode": "countryCode8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

