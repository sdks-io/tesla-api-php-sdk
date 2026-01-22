
# Signaling

*This model accepts additional fields of type array.*

## Structure

`Signaling`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `enabled` | `bool` | Required | - | getEnabled(): bool | setEnabled(bool enabled): void |
| `subscribeConnectivity` | `bool` | Required | - | getSubscribeConnectivity(): bool | setSubscribeConnectivity(bool subscribeConnectivity): void |
| `useAuthToken` | `bool` | Required | - | getUseAuthToken(): bool | setUseAuthToken(bool useAuthToken): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "enabled": false,
  "subscribe_connectivity": false,
  "use_auth_token": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

