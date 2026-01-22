
# Response Charge History Response

*This model accepts additional fields of type array.*

## Structure

`ResponseChargeHistoryResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `chargeHistory` | [`ChargeHistory[]`](../../doc/models/charge-history.md) | Required | - | getChargeHistory(): array | setChargeHistory(array chargeHistory): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "charge_history": [
    {
      "charge_start_time": {
        "seconds": 206,
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "charge_duration": {
        "seconds": 62,
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "energy_added_wh": 56,
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

