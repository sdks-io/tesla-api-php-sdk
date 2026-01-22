
# Live Status Response

*This model accepts additional fields of type array.*

## Structure

`LiveStatusResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `response` | [`ResponseLiveStatusResponse`](../../doc/models/response-live-status-response.md) | Required | - | getResponse(): ResponseLiveStatusResponse | setResponse(ResponseLiveStatusResponse response): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "response": {
    "solar_power": 9.5,
    "energy_left": 169.18,
    "total_pack_energy": 222.56,
    "percentage_charged": 213.42,
    "backup_capable": false,
    "battery_power": 112.84,
    "load_power": 150.1,
    "grid_status": "grid_status2",
    "grid_power": 60.64,
    "island_status": "island_status0",
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

