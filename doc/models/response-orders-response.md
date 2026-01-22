
# Response Orders Response

*This model accepts additional fields of type array.*

## Structure

`ResponseOrdersResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `vehicleMapId` | `int` | Required | - | getVehicleMapId(): int | setVehicleMapId(int vehicleMapId): void |
| `referenceNumber` | `string` | Required | - | getReferenceNumber(): string | setReferenceNumber(string referenceNumber): void |
| `vin` | `string` | Required | - | getVin(): string | setVin(string vin): void |
| `orderStatus` | `string` | Required | - | getOrderStatus(): string | setOrderStatus(string orderStatus): void |
| `orderSubstatus` | `string` | Required | - | getOrderSubstatus(): string | setOrderSubstatus(string orderSubstatus): void |
| `modelCode` | `string` | Required | - | getModelCode(): string | setModelCode(string modelCode): void |
| `countryCode` | `string` | Required | - | getCountryCode(): string | setCountryCode(string countryCode): void |
| `locale` | `string` | Required | - | getLocale(): string | setLocale(string locale): void |
| `mktOptions` | `string` | Required | - | getMktOptions(): string | setMktOptions(string mktOptions): void |
| `isB2B` | `bool` | Required | - | getIsB2B(): bool | setIsB2B(bool isB2B): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "vehicleMapId": 198,
  "referenceNumber": "referenceNumber2",
  "vin": "vin8",
  "orderStatus": "orderStatus6",
  "orderSubstatus": "orderSubstatus2",
  "modelCode": "modelCode6",
  "countryCode": "countryCode6",
  "locale": "locale6",
  "mktOptions": "mktOptions2",
  "isB2b": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

