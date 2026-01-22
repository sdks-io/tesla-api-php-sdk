
# Response Register Partner Response

*This model accepts additional fields of type array.*

## Structure

`ResponseRegisterPartnerResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `clientId` | `string` | Required | - | getClientId(): string | setClientId(string clientId): void |
| `name` | `string` | Required | - | getName(): string | setName(string name): void |
| `description` | `?string` | Optional | - | getDescription(): ?string | setDescription(?string description): void |
| `domain` | `string` | Required | - | getDomain(): string | setDomain(string domain): void |
| `ca` | `?string` | Optional | - | getCa(): ?string | setCa(?string ca): void |
| `createdAt` | `DateTime` | Required | - | getCreatedAt(): \DateTime | setCreatedAt(\DateTime createdAt): void |
| `updatedAt` | `DateTime` | Required | - | getUpdatedAt(): \DateTime | setUpdatedAt(\DateTime updatedAt): void |
| `enterpriseTier` | `string` | Required | - | getEnterpriseTier(): string | setEnterpriseTier(string enterpriseTier): void |
| `accountId` | `string` | Required | - | getAccountId(): string | setAccountId(string accountId): void |
| `issuer` | `?string` | Optional | - | getIssuer(): ?string | setIssuer(?string issuer): void |
| `csr` | `?string` | Optional | - | getCsr(): ?string | setCsr(?string csr): void |
| `csrUpdatedAt` | `?DateTime` | Optional | - | getCsrUpdatedAt(): ?\DateTime | setCsrUpdatedAt(?\DateTime csrUpdatedAt): void |
| `publicKey` | `string` | Required | - | getPublicKey(): string | setPublicKey(string publicKey): void |
| `publicKeyHash` | `string` | Required | - | getPublicKeyHash(): string | setPublicKeyHash(string publicKeyHash): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "client_id": "client_id6",
  "name": "name4",
  "description": "description4",
  "domain": "domain0",
  "ca": "ca8",
  "created_at": "2016-03-13T12:52:32.123Z",
  "updated_at": "2016-03-13T12:52:32.123Z",
  "enterprise_tier": "enterprise_tier8",
  "account_id": "account_id6",
  "issuer": "issuer4",
  "csr": "csr6",
  "csr_updated_at": "2016-03-13T12:52:32.123Z",
  "public_key": "public_key2",
  "public_key_hash": "public_key_hash2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

