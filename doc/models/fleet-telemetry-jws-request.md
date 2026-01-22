
# Fleet Telemetry Jws Request

*This model accepts additional fields of type array.*

## Structure

`FleetTelemetryJwsRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `token` | `?string` | Optional | - | getToken(): ?string | setToken(?string token): void |
| `vins` | `?(string[])` | Optional | - | getVins(): ?array | setVins(?array vins): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "token": "token8",
  "vins": [
    "vins0",
    "vins9",
    "vins8"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

