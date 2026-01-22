
# Response Region Response

*This model accepts additional fields of type array.*

## Structure

`ResponseRegionResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `region` | `string` | Required | - | getRegion(): string | setRegion(string region): void |
| `fleetApiBaseUrl` | `string` | Required | - | getFleetApiBaseUrl(): string | setFleetApiBaseUrl(string fleetApiBaseUrl): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "region": "region0",
  "fleet_api_base_url": "fleet_api_base_url8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

