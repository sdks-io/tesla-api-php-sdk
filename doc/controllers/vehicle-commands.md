# Vehicle Commands

```php
$vehicleCommandsController = $client->getVehicleCommandsController();
```

## Class Name

`VehicleCommandsController`

## Methods

* [Actuate Trunk](../../doc/controllers/vehicle-commands.md#actuate-trunk)
* [Add Charge Schedule](../../doc/controllers/vehicle-commands.md#add-charge-schedule)
* [Add Precondition Schedule](../../doc/controllers/vehicle-commands.md#add-precondition-schedule)
* [Adjust Media Volume](../../doc/controllers/vehicle-commands.md#adjust-media-volume)
* [Start Climate Preconditioning](../../doc/controllers/vehicle-commands.md#start-climate-preconditioning)
* [Stop Climate Preconditioning](../../doc/controllers/vehicle-commands.md#stop-climate-preconditioning)
* [Cancel Software Update](../../doc/controllers/vehicle-commands.md#cancel-software-update)
* [Charge Max Range](../../doc/controllers/vehicle-commands.md#charge-max-range)
* [Open Charge Port Door](../../doc/controllers/vehicle-commands.md#open-charge-port-door)
* [Close Charge Port Door](../../doc/controllers/vehicle-commands.md#close-charge-port-door)
* [Charge Standard](../../doc/controllers/vehicle-commands.md#charge-standard)
* [Start Charging](../../doc/controllers/vehicle-commands.md#start-charging)
* [Stop Charging](../../doc/controllers/vehicle-commands.md#stop-charging)
* [Clear PIN to Drive Admin](../../doc/controllers/vehicle-commands.md#clear-pin-to-drive-admin)
* [Lock Doors](../../doc/controllers/vehicle-commands.md#lock-doors)
* [Unlock Doors](../../doc/controllers/vehicle-commands.md#unlock-doors)
* [Erase User Data](../../doc/controllers/vehicle-commands.md#erase-user-data)
* [Flash Lights](../../doc/controllers/vehicle-commands.md#flash-lights)
* [Enable or Disable Guest Mode](../../doc/controllers/vehicle-commands.md#enable-or-disable-guest-mode)
* [Honk Horn](../../doc/controllers/vehicle-commands.md#honk-horn)
* [Next Favorite Media Track](../../doc/controllers/vehicle-commands.md#next-favorite-media-track)


# Actuate Trunk

Controls the front or rear trunk

```php
function actuateTrunk(string $vehicleTag, ActuateTrunkRequest $body): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `body` | [`ActuateTrunkRequest`](../../doc/models/actuate-trunk-request.md) | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$body = ActuateTrunkRequestBuilder::init(
    WhichTrunk::FRONT
)->build();

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->actuateTrunk(
    $vehicleTag,
    $body
);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Add Charge Schedule

```php
function addChargeSchedule(string $vehicleTag, AddChargeScheduleRequest $body): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `body` | [`AddChargeScheduleRequest`](../../doc/models/add-charge-schedule-request.md) | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$body = AddChargeScheduleRequestBuilder::init(
    213.84,
    209.06,
    120,
    false
)->build();

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->addChargeSchedule(
    $vehicleTag,
    $body
);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Add Precondition Schedule

```php
function addPreconditionSchedule(string $vehicleTag, AddPreconditionScheduleRequest $body): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `body` | [`AddPreconditionScheduleRequest`](../../doc/models/add-precondition-schedule-request.md) | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$body = AddPreconditionScheduleRequestBuilder::init(
    213.84,
    209.06,
    120,
    false
)->build();

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->addPreconditionSchedule(
    $vehicleTag,
    $body
);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Adjust Media Volume

```php
function adjustMediaVolume(string $vehicleTag, AdjustVolumeRequest $body): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `body` | [`AdjustVolumeRequest`](../../doc/models/adjust-volume-request.md) | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$body = AdjustVolumeRequestBuilder::init(
    74
)->build();

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->adjustMediaVolume(
    $vehicleTag,
    $body
);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Start Climate Preconditioning

```php
function startClimatePreconditioning(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->startClimatePreconditioning($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Stop Climate Preconditioning

```php
function stopClimatePreconditioning(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->stopClimatePreconditioning($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Cancel Software Update

```php
function cancelSoftwareUpdate(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->cancelSoftwareUpdate($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Charge Max Range

```php
function chargeMaxRange(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->chargeMaxRange($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Open Charge Port Door

```php
function openChargePortDoor(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->openChargePortDoor($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Close Charge Port Door

```php
function closeChargePortDoor(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->closeChargePortDoor($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Charge Standard

```php
function chargeStandard(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->chargeStandard($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Start Charging

```php
function startCharging(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->startCharging($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Stop Charging

```php
function stopCharging(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->stopCharging($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Clear PIN to Drive Admin

Deactivates PIN to Drive and resets the associated PIN for supported firmware versions.

```php
function clearPinToDriveAdmin(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->clearPinToDriveAdmin($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Lock Doors

```php
function lockDoors(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->lockDoors($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Unlock Doors

```php
function unlockDoors(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->unlockDoors($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Erase User Data

Erases user data from the vehicle UI. Requires Guest Mode.

```php
function eraseUserData(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->eraseUserData($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Flash Lights

Briefly flashes vehicle headlights.

```php
function flashLights(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->flashLights($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Enable or Disable Guest Mode

```php
function enableOrDisableGuestMode(string $vehicleTag, GuestModeRequest $body): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |
| `body` | [`GuestModeRequest`](../../doc/models/guest-mode-request.md) | Body, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$body = GuestModeRequestBuilder::init(
    false
)->build();

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->enableOrDisableGuestMode(
    $vehicleTag,
    $body
);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Honk Horn

```php
function honkHorn(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->honkHorn($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Next Favorite Media Track

```php
function nextFavoriteMediaTrack(string $vehicleTag): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `vehicleTag` | `string` | Template, Required | - |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CommandResponse`](../../doc/models/command-response.md).

## Example Usage

```php
$vehicleTag = 'vehicle_tag6';

$vehicleCommandsController = $client->getVehicleCommandsController();
$apiResponse = $vehicleCommandsController->nextFavoriteMediaTrack($vehicleTag);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'CommandResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```

