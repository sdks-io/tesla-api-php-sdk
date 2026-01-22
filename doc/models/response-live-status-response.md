
# Response Live Status Response

*This model accepts additional fields of type array.*

## Structure

`ResponseLiveStatusResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `solarPower` | `float` | Required | - | getSolarPower(): float | setSolarPower(float solarPower): void |
| `energyLeft` | `float` | Required | - | getEnergyLeft(): float | setEnergyLeft(float energyLeft): void |
| `totalPackEnergy` | `float` | Required | - | getTotalPackEnergy(): float | setTotalPackEnergy(float totalPackEnergy): void |
| `percentageCharged` | `float` | Required | - | getPercentageCharged(): float | setPercentageCharged(float percentageCharged): void |
| `backupCapable` | `bool` | Required | - | getBackupCapable(): bool | setBackupCapable(bool backupCapable): void |
| `batteryPower` | `?float` | Optional | - | getBatteryPower(): ?float | setBatteryPower(?float batteryPower): void |
| `loadPower` | `?float` | Optional | - | getLoadPower(): ?float | setLoadPower(?float loadPower): void |
| `gridStatus` | `?string` | Optional | - | getGridStatus(): ?string | setGridStatus(?string gridStatus): void |
| `gridPower` | `?float` | Optional | - | getGridPower(): ?float | setGridPower(?float gridPower): void |
| `islandStatus` | `?string` | Optional | - | getIslandStatus(): ?string | setIslandStatus(?string islandStatus): void |
| `stormModeActive` | `?bool` | Optional | - | getStormModeActive(): ?bool | setStormModeActive(?bool stormModeActive): void |
| `timestamp` | `?DateTime` | Optional | - | getTimestamp(): ?\DateTime | setTimestamp(?\DateTime timestamp): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "solar_power": 108.14,
  "energy_left": 185.46,
  "total_pack_energy": 65.2,
  "percentage_charged": 141.22,
  "backup_capable": false,
  "battery_power": 211.48,
  "load_power": 248.74,
  "grid_status": "grid_status2",
  "grid_power": 38.0,
  "island_status": "island_status4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

