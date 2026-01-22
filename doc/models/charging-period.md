
# Charging Period

*This model accepts additional fields of type array.*

## Structure

`ChargingPeriod`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `startDateTime` | `?string` | Optional | - | getStartDateTime(): ?string | setStartDateTime(?string startDateTime): void |
| `dimensions` | [`?(ChargingDimension[])`](../../doc/models/charging-dimension.md) | Optional | - | getDimensions(): ?array | setDimensions(?array dimensions): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "start_date_time": "start_date_time8",
  "dimensions": [
    {
      "type": "type6",
      "volume": 148.9,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "type": "type6",
      "volume": 148.9,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

