
# Drivers Response

*This model accepts additional fields of type array.*

## Structure

`DriversResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `response` | [`?(Driver[])`](../../doc/models/driver.md) | Optional | - | getResponse(): ?array | setResponse(?array response): void |
| `count` | `?int` | Optional | - | getCount(): ?int | setCount(?int count): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "response": [
    {
      "my_tesla_unique_id": 234,
      "user_id": 46,
      "user_id_s": "user_id_s8",
      "vault_uuid": "vault_uuid4",
      "driver_first_name": "driver_first_name6",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "my_tesla_unique_id": 234,
      "user_id": 46,
      "user_id_s": "user_id_s8",
      "vault_uuid": "vault_uuid4",
      "driver_first_name": "driver_first_name6",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "count": 124,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

