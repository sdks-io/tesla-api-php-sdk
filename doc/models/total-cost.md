
# Total Cost

*This model accepts additional fields of type array.*

## Structure

`TotalCost`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `exclVat` | `?float` | Optional | - | getExclVat(): ?float | setExclVat(?float exclVat): void |
| `inclVat` | `?float` | Optional | - | getInclVat(): ?float | setInclVat(?float inclVat): void |
| `vat` | `?float` | Optional | - | getVat(): ?float | setVat(?float vat): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "excl_vat": 13.82,
  "incl_vat": 65.46,
  "vat": 170.96,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

