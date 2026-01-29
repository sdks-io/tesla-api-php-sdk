# Partner

Partner account and telemetry endpoints

```php
$partnerController = $client->getPartnerController();
```

## Class Name

`PartnerController`

## Methods

* [Get Vins With Fleet Telemetry Errors](../../doc/controllers/partner.md#get-vins-with-fleet-telemetry-errors)
* [Get Recent Fleet Telemetry Errors](../../doc/controllers/partner.md#get-recent-fleet-telemetry-errors)
* [Get Public Key for a Domain](../../doc/controllers/partner.md#get-public-key-for-a-domain)
* [Register a Partner Account](../../doc/controllers/partner.md#register-a-partner-account)


# Get Vins With Fleet Telemetry Errors

```php
function getVinsWithFleetTelemetryErrors(): ApiResponse
```

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`BackupResponse`](../../doc/models/backup-response.md).

## Example Usage

```php
$apiResponse = $partnerController->getVinsWithFleetTelemetryErrors();
```


# Get Recent Fleet Telemetry Errors

```php
function getRecentFleetTelemetryErrors(): ApiResponse
```

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`FleetTelemetryErrorsResponse`](../../doc/models/fleet-telemetry-errors-response.md).

## Example Usage

```php
$apiResponse = $partnerController->getRecentFleetTelemetryErrors();
```


# Get Public Key for a Domain

```php
function getPublicKeyForADomain(string $domain): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `domain` | `string` | Query, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`PublicKeyResponse`](../../doc/models/public-key-response.md).

## Example Usage

```php
$domain = 'domain6';

$apiResponse = $partnerController->getPublicKeyForADomain($domain);
```


# Register a Partner Account

```php
function registerAPartnerAccount(RegisterPartnerRequest $body): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`RegisterPartnerRequest`](../../doc/models/register-partner-request.md) | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`RegisterPartnerResponse`](../../doc/models/register-partner-response.md).

## Example Usage

```php
$body = RegisterPartnerRequestBuilder::init(
    'domain.com'
)->build();

$apiResponse = $partnerController->registerAPartnerAccount($body);
```

