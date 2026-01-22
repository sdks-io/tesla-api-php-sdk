
# Response 2

*This model accepts additional fields of type array.*

## Structure

`Response2`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `signaling` | [`Signaling`](../../doc/models/signaling.md) | Required | - | getSignaling(): Signaling | setSignaling(Signaling signaling): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "signaling": {
    "enabled": false,
    "subscribe_connectivity": false,
    "use_auth_token": false,
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

