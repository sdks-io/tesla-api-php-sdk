
# Charge History

*This model accepts additional fields of type array.*

## Structure

`ChargeHistory`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `chargeStartTime` | [`ChargeStartTime`](../../doc/models/charge-start-time.md) | Required | - | getChargeStartTime(): ChargeStartTime | setChargeStartTime(ChargeStartTime chargeStartTime): void |
| `chargeDuration` | [`ChargeDuration`](../../doc/models/charge-duration.md) | Required | - | getChargeDuration(): ChargeDuration | setChargeDuration(ChargeDuration chargeDuration): void |
| `energyAddedWh` | `int` | Required | - | getEnergyAddedWh(): int | setEnergyAddedWh(int energyAddedWh): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "charge_start_time": {
    "seconds": 206,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "charge_duration": {
    "seconds": 62,
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "energy_added_wh": 176,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

