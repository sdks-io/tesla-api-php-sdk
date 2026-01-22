
# Off Grid Vehicle Charging Reserve Request

*This model accepts additional fields of type array.*

## Structure

`OffGridVehicleChargingReserveRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `offGridVehicleChargingReservePercent` | `int` | Required | - | getOffGridVehicleChargingReservePercent(): int | setOffGridVehicleChargingReservePercent(int offGridVehicleChargingReservePercent): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "off_grid_vehicle_charging_reserve_percent": 228,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

