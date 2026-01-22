
# Fleet Telemetry Error

*This model accepts additional fields of type array.*

## Structure

`FleetTelemetryError`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `name` | `string` | Required | - | getName(): string | setName(string name): void |
| `error` | `string` | Required | - | getError(): string | setError(string error): void |
| `vin` | `string` | Required | - | getVin(): string | setVin(string vin): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "name": "name2",
  "error": "error6",
  "vin": "vin6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

