
# Response 3

*This model accepts additional fields of type array.*

## Structure

`Response3`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `destinationCharging` | [`?(ChargingLocation[])`](../../doc/models/charging-location.md) | Optional | - | getDestinationCharging(): ?array | setDestinationCharging(?array destinationCharging): void |
| `superchargers` | [`?(ChargingLocation[])`](../../doc/models/charging-location.md) | Optional | - | getSuperchargers(): ?array | setSuperchargers(?array superchargers): void |
| `timestamp` | `?int` | Optional | - | getTimestamp(): ?int | setTimestamp(?int timestamp): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "destination_charging": [
    {
      "name": "name8",
      "type": "type2",
      "distance_miles": 106.72,
      "amenities": "amenities8",
      "available_stalls": 140,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "name": "name8",
      "type": "type2",
      "distance_miles": 106.72,
      "amenities": "amenities8",
      "available_stalls": 140,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "name": "name8",
      "type": "type2",
      "distance_miles": 106.72,
      "amenities": "amenities8",
      "available_stalls": 140,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "superchargers": [
    {
      "name": "name0",
      "type": "type0",
      "distance_miles": 190.44,
      "amenities": "amenities0",
      "available_stalls": 64,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "timestamp": 194,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

