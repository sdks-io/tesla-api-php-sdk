
# Actuate Trunk Request

*This model accepts additional fields of type array.*

## Structure

`ActuateTrunkRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `whichTrunk` | [`string(WhichTrunk)`](../../doc/models/which-trunk.md) | Required | - | getWhichTrunk(): string | setWhichTrunk(string whichTrunk): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "which_trunk": "front",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

