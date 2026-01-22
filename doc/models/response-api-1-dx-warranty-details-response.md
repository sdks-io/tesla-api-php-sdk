
# Response Api 1 Dx Warranty Details Response

*This model accepts additional fields of type array.*

## Structure

`ResponseApi1DxWarrantyDetailsResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `activeWarranty` | [`?(WarrantyItem[])`](../../doc/models/warranty-item.md) | Optional | - | getActiveWarranty(): ?array | setActiveWarranty(?array activeWarranty): void |
| `upcomingWarranty` | [`?(WarrantyItem[])`](../../doc/models/warranty-item.md) | Optional | - | getUpcomingWarranty(): ?array | setUpcomingWarranty(?array upcomingWarranty): void |
| `expiredWarranty` | [`?(WarrantyItem[])`](../../doc/models/warranty-item.md) | Optional | - | getExpiredWarranty(): ?array | setExpiredWarranty(?array expiredWarranty): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "activeWarranty": [
    {
      "warrantyType": "warrantyType4",
      "warrantyDisplayName": "warrantyDisplayName6",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 200,
      "odometerUnit": "odometerUnit0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "warrantyType": "warrantyType4",
      "warrantyDisplayName": "warrantyDisplayName6",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 200,
      "odometerUnit": "odometerUnit0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "warrantyType": "warrantyType4",
      "warrantyDisplayName": "warrantyDisplayName6",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 200,
      "odometerUnit": "odometerUnit0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "upcomingWarranty": [
    {
      "warrantyType": "warrantyType6",
      "warrantyDisplayName": "warrantyDisplayName8",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 236,
      "odometerUnit": "odometerUnit8",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "warrantyType": "warrantyType6",
      "warrantyDisplayName": "warrantyDisplayName8",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 236,
      "odometerUnit": "odometerUnit8",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "expiredWarranty": [
    {
      "warrantyType": "warrantyType0",
      "warrantyDisplayName": "warrantyDisplayName2",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 38,
      "odometerUnit": "odometerUnit6",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "warrantyType": "warrantyType0",
      "warrantyDisplayName": "warrantyDisplayName2",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 38,
      "odometerUnit": "odometerUnit6",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "warrantyType": "warrantyType0",
      "warrantyDisplayName": "warrantyDisplayName2",
      "expirationDate": "2016-03-13T12:52:32.123Z",
      "expirationOdometer": 38,
      "odometerUnit": "odometerUnit6",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

