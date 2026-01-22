
# Tariff Element

*This model accepts additional fields of type array.*

## Structure

`TariffElement`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `priceComponents` | [`?(PriceComponent[])`](../../doc/models/price-component.md) | Optional | - | getPriceComponents(): ?array | setPriceComponents(?array priceComponents): void |
| `restrictions` | `?array` | Optional | - | getRestrictions(): ?array | setRestrictions(?array restrictions): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "price_components": [
    {
      "type": "type2",
      "price": 107.9,
      "step_size": 154.12,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "type": "type2",
      "price": 107.9,
      "step_size": 154.12,
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "restrictions": {
    "key0": {
      "key1": "val1",
      "key2": "val2"
    },
    "key1": {
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

