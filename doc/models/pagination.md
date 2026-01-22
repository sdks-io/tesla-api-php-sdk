
# Pagination

*This model accepts additional fields of type array.*

## Structure

`Pagination`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `previous` | `?int` | Optional | - | getPrevious(): ?int | setPrevious(?int previous): void |
| `next` | `?int` | Optional | - | getNext(): ?int | setNext(?int next): void |
| `current` | `?int` | Optional | - | getCurrent(): ?int | setCurrent(?int current): void |
| `perPage` | `?int` | Optional | - | getPerPage(): ?int | setPerPage(?int perPage): void |
| `count` | `?int` | Optional | - | getCount(): ?int | setCount(?int count): void |
| `pages` | `?int` | Optional | - | getPages(): ?int | setPages(?int pages): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "previous": 176,
  "next": 10,
  "current": 16,
  "per_page": 92,
  "count": 210,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

