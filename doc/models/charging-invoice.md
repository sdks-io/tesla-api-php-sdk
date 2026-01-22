
# Charging Invoice

*This model accepts additional fields of type array.*

## Structure

`ChargingInvoice`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `fileName` | `?string` | Optional | - | getFileName(): ?string | setFileName(?string fileName): void |
| `contentId` | `?string` | Optional | - | getContentId(): ?string | setContentId(?string contentId): void |
| `invoiceType` | `?string` | Optional | - | getInvoiceType(): ?string | setInvoiceType(?string invoiceType): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "fileName": "fileName0",
  "contentId": "contentId0",
  "invoiceType": "invoiceType0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

