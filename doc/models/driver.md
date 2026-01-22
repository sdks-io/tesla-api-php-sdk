
# Driver

*This model accepts additional fields of type array.*

## Structure

`Driver`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `myTeslaUniqueId` | `?int` | Optional | - | getMyTeslaUniqueId(): ?int | setMyTeslaUniqueId(?int myTeslaUniqueId): void |
| `userId` | `?int` | Optional | - | getUserId(): ?int | setUserId(?int userId): void |
| `userIdS` | `?string` | Optional | - | getUserIdS(): ?string | setUserIdS(?string userIdS): void |
| `vaultUuid` | `?string` | Optional | - | getVaultUuid(): ?string | setVaultUuid(?string vaultUuid): void |
| `driverFirstName` | `?string` | Optional | - | getDriverFirstName(): ?string | setDriverFirstName(?string driverFirstName): void |
| `driverLastName` | `?string` | Optional | - | getDriverLastName(): ?string | setDriverLastName(?string driverLastName): void |
| `granularAccess` | `?array` | Optional | - | getGranularAccess(): ?array | setGranularAccess(?array granularAccess): void |
| `activePubkeys` | `?(string[])` | Optional | - | getActivePubkeys(): ?array | setActivePubkeys(?array activePubkeys): void |
| `publicKey` | `?string` | Optional | - | getPublicKey(): ?string | setPublicKey(?string publicKey): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "my_tesla_unique_id": 40,
  "user_id": 64,
  "user_id_s": "user_id_s4",
  "vault_uuid": "vault_uuid0",
  "driver_first_name": "driver_first_name2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

