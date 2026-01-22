
# Api 1 Dx Vehicles Options Response

*This model accepts additional fields of type array.*

## Structure

`Api1DxVehiclesOptionsResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `response` | [`?ResponseApi1DxVehiclesOptionsResponse`](../../doc/models/response-api-1-dx-vehicles-options-response.md) | Optional | - | getResponse(): ?ResponseApi1DxVehiclesOptionsResponse | setResponse(?ResponseApi1DxVehiclesOptionsResponse response): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "response": {
    "codes": [
      {
        "code": "code0",
        "displayName": "displayName0",
        "colorCode": "colorCode2",
        "isActive": false,
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

