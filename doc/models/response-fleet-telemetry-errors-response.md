
# Response Fleet Telemetry Errors Response

*This model accepts additional fields of type array.*

## Structure

`ResponseFleetTelemetryErrorsResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `fleetTelemetryErrors` | [`FleetTelemetryError[]`](../../doc/models/fleet-telemetry-error.md) | Required | - | getFleetTelemetryErrors(): array | setFleetTelemetryErrors(array fleetTelemetryErrors): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "fleet_telemetry_errors": [
    {
      "name": "name8",
      "error": "error2",
      "vin": "vin8",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

