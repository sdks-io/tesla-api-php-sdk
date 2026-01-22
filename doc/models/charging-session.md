
# Charging Session

*This model accepts additional fields of type array.*

## Structure

`ChargingSession`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `id` | `?string` | Optional | - | getId(): ?string | setId(?string id): void |
| `vin` | `?string` | Optional | - | getVin(): ?string | setVin(?string vin): void |
| `model` | `?string` | Optional | - | getModel(): ?string | setModel(?string model): void |
| `startDateTime` | `?string` | Optional | - | getStartDateTime(): ?string | setStartDateTime(?string startDateTime): void |
| `stopDateTime` | `?string` | Optional | - | getStopDateTime(): ?string | setStopDateTime(?string stopDateTime): void |
| `totalEnergy` | `?float` | Optional | - | getTotalEnergy(): ?float | setTotalEnergy(?float totalEnergy): void |
| `totalTime` | `?float` | Optional | - | getTotalTime(): ?float | setTotalTime(?float totalTime): void |
| `totalCost` | [`?TotalCost`](../../doc/models/total-cost.md) | Optional | - | getTotalCost(): ?TotalCost | setTotalCost(?TotalCost totalCost): void |
| `location` | [`?Location`](../../doc/models/location.md) | Optional | - | getLocation(): ?Location | setLocation(?Location location): void |
| `chargingPeriods` | [`?(ChargingPeriod[])`](../../doc/models/charging-period.md) | Optional | - | getChargingPeriods(): ?array | setChargingPeriods(?array chargingPeriods): void |
| `tariffs` | [`?Tariffs`](../../doc/models/tariffs.md) | Optional | - | getTariffs(): ?Tariffs | setTariffs(?Tariffs tariffs): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "id": "id0",
  "vin": "vin6",
  "model": "model8",
  "start_date_time": "start_date_time6",
  "stop_date_time": "stop_date_time2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

