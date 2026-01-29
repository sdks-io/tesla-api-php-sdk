
# Command Result

*This model accepts additional fields of type array.*

## Structure

`CommandResult`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `result` | `bool` | Required | - | getResult(): bool | setResult(bool result): void |
| `reason` | `string` | Required | - | getReason(): string | setReason(string reason): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "result": false,
  "reason": "reason0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

