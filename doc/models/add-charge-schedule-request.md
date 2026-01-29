
# Add Charge Schedule Request

*This model accepts additional fields of type array.*

## Structure

`AddChargeScheduleRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `lat` | `float` | Required | - | getLat(): float | setLat(float lat): void |
| `lon` | `float` | Required | - | getLon(): float | setLon(float lon): void |
| `id` | `int` | Required | - | getId(): int | setId(int id): void |
| `daysOfWeek` | `?string` | Optional | - | getDaysOfWeek(): ?string | setDaysOfWeek(?string daysOfWeek): void |
| `startEnabled` | `?bool` | Optional | - | getStartEnabled(): ?bool | setStartEnabled(?bool startEnabled): void |
| `startTime` | `?int` | Optional | - | getStartTime(): ?int | setStartTime(?int startTime): void |
| `endEnabled` | `?bool` | Optional | - | getEndEnabled(): ?bool | setEndEnabled(?bool endEnabled): void |
| `endTime` | `?int` | Optional | - | getEndTime(): ?int | setEndTime(?int endTime): void |
| `oneTime` | `?bool` | Optional | - | getOneTime(): ?bool | setOneTime(?bool oneTime): void |
| `enabled` | `bool` | Required | - | getEnabled(): bool | setEnabled(bool enabled): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "lat": 196.62,
  "lon": 29.72,
  "id": 190,
  "days_of_week": "days_of_week8",
  "start_enabled": false,
  "start_time": 214,
  "end_enabled": false,
  "end_time": 174,
  "enabled": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

