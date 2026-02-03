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
$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->listVehicles();

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'Api1VehiclesResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->getVehicle($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'Api1VehiclesResponseGetVehicle:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->mobileEnabled($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'Api1VehiclesMobileEnabledResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->nearbyChargingSites($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'Api1VehiclesNearbyChargingSitesResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->vehicleLiveData($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'SiteInfoResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->wakeUpVehicle($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'Api1VehiclesWakeUpResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->vehicleSpecs($vin);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'SiteInfoResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->vehicleOptions($vin);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'Api1DxVehiclesOptionsResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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
$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->warrantyDetails();

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'Api1DxWarrantyDetailsResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->getAllowedDriversForAVehicle($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'DriversResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->removeDriverAccessFromAVehicle($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'SimpleOkResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->getEligibleVehicleSubscriptions($vin);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'SiteInfoResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->getEligibleVehicleUpgrades($vin);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'SiteInfoResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->setEnterprisePayerRoles(
    $vin,
    $body
);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'void:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->getEnterpriseRolesForAVehicle($vin);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'array:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->getFleetStatusForVehicles($body);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'array:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->createOrUpdateFleetTelemetryConfiguration($body);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'array:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->getFleetTelemetryConfiguration($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'array:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->deleteFleetTelemetryConfiguration($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'array:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->configureFleetTelemetryUsingSignedJwsToken($body);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'array:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
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

$vehiclesController = $client->getVehiclesController();
$apiResponse = $vehiclesController->getFleetTelemetryErrorsForAVehicle($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'array:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```

