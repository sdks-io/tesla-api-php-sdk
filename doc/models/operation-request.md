
# Operation Request

*This model accepts additional fields of type array.*

## Structure

`OperationRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `defaultRealMode` | [`string(DefaultRealMode)`](../../doc/models/default-real-mode.md) | Required | - | getDefaultRealMode(): string | setDefaultRealMode(string defaultRealMode): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "default_real_mode": "autonomous",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

