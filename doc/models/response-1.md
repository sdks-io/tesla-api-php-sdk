
# Response 1

*This model accepts additional fields of type array.*

## Structure

`Response1`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `fleetTelemetryErrorVins` | `string[]` | Required | - | getFleetTelemetryErrorVins(): array | setFleetTelemetryErrorVins(array fleetTelemetryErrorVins): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "fleet_telemetry_error_vins": [
    "fleet_telemetry_error_vins1",
    "fleet_telemetry_error_vins2"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

