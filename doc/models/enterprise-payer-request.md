
# Enterprise Payer Request

*This model accepts additional fields of type array.*

## Structure

`EnterprisePayerRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `role` | `string` | Required | - | getRole(): string | setRole(string role): void |
| `federationId` | `?string` | Optional | - | getFederationId(): ?string | setFederationId(?string federationId): void |
| `accountId` | `?string` | Optional | - | getAccountId(): ?string | setAccountId(?string accountId): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "role": "role0",
  "federation_id": "federation_id0",
  "account_id": "account_id8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

