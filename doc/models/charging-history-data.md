
# Charging History Data

*This model accepts additional fields of type array.*

## Structure

`ChargingHistoryData`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `data` | [`ChargingHistoryItem[]`](../../doc/models/charging-history-item.md) | Required | - | getData(): array | setData(array data): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "data": [
    {
      "sessionId": 186,
      "vin": "vin4",
      "siteLocationName": "siteLocationName6",
      "chargeStartDateTime": "2016-03-13T12:52:32.123Z",
      "chargeStopDateTime": "2016-03-13T12:52:32.123Z",
      "unlatchDateTime": "2016-03-13T12:52:32.123Z",
      "countryCode": "countryCode6",
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

