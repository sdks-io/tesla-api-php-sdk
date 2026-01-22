
# Charging Location

*This model accepts additional fields of type array.*

## Structure

`ChargingLocation`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `name` | `?string` | Optional | - | getName(): ?string | setName(?string name): void |
| `type` | `?string` | Optional | - | getType(): ?string | setType(?string type): void |
| `distanceMiles` | `?float` | Optional | - | getDistanceMiles(): ?float | setDistanceMiles(?float distanceMiles): void |
| `amenities` | `?string` | Optional | - | getAmenities(): ?string | setAmenities(?string amenities): void |
| `availableStalls` | `?int` | Optional | - | getAvailableStalls(): ?int | setAvailableStalls(?int availableStalls): void |
| `totalStalls` | `?int` | Optional | - | getTotalStalls(): ?int | setTotalStalls(?int totalStalls): void |
| `siteClosed` | `?bool` | Optional | - | getSiteClosed(): ?bool | setSiteClosed(?bool siteClosed): void |
| `billingInfo` | `?string` | Optional | - | getBillingInfo(): ?string | setBillingInfo(?string billingInfo): void |
| `location` | [`?Location1`](../../doc/models/location-1.md) | Optional | - | getLocation(): ?Location1 | setLocation(?Location1 location): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "name": "name0",
  "type": "type0",
  "distance_miles": 123.84,
  "amenities": "amenities0",
  "available_stalls": 60,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

