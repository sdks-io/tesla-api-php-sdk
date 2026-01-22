
# Price Component

*This model accepts additional fields of type array.*

## Structure

`PriceComponent`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `type` | `?string` | Optional | - | getType(): ?string | setType(?string type): void |
| `price` | `?float` | Optional | - | getPrice(): ?float | setPrice(?float price): void |
| `stepSize` | `?float` | Optional | - | getStepSize(): ?float | setStepSize(?float stepSize): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "type": "type2",
  "price": 87.54,
  "step_size": 214.68,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

