
# Warranty Item

*This model accepts additional fields of type array.*

## Structure

`WarrantyItem`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `warrantyType` | `?string` | Optional | - | getWarrantyType(): ?string | setWarrantyType(?string warrantyType): void |
| `warrantyDisplayName` | `?string` | Optional | - | getWarrantyDisplayName(): ?string | setWarrantyDisplayName(?string warrantyDisplayName): void |
| `expirationDate` | `?DateTime` | Optional | - | getExpirationDate(): ?\DateTime | setExpirationDate(?\DateTime expirationDate): void |
| `expirationOdometer` | `?int` | Optional | - | getExpirationOdometer(): ?int | setExpirationOdometer(?int expirationOdometer): void |
| `odometerUnit` | `?string` | Optional | - | getOdometerUnit(): ?string | setOdometerUnit(?string odometerUnit): void |
| `warrantyExpiredOn` | `?string` | Optional | - | getWarrantyExpiredOn(): ?string | setWarrantyExpiredOn(?string warrantyExpiredOn): void |
| `coverageAgeInYears` | `?int` | Optional | - | getCoverageAgeInYears(): ?int | setCoverageAgeInYears(?int coverageAgeInYears): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "warrantyType": "warrantyType8",
  "warrantyDisplayName": "warrantyDisplayName0",
  "expirationDate": "2016-03-13T12:52:32.123Z",
  "expirationOdometer": 224,
  "odometerUnit": "odometerUnit6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

