
# Api 1 Vehicles Wake up Response

*This model accepts additional fields of type array.*

## Structure

`Api1VehiclesWakeUpResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `response` | [`?VehicleBase`](../../doc/models/vehicle-base.md) | Optional | - | getResponse(): ?VehicleBase | setResponse(?VehicleBase response): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "response": {
    "id": 206,
    "vehicle_id": 56,
    "vin": "vin6",
    "display_name": "display_name0",
    "access_type": "access_type4",
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

