
# Tou Settings

*This model accepts additional fields of type array.*

## Structure

`TouSettings`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `tariffContentV2` | `?array` | Optional | - | getTariffContentV2(): ?array | setTariffContentV2(?array tariffContentV2): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "tariff_content_v2": {
    "key1": "val1",
    "key2": "val2"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

