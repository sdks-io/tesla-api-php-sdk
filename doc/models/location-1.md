
# Location 1

*This model accepts additional fields of type array.*

## Structure

`Location1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `lat` | `?float` | Optional | - | getLat(): ?float | setLat(?float lat): void |
| `long` | `?float` | Optional | - | getLong(): ?float | setLong(?float long): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "lat": 224.48,
  "long": 54.54,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

