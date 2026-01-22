
# Charging Sessions Data

*This model accepts additional fields of type array.*

## Structure

`ChargingSessionsData`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `data` | [`?(ChargingSession[])`](../../doc/models/charging-session.md) | Optional | - | getData(): ?array | setData(?array data): void |
| `statusCode` | `?int` | Optional | - | getStatusCode(): ?int | setStatusCode(?int statusCode): void |
| `statusMessage` | `?string` | Optional | - | getStatusMessage(): ?string | setStatusMessage(?string statusMessage): void |
| `timestamp` | `?array<string,string>` | Optional | - | getTimestamp(): ?array | setTimestamp(?array timestamp): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "data": [
    {
      "id": "id0",
      "vin": "vin4",
      "model": "model8",
      "start_date_time": "start_date_time6",
      "stop_date_time": "stop_date_time2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "id": "id0",
      "vin": "vin4",
      "model": "model8",
      "start_date_time": "start_date_time6",
      "stop_date_time": "stop_date_time2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "id": "id0",
      "vin": "vin4",
      "model": "model8",
      "start_date_time": "start_date_time6",
      "stop_date_time": "stop_date_time2",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "status_code": 188,
  "status_message": "status_message8",
  "timestamp": {
    "key0": "timestamp7",
    "key1": "timestamp8"
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

