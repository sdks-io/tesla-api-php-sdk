
# Add Precondition Schedule Request

*This model accepts additional fields of type array.*

## Structure

`AddPreconditionScheduleRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `lat` | `float` | Required | - | getLat(): float | setLat(float lat): void |
| `lon` | `float` | Required | - | getLon(): float | setLon(float lon): void |
| `id` | `int` | Required | - | getId(): int | setId(int id): void |
| `daysOfWeek` | `?string` | Optional | - | getDaysOfWeek(): ?string | setDaysOfWeek(?string daysOfWeek): void |
| `preconditionTime` | `?int` | Optional | - | getPreconditionTime(): ?int | setPreconditionTime(?int preconditionTime): void |
| `oneTime` | `?bool` | Optional | - | getOneTime(): ?bool | setOneTime(?bool oneTime): void |
| `enabled` | `bool` | Required | - | getEnabled(): bool | setEnabled(bool enabled): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "lat": 87.82,
  "lon": 176.92,
  "id": 62,
  "days_of_week": "days_of_week8",
  "precondition_time": 70,
  "one_time": false,
  "enabled": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

