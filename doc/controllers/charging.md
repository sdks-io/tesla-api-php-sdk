# Charging

Charging history, invoices, and session data

```php
$chargingController = $client->getChargingController();
```

## Class Name

`ChargingController`

## Methods

* [Get Charging History](../../doc/controllers/charging.md#get-charging-history)
* [Get Charging Invoice](../../doc/controllers/charging.md#get-charging-invoice)
* [Get Charging Sessions](../../doc/controllers/charging.md#get-charging-sessions)


# Get Charging History

Returns the paginated charging history for the authenticated account.

```php
function getChargingHistory(): ApiResponse
```

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`ChargingHistoryResponse`](../../doc/models/charging-history-response.md).

## Example Usage

```php
$chargingController = $client->getChargingController();
$apiResponse = $chargingController->getChargingHistory();

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'ChargingHistoryResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Get Charging Invoice

Returns a charging invoice PDF for a charging session.

```php
function getChargingInvoice(string $id): ApiResponse
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `string` | Template, Required | Charging session invoice identifier |

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type `mixed`.

## Example Usage

```php
$id = 'id0';

$chargingController = $client->getChargingController();
$apiResponse = $chargingController->getChargingInvoice($id);

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'mixed:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```


# Get Charging Sessions

Returns charging session information. Only available for business fleet owners.

```php
function getChargingSessions(): ApiResponse
```

## Requires scope

### thirdpartytoken

`energy_cmds`, `energy_device_data`, `enterprise_management`, `offline_access`, `openid`, `user_data`, `vehicle_charging_cmds`, `vehicle_cmds`, `vehicle_device_data`, `vehicle_location`, `vehicle_specs`

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `getResult()` method on this instance returns the response data which is of type [`ChargingSessionsResponse`](../../doc/models/charging-sessions-response.md).

## Example Usage

```php
$chargingController = $client->getChargingController();
$apiResponse = $chargingController->getChargingSessions();

// Extracting response status code
var_dump($apiResponse->getStatusCode());
// Extracting response headers
var_dump($apiResponse->getHeaders());

if ($apiResponse->isSuccess()) {
    echo 'ChargingSessionsResponse:';
    var_dump($apiResponse->getResult());
} else {
    $error = $apiResponse->getResult();
    var_dump($error);
}
```

