
# Api 1 Vehicles Nearby Charging Sites Response

*This model accepts additional fields of type array.*

## Structure

`Api1VehiclesNearbyChargingSitesResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `response` | [`?Response3`](../../doc/models/response-3.md) | Optional | - | getResponse(): ?Response3 | setResponse(?Response3 response): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "response": {
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
    "timestamp": 244,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

