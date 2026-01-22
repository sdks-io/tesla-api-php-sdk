
# Region Response

*This model accepts additional fields of type array.*

## Structure

`RegionResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `response` | [`ResponseRegionResponse`](../../doc/models/response-region-response.md) | Required | - | getResponse(): ResponseRegionResponse | setResponse(ResponseRegionResponse response): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "response": {
    "region": "region6",
    "fleet_api_base_url": "fleet_api_base_url4",
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

