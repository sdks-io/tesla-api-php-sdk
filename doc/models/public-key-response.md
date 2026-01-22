
# Public Key Response

*This model accepts additional fields of type array.*

## Structure

`PublicKeyResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `response` | [`ResponsePublicKeyResponse`](../../doc/models/response-public-key-response.md) | Required | - | getResponse(): ResponsePublicKeyResponse | setResponse(ResponsePublicKeyResponse response): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "response": {
    "public_key": "public_key6",
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

