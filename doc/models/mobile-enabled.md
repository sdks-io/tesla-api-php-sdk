
# Mobile Enabled

*This model accepts additional fields of type array.*

## Structure

`MobileEnabled`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `result` | `?bool` | Optional | - | getResult(): ?bool | setResult(?bool result): void |
| `reason` | `?string` | Optional | - | getReason(): ?string | setReason(?string reason): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "result": false,
  "reason": "reason2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

