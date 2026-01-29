
# Command Response

*This model accepts additional fields of type array.*

## Structure

`CommandResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `response` | [`?CommandResult`](../../doc/models/command-result.md) | Optional | - | getResponse(): ?CommandResult | setResponse(?CommandResult response): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "response": {
    "result": false,
    "reason": "reason4",
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

