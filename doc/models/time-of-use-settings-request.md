
# Time of Use Settings Request

*This model accepts additional fields of type array.*

## Structure

`TimeOfUseSettingsRequest`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `touSettings` | [`TouSettings`](../../doc/models/tou-settings.md) | Required | - | getTouSettings(): TouSettings | setTouSettings(TouSettings touSettings): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "tou_settings": {
    "tariff_content_v2": {
      "key1": "val1",
      "key2": "val2"
    },
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

