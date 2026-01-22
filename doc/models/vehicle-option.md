
# Vehicle Option

*This model accepts additional fields of type array.*

## Structure

`VehicleOption`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `code` | `?string` | Optional | - | getCode(): ?string | setCode(?string code): void |
| `displayName` | `?string` | Optional | - | getDisplayName(): ?string | setDisplayName(?string displayName): void |
| `colorCode` | `?string` | Optional | - | getColorCode(): ?string | setColorCode(?string colorCode): void |
| `isActive` | `?bool` | Optional | - | getIsActive(): ?bool | setIsActive(?bool isActive): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "code": "code2",
  "displayName": "displayName8",
  "colorCode": "colorCode4",
  "isActive": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

