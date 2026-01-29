# User

User account and settings endpoints

```php
$userController = $client->getUserController();
```

## Class Name

`UserController`

## Methods

* [Get Custom Feature Flags for a User](../../doc/controllers/user.md#get-custom-feature-flags-for-a-user)
* [Get Summary of a User S Account](../../doc/controllers/user.md#get-summary-of-a-user-s-account)
* [Get Active Orders for a User](../../doc/controllers/user.md#get-active-orders-for-a-user)
* [Get User S Region and Fleet Api Base Url](../../doc/controllers/user.md#get-user-s-region-and-fleet-api-base-url)


# Get Custom Feature Flags for a User

```php
function getCustomFeatureFlagsForAUser(): ApiResponse
```

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`BackupResponse`](../../doc/models/backup-response.md).

## Example Usage

```php
$apiResponse = $userController->getCustomFeatureFlagsForAUser();
```


# Get Summary of a User S Account

```php
function getSummaryOfAUserSAccount(): ApiResponse
```

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`MeResponse`](../../doc/models/me-response.md).

## Example Usage

```php
$apiResponse = $userController->getSummaryOfAUserSAccount();
```


# Get Active Orders for a User

```php
function getActiveOrdersForAUser(): ApiResponse
```

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`OrdersResponse`](../../doc/models/orders-response.md).

## Example Usage

```php
$apiResponse = $userController->getActiveOrdersForAUser();
```


# Get User S Region and Fleet Api Base Url

```php
function getUserSRegionAndFleetApiBaseUrl(): ApiResponse
```

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`RegionResponse`](../../doc/models/region-response.md).

## Example Usage

```php
$apiResponse = $userController->getUserSRegionAndFleetApiBaseUrl();
```

