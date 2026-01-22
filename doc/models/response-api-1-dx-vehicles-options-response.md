
# Response Api 1 Dx Vehicles Options Response

*This model accepts additional fields of type array.*

## Structure

`ResponseApi1DxVehiclesOptionsResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `codes` | [`?(VehicleOption[])`](../../doc/models/vehicle-option.md) | Optional | - | getCodes(): ?array | setCodes(?array codes): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
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
    },
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
}
```

