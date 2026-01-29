# Vehicles

```php
$vehiclesController = $client->getVehiclesController();
```

## Class Name

`VehiclesController`

## Methods

* [List Vehicles](../../doc/controllers/vehicles.md#list-vehicles)
* [Get Vehicle](../../doc/controllers/vehicles.md#get-vehicle)
* [Mobile Enabled](../../doc/controllers/vehicles.md#mobile-enabled)
* [Nearby Charging Sites](../../doc/controllers/vehicles.md#nearby-charging-sites)
* [Vehicle Live Data](../../doc/controllers/vehicles.md#vehicle-live-data)
* [Wake up Vehicle](../../doc/controllers/vehicles.md#wake-up-vehicle)
* [Vehicle Specs](../../doc/controllers/vehicles.md#vehicle-specs)
* [Vehicle Options](../../doc/controllers/vehicles.md#vehicle-options)
* [Warranty Details](../../doc/controllers/vehicles.md#warranty-details)
* [Get Allowed Drivers for a Vehicle](../../doc/controllers/vehicles.md#get-allowed-drivers-for-a-vehicle)
* [Remove Driver Access From a Vehicle](../../doc/controllers/vehicles.md#remove-driver-access-from-a-vehicle)
* [Get Eligible Vehicle Subscriptions](../../doc/controllers/vehicles.md#get-eligible-vehicle-subscriptions)
* [Get Eligible Vehicle Upgrades](../../doc/controllers/vehicles.md#get-eligible-vehicle-upgrades)
* [Set Enterprise Payer Roles](../../doc/controllers/vehicles.md#set-enterprise-payer-roles)
* [Get Enterprise Roles for a Vehicle](../../doc/controllers/vehicles.md#get-enterprise-roles-for-a-vehicle)
* [Get Fleet Status for Vehicles](../../doc/controllers/vehicles.md#get-fleet-status-for-vehicles)
* [Create or Update Fleet Telemetry Configuration](../../doc/controllers/vehicles.md#create-or-update-fleet-telemetry-configuration)
* [Get Fleet Telemetry Configuration](../../doc/controllers/vehicles.md#get-fleet-telemetry-configuration)
* [Delete Fleet Telemetry Configuration](../../doc/controllers/vehicles.md#delete-fleet-telemetry-configuration)
* [Configure Fleet Telemetry Using Signed Jws Token](../../doc/controllers/vehicles.md#configure-fleet-telemetry-using-signed-jws-token)
* [Get Fleet Telemetry Errors for a Vehicle](../../doc/controllers/vehicles.md#get-fleet-telemetry-errors-for-a-vehicle)


# List Vehicles

```php
function listVehicles(): ApiResponse
```

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`Api1VehiclesResponse`](../../doc/models/api-1-vehicles-response.md).

## Example Usage

```php
$apiResponse = $vehiclesController->listVehicles();
```


# Get Vehicle

```php
function getVehicle(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`Api1VehiclesResponseGetVehicle`](../../doc/models/api-1-vehicles-response-get-vehicle.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$apiResponse = $vehiclesController->getVehicle($vehicleTag);
```


# Mobile Enabled

```php
function mobileEnabled(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`Api1VehiclesMobileEnabledResponse`](../../doc/models/api-1-vehicles-mobile-enabled-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$apiResponse = $vehiclesController->mobileEnabled($vehicleTag);
```


# Nearby Charging Sites

```php
function nearbyChargingSites(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`Api1VehiclesNearbyChargingSitesResponse`](../../doc/models/api-1-vehicles-nearby-charging-sites-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$apiResponse = $vehiclesController->nearbyChargingSites($vehicleTag);
```


# Vehicle Live Data

```php
function vehicleLiveData(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`SiteInfoResponse`](../../doc/models/site-info-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$apiResponse = $vehiclesController->vehicleLiveData($vehicleTag);
```


# Wake up Vehicle

```php
function wakeUpVehicle(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`Api1VehiclesWakeUpResponse`](../../doc/models/api-1-vehicles-wake-up-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$apiResponse = $vehiclesController->wakeUpVehicle($vehicleTag);
```


# Vehicle Specs

```php
function vehicleSpecs(string $vin): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`SiteInfoResponse`](../../doc/models/site-info-response.md).

## Example Usage

```php
$vin = 'vin6';

$apiResponse = $vehiclesController->vehicleSpecs($vin);
```


# Vehicle Options

```php
function vehicleOptions(string $vin): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Query, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`Api1DxVehiclesOptionsResponse`](../../doc/models/api-1-dx-vehicles-options-response.md).

## Example Usage

```php
$vin = 'vin6';

$apiResponse = $vehiclesController->vehicleOptions($vin);
```


# Warranty Details

```php
function warrantyDetails(): ApiResponse
```

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`Api1DxWarrantyDetailsResponse`](../../doc/models/api-1-dx-warranty-details-response.md).

## Example Usage

```php
$apiResponse = $vehiclesController->warrantyDetails();
```


# Get Allowed Drivers for a Vehicle

```php
function getAllowedDriversForAVehicle(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`DriversResponse`](../../doc/models/drivers-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$apiResponse = $vehiclesController->getAllowedDriversForAVehicle($vehicleTag);
```


# Remove Driver Access From a Vehicle

```php
function removeDriverAccessFromAVehicle(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`SimpleOkResponse`](../../doc/models/simple-ok-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$apiResponse = $vehiclesController->removeDriverAccessFromAVehicle($vehicleTag);
```


# Get Eligible Vehicle Subscriptions

```php
function getEligibleVehicleSubscriptions(string $vin): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Query, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`SiteInfoResponse`](../../doc/models/site-info-response.md).

## Example Usage

```php
$vin = 'vin6';

$apiResponse = $vehiclesController->getEligibleVehicleSubscriptions($vin);
```


# Get Eligible Vehicle Upgrades

```php
function getEligibleVehicleUpgrades(string $vin): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Query, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`SiteInfoResponse`](../../doc/models/site-info-response.md).

## Example Usage

```php
$vin = 'vin6';

$apiResponse = $vehiclesController->getEligibleVehicleUpgrades($vin);
```


# Set Enterprise Payer Roles

```php
function setEnterprisePayerRoles(string $vin, EnterprisePayerRequest $body): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Template, Required | - |
| `body` | [`EnterprisePayerRequest`](../../doc/models/enterprise-payer-request.md) | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```php
$vin = 'vin6';

$body = EnterprisePayerRequestBuilder::init(
    'role0'
)->build();

$apiResponse = $vehiclesController->setEnterprisePayerRoles(
    $vin,
    $body
);
```


# Get Enterprise Roles for a Vehicle

```php
function getEnterpriseRolesForAVehicle(string $vin): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vin` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type `array`.

## Example Usage

```php
$vin = 'vin6';

$apiResponse = $vehiclesController->getEnterpriseRolesForAVehicle($vin);
```


# Get Fleet Status for Vehicles

```php
function getFleetStatusForVehicles(FleetStatusRequest $body): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`FleetStatusRequest`](../../doc/models/fleet-status-request.md) | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type `array`.

## Example Usage

```php
$body = FleetStatusRequestBuilder::init()->build();

$apiResponse = $vehiclesController->getFleetStatusForVehicles($body);
```


# Create or Update Fleet Telemetry Configuration

```php
function createOrUpdateFleetTelemetryConfiguration(array $body): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | `array` | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type `array`.

## Example Usage

```php
$body = ApiHelper::deserialize('{"key1":"val1","key2":"val2"}');

$apiResponse = $vehiclesController->createOrUpdateFleetTelemetryConfiguration($body);
```


# Get Fleet Telemetry Configuration

```php
function getFleetTelemetryConfiguration(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type `array`.

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$apiResponse = $vehiclesController->getFleetTelemetryConfiguration($vehicleTag);
```


# Delete Fleet Telemetry Configuration

```php
function deleteFleetTelemetryConfiguration(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type `array`.

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$apiResponse = $vehiclesController->deleteFleetTelemetryConfiguration($vehicleTag);
```


# Configure Fleet Telemetry Using Signed Jws Token

```php
function configureFleetTelemetryUsingSignedJwsToken(FleetTelemetryJwsRequest $body): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`FleetTelemetryJwsRequest`](../../doc/models/fleet-telemetry-jws-request.md) | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type `array`.

## Example Usage

```php
$body = FleetTelemetryJwsRequestBuilder::init()->build();

$apiResponse = $vehiclesController->configureFleetTelemetryUsingSignedJwsToken($body);
```


# Get Fleet Telemetry Errors for a Vehicle

```php
function getFleetTelemetryErrorsForAVehicle(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type `array`.

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$apiResponse = $vehiclesController->getFleetTelemetryErrorsForAVehicle($vehicleTag);
```

