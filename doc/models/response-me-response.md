
# Response Me Response

*This model accepts additional fields of type array.*

## Structure

`ResponseMeResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `email` | `string` | Required | - | getEmail(): string | setEmail(string email): void |
| `fullName` | `string` | Required | - | getFullName(): string | setFullName(string fullName): void |
| `profileImageUrl` | `string` | Required | - | getProfileImageUrl(): string | setProfileImageUrl(string profileImageUrl): void |
| `vaultUuid` | `string` | Required | - | getVaultUuid(): string | setVaultUuid(string vaultUuid): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "email": "email4",
  "full_name": "full_name8",
  "profile_image_url": "profile_image_url8",
  "vault_uuid": "000013ee-0000-0000-0000-000000000000",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

