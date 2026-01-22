
# Fleet Telemetry Errors Response

*This model accepts additional fields of type array.*

## Structure

`FleetTelemetryErrorsResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `response` | [`ResponseFleetTelemetryErrorsResponse`](../../doc/models/response-fleet-telemetry-errors-response.md) | Required | - | getResponse(): ResponseFleetTelemetryErrorsResponse | setResponse(ResponseFleetTelemetryErrorsResponse response): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "response": {
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
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

