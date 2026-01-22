
# Vehicle Base

*This model accepts additional fields of type array.*

## Structure

`VehicleBase`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `id` | `?int` | Optional | - | getId(): ?int | setId(?int id): void |
| `vehicleId` | `?int` | Optional | - | getVehicleId(): ?int | setVehicleId(?int vehicleId): void |
| `vin` | `?string` | Optional | - | getVin(): ?string | setVin(?string vin): void |
| `displayName` | `?string` | Optional | - | getDisplayName(): ?string | setDisplayName(?string displayName): void |
| `accessType` | `?string` | Optional | - | getAccessType(): ?string | setAccessType(?string accessType): void |
| `state` | `?string` | Optional | - | getState(): ?string | setState(?string state): void |
| `inService` | `?bool` | Optional | - | getInService(): ?bool | setInService(?bool inService): void |
| `calendarEnabled` | `?bool` | Optional | - | getCalendarEnabled(): ?bool | setCalendarEnabled(?bool calendarEnabled): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "id": 126,
  "vehicle_id": 120,
  "vin": "vin8",
  "display_name": "display_name4",
  "access_type": "access_type0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

