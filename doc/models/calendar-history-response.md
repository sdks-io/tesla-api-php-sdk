
# Calendar History Response

*This model accepts additional fields of type array.*

## Structure

`CalendarHistoryResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `response` | [`ResponseCalendarHistoryResponse`](../../doc/models/response-calendar-history-response.md) | Required | - | getResponse(): ResponseCalendarHistoryResponse | setResponse(ResponseCalendarHistoryResponse response): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "response": {
    "events": [
      {
        "timestamp": "2016-03-13T12:52:32.123Z",
        "duration": 68,
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      }
    ],
    "total_events": 236,
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

