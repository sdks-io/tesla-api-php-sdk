
# Response Public Key Response

*This model accepts additional fields of type array.*

## Structure

`ResponsePublicKeyResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `publicKey` | `string` | Required | - | getPublicKey(): string | setPublicKey(string publicKey): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "public_key": "public_key0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

