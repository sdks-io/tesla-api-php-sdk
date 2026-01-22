
# Backup Request

*This model accepts additional fields of type array.*

## Structure

`BackupRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `backupReservePercent` | `int` | Required | - | getBackupReservePercent(): int | setBackupReservePercent(int backupReservePercent): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "backup_reserve_percent": 32,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

