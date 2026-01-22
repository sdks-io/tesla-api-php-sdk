
# Charging Fee

*This model accepts additional fields of type array.*

## Structure

`ChargingFee`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `sessionFeeId` | `?int` | Optional | - | getSessionFeeId(): ?int | setSessionFeeId(?int sessionFeeId): void |
| `feeType` | `?string` | Optional | - | getFeeType(): ?string | setFeeType(?string feeType): void |
| `currencyCode` | `?string` | Optional | - | getCurrencyCode(): ?string | setCurrencyCode(?string currencyCode): void |
| `pricingType` | `?string` | Optional | - | getPricingType(): ?string | setPricingType(?string pricingType): void |
| `rateBase` | `?float` | Optional | - | getRateBase(): ?float | setRateBase(?float rateBase): void |
| `rateTier1` | `?float` | Optional | - | getRateTier1(): ?float | setRateTier1(?float rateTier1): void |
| `rateTier2` | `?float` | Optional | - | getRateTier2(): ?float | setRateTier2(?float rateTier2): void |
| `rateTier3` | `?float` | Optional | - | getRateTier3(): ?float | setRateTier3(?float rateTier3): void |
| `rateTier4` | `?float` | Optional | - | getRateTier4(): ?float | setRateTier4(?float rateTier4): void |
| `usageBase` | `?float` | Optional | - | getUsageBase(): ?float | setUsageBase(?float usageBase): void |
| `usageTier1` | `?float` | Optional | - | getUsageTier1(): ?float | setUsageTier1(?float usageTier1): void |
| `usageTier2` | `?float` | Optional | - | getUsageTier2(): ?float | setUsageTier2(?float usageTier2): void |
| `usageTier3` | `?float` | Optional | - | getUsageTier3(): ?float | setUsageTier3(?float usageTier3): void |
| `usageTier4` | `?float` | Optional | - | getUsageTier4(): ?float | setUsageTier4(?float usageTier4): void |
| `totalBase` | `?float` | Optional | - | getTotalBase(): ?float | setTotalBase(?float totalBase): void |
| `totalTier1` | `?float` | Optional | - | getTotalTier1(): ?float | setTotalTier1(?float totalTier1): void |
| `totalTier2` | `?float` | Optional | - | getTotalTier2(): ?float | setTotalTier2(?float totalTier2): void |
| `totalTier3` | `?float` | Optional | - | getTotalTier3(): ?float | setTotalTier3(?float totalTier3): void |
| `totalTier4` | `?float` | Optional | - | getTotalTier4(): ?float | setTotalTier4(?float totalTier4): void |
| `totalDue` | `?float` | Optional | - | getTotalDue(): ?float | setTotalDue(?float totalDue): void |
| `netDue` | `?float` | Optional | - | getNetDue(): ?float | setNetDue(?float netDue): void |
| `uom` | `?string` | Optional | - | getUom(): ?string | setUom(?string uom): void |
| `isPaid` | `?bool` | Optional | - | getIsPaid(): ?bool | setIsPaid(?bool isPaid): void |
| `status` | `?string` | Optional | - | getStatus(): ?string | setStatus(?string status): void |
| `additionalProperties` | `array<string, array>` | Optional | - | findAdditionalProperty(string key): array | additionalProperty(string key, array value): void |

## Example (as JSON)

```json
{
  "sessionFeeId": 236,
  "feeType": "feeType4",
  "currencyCode": "currencyCode0",
  "pricingType": "pricingType6",
  "rateBase": 226.56,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

