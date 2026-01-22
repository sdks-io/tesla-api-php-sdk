
# Response Calendar History Response

*This model accepts additional fields of type array.*

## Structure

`ResponseCalendarHistoryResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `events` | [`Event[]`](../../doc/models/event.md) | Required | - | getEvents(): array | setEvents(array events): void |
| `totalEvents` | `int` | Required | - | getTotalEvents(): int | setTotalEvents(int totalEvents): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
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
  "total_events": 12,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

