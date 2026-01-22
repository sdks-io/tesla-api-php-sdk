
# Api 1 Dx Warranty Details Response

*This model accepts additional fields of type array.*

## Structure

`Api1DxWarrantyDetailsResponse`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `response` | [`?ResponseApi1DxWarrantyDetailsResponse`](../../doc/models/response-api-1-dx-warranty-details-response.md) | Optional | - | getResponse(): ?ResponseApi1DxWarrantyDetailsResponse | setResponse(?ResponseApi1DxWarrantyDetailsResponse response): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "response": {
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
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

