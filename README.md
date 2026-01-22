
# Getting Started with Tesla Fleet Management API

## Introduction

Unofficial OpenAPI specification for Tesla Fleet Management Charging endpoints.

## Install the Package

Run the following command to install the package and automatically add the dependency to your composer.json file:

```bash
composer require "tesla/tesla-api-sdk:1.0.0"
```

Or add it to the composer.json file manually as given below:

```json
"require": {
    "tesla/tesla-api-sdk": "1.0.0"
}
```

You can also view the package at:
https://packagist.org/packages/tesla/tesla-api-sdk#1.0.0

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| environment | `Environment` | The API environment. <br> **Default: `Environment.PRODUCTION`** |
| timeout | `int` | Timeout for API calls in seconds.<br>*Default*: `0` |
| enableRetries | `bool` | Whether to enable retries and backoff feature.<br>*Default*: `false` |
| numberOfRetries | `int` | The number of retries to make.<br>*Default*: `0` |
| retryInterval | `float` | The retry time interval between the endpoint calls.<br>*Default*: `1` |
| backOffFactor | `float` | Exponential backoff factor to increase interval between retries.<br>*Default*: `2` |
| maximumRetryWaitTime | `int` | The maximum wait time in seconds for overall retrying requests.<br>*Default*: `0` |
| retryOnTimeout | `bool` | Whether to retry on request timeout.<br>*Default*: `true` |
| httpStatusCodesToRetry | `array` | Http status codes to retry against.<br>*Default*: `408, 413, 429, 500, 502, 503, 504, 521, 522, 524` |
| httpMethodsToRetry | `array` | Http methods to retry against.<br>*Default*: `'GET', 'PUT'` |
| loggingConfiguration | [`LoggingConfigurationBuilder`](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/logging-configuration-builder.md) | Represents the logging configurations for API calls |
| proxyConfiguration | [`ProxyConfigurationBuilder`](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/proxy-configuration-builder.md) | Represents the proxy configurations for API calls |
| bearerAuthCredentials | [`BearerAuthCredentials`](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/auth/oauth-2-bearer-token.md) | The Credentials Setter for OAuth 2 Bearer token |
| oauth2Credentials | [`Oauth2Credentials`](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/auth/oauth-2-authorization-code-grant.md) | The Credentials Setter for OAuth 2 Authorization Code Grant |

The API client can be initialized as follows:

```php
use TeslaFleetManagementApiLib\Logging\LoggingConfigurationBuilder;
use TeslaFleetManagementApiLib\Logging\RequestLoggingConfigurationBuilder;
use TeslaFleetManagementApiLib\Logging\ResponseLoggingConfigurationBuilder;
use Psr\Log\LogLevel;
use TeslaFleetManagementApiLib\Environment;
use TeslaFleetManagementApiLib\Authentication\BearerAuthCredentialsBuilder;
use TeslaFleetManagementApiLib\Authentication\Oauth2CredentialsBuilder;
use TeslaFleetManagementApiLib\TeslaFleetManagementApiClientBuilder;

$client = TeslaFleetManagementApiClientBuilder::init()
    ->bearerAuthCredentials(
        BearerAuthCredentialsBuilder::init(
            'AccessToken'
        )
    )
    ->oauth2Credentials(
        Oauth2CredentialsBuilder::init(
            'OAuthClientId',
            'OAuthClientSecret',
            'OAuthRedirectUri'
        )
    )
    ->environment(Environment::PRODUCTION)
    ->loggingConfiguration(
        LoggingConfigurationBuilder::init()
            ->level(LogLevel::INFO)
            ->requestConfiguration(RequestLoggingConfigurationBuilder::init()->body(true))
            ->responseConfiguration(ResponseLoggingConfigurationBuilder::init()->headers(true))
    )
    ->build();
```

## Authorization

This API uses the following authentication schemes.

* [`bearerAuth (OAuth 2 Bearer token)`](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/auth/oauth-2-bearer-token.md)
* [`oauth2 (OAuth 2 Authorization Code Grant)`](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/auth/oauth-2-authorization-code-grant.md)

## List of APIs

* [Charging](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/controllers/charging.md)
* [Energy](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/controllers/energy.md)
* [Partner](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/controllers/partner.md)
* [User](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/controllers/user.md)
* [Vehicles](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/controllers/vehicles.md)

## SDK Infrastructure

### Configuration

* [ProxyConfigurationBuilder](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/proxy-configuration-builder.md)
* [LoggingConfigurationBuilder](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/logging-configuration-builder.md)
* [RequestLoggingConfigurationBuilder](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/request-logging-configuration-builder.md)
* [ResponseLoggingConfigurationBuilder](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/response-logging-configuration-builder.md)

### HTTP

* [HttpRequest](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/http-request.md)

### Utilities

* [ApiResponse](https://www.github.com/sdks-io/tesla-api-php-sdk/tree/1.0.0/doc/api-response.md)

