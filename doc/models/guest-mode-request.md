
# Guest Mode Request

*This model accepts additional fields of type array.*

## Structure

`GuestModeRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `enable` | `bool` | Required | Enable or disable Guest Mode | getEnable(): bool | setEnable(bool enable): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "enable": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

