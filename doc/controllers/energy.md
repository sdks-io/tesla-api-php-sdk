# Energy

Energy site and Powerwall endpoints

```php
$energyController = $client->getEnergyController();
```

## Class Name

`EnergyController`

## Methods

* [Adjust Site S Backup Reserve](../../doc/controllers/energy.md#adjust-site-s-backup-reserve)
* [Get Backup or Energy History](../../doc/controllers/energy.md#get-backup-or-energy-history)
* [Get Wall Connector Charging History](../../doc/controllers/energy.md#get-wall-connector-charging-history)
* [Get Live Site Status](../../doc/controllers/energy.md#get-live-site-status)
* [Set Site Mode Autonomous or Self Consumption](../../doc/controllers/energy.md#set-site-mode-autonomous-or-self-consumption)
* [Allow Disallow Charging From the Grid and Exporting Energy to the Grid](../../doc/controllers/energy.md#allow-disallow-charging-from-the-grid-and-exporting-energy-to-the-grid)
* [Adjust Site S Off Grid Vehicle Charging Reserve](../../doc/controllers/energy.md#adjust-site-s-off-grid-vehicle-charging-reserve)
* [Update Storm Watch Participation](../../doc/controllers/energy.md#update-storm-watch-participation)
* [Update Time of Use Tou Settings](../../doc/controllers/energy.md#update-time-of-use-tou-settings)
* [Get User Products Vehicles Energy Sites](../../doc/controllers/energy.md#get-user-products-vehicles-energy-sites)
* [Get Site Information Assets Settings Features](../../doc/controllers/energy.md#get-site-information-assets-settings-features)


# Adjust Site S Backup Reserve

```php
function adjustSiteSBackupReserve(string $energySiteId, BackupRequest $body): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | [`BackupRequest`](../../doc/models/backup-request.md) | Body, Required | - |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`BackupResponse`](../../doc/models/backup-response.md).

## Example Usage

```php
$energySiteId = 'energy_site_id2';

$body = BackupRequestBuilder::init(
    76
)->build();

$apiResponse = $energyController->adjustSiteSBackupReserve(
    $energySiteId,
    $body
);
```


# Get Backup or Energy History

```php
function getBackupOrEnergyHistory(
    string $energySiteId,
    string $kind,
    \DateTime $startDate,
    \DateTime $endDate,
    ?string $period = null,
    ?string $timeZone = null
): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `kind` | [`string(Kind)`](../../doc/models/kind.md) | Query, Required | - |
| `startDate` | `DateTime` | Query, Required | - |
| `endDate` | `DateTime` | Query, Required | - |
| `period` | `?string` | Query, Optional | - |
| `timeZone` | `?string` | Query, Optional | - |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`CalendarHistoryResponse`](../../doc/models/calendar-history-response.md).

## Example Usage

```php
$energySiteId = 'energy_site_id2';

$kind = Kind::BACKUP;

$startDate = DateTimeHelper::fromRfc3339DateTimeRequired('2016-03-13T12:52:32.123Z');

$endDate = DateTimeHelper::fromRfc3339DateTimeRequired('2016-03-13T12:52:32.123Z');

$apiResponse = $energyController->getBackupOrEnergyHistory(
    $energySiteId,
    $kind,
    $startDate,
    $endDate
);
```


# Get Wall Connector Charging History

```php
function getWallConnectorChargingHistory(
    string $energySiteId,
    string $kind,
    \DateTime $startDate,
    \DateTime $endDate,
    ?string $timeZone = null
): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `kind` | [`string(KindGetWallConnectorChargingHistory)`](../../doc/models/kind-get-wall-connector-charging-history.md) | Query, Required | - |
| `startDate` | `DateTime` | Query, Required | - |
| `endDate` | `DateTime` | Query, Required | - |
| `timeZone` | `?string` | Query, Optional | - |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`ChargeHistoryResponse`](../../doc/models/charge-history-response.md).

## Example Usage

```php
$energySiteId = 'energy_site_id2';

$kind = KindGetWallConnectorChargingHistory::CHARGE;

$startDate = DateTimeHelper::fromRfc3339DateTimeRequired('2016-03-13T12:52:32.123Z');

$endDate = DateTimeHelper::fromRfc3339DateTimeRequired('2016-03-13T12:52:32.123Z');

$apiResponse = $energyController->getWallConnectorChargingHistory(
    $energySiteId,
    $kind,
    $startDate,
    $endDate
);
```


# Get Live Site Status

```php
function getLiveSiteStatus(string $energySiteId): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`LiveStatusResponse`](../../doc/models/live-status-response.md).

## Example Usage

```php
$energySiteId = 'energy_site_id2';

$apiResponse = $energyController->getLiveSiteStatus($energySiteId);
```


# Set Site Mode Autonomous or Self Consumption

```php
function setSiteModeAutonomousOrSelfConsumption(string $energySiteId, OperationRequest $body): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | [`OperationRequest`](../../doc/models/operation-request.md) | Body, Required | - |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`GenericUpdateResponse`](../../doc/models/generic-update-response.md).

## Example Usage

```php
$energySiteId = 'energy_site_id2';

$body = OperationRequestBuilder::init(
    DefaultRealMode::AUTONOMOUS
)->build();

$apiResponse = $energyController->setSiteModeAutonomousOrSelfConsumption(
    $energySiteId,
    $body
);
```


# Allow Disallow Charging From the Grid and Exporting Energy to the Grid

```php
function allowDisallowChargingFromTheGridAndExportingEnergyToTheGrid(
    string $energySiteId,
    ?array $body = null
): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | `?array` | Body, Optional | - |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`GenericUpdateResponse`](../../doc/models/generic-update-response.md).

## Example Usage

```php
$energySiteId = 'energy_site_id2';

$apiResponse = $energyController->allowDisallowChargingFromTheGridAndExportingEnergyToTheGrid($energySiteId);
```


# Adjust Site S Off Grid Vehicle Charging Reserve

```php
function adjustSiteSOffGridVehicleChargingReserve(
    string $energySiteId,
    OffGridVehicleChargingReserveRequest $body
): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | [`OffGridVehicleChargingReserveRequest`](../../doc/models/off-grid-vehicle-charging-reserve-request.md) | Body, Required | - |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`GenericUpdateResponse`](../../doc/models/generic-update-response.md).

## Example Usage

```php
$energySiteId = 'energy_site_id2';

$body = OffGridVehicleChargingReserveRequestBuilder::init(
    52
)->build();

$apiResponse = $energyController->adjustSiteSOffGridVehicleChargingReserve(
    $energySiteId,
    $body
);
```


# Update Storm Watch Participation

```php
function updateStormWatchParticipation(string $energySiteId, StormModeRequest $body): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | [`StormModeRequest`](../../doc/models/storm-mode-request.md) | Body, Required | - |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`GenericUpdateResponse`](../../doc/models/generic-update-response.md).

## Example Usage

```php
$energySiteId = 'energy_site_id2';

$body = StormModeRequestBuilder::init(
    false
)->build();

$apiResponse = $energyController->updateStormWatchParticipation(
    $energySiteId,
    $body
);
```


# Update Time of Use Tou Settings

```php
function updateTimeOfUseTouSettings(string $energySiteId, TimeOfUseSettingsRequest $body): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |
| `body` | [`TimeOfUseSettingsRequest`](../../doc/models/time-of-use-settings-request.md) | Body, Required | - |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`GenericUpdateResponse`](../../doc/models/generic-update-response.md).

## Example Usage

```php
$energySiteId = 'energy_site_id2';

$body = TimeOfUseSettingsRequestBuilder::init(
    TouSettingsBuilder::init()->build()
)->build();

$apiResponse = $energyController->updateTimeOfUseTouSettings(
    $energySiteId,
    $body
);
```


# Get User Products Vehicles Energy Sites

```php
function getUserProductsVehiclesEnergySites(): ApiResponse
```

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`ProductsResponse`](../../doc/models/products-response.md).

## Example Usage

```php
$apiResponse = $energyController->getUserProductsVehiclesEnergySites();
```


# Get Site Information Assets Settings Features

```php
function getSiteInformationAssetsSettingsFeatures(string $energySiteId): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `energySiteId` | `string` | Template, Required | - |

## Requires scope

### oauth2

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`SiteInfoResponse`](../../doc/models/site-info-response.md).

## Example Usage

```php
$energySiteId = 'energy_site_id2';

$apiResponse = $energyController->getSiteInformationAssetsSettingsFeatures($energySiteId);
```

