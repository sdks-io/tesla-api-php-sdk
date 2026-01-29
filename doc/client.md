
# Client Class Documentation

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
| loggingConfiguration | [`LoggingConfigurationBuilder`](../doc/logging-configuration-builder.md) | Represents the logging configurations for API calls |
| proxyConfiguration | [`ProxyConfigurationBuilder`](../doc/proxy-configuration-builder.md) | Represents the proxy configurations for API calls |
| bearerAuthCredentials | [`BearerAuthCredentials`](auth/oauth-2-bearer-token.md) | The Credentials Setter for OAuth 2 Bearer token |
| thirdpartytokenCredentials | [`ThirdpartytokenCredentials`](auth/oauth-2-authorization-code-grant.md) | The Credentials Setter for OAuth 2 Authorization Code Grant |

The API client can be initialized as follows:

```php
use TeslaFleetManagementApiLib\Logging\LoggingConfigurationBuilder;
use TeslaFleetManagementApiLib\Logging\RequestLoggingConfigurationBuilder;
use TeslaFleetManagementApiLib\Logging\ResponseLoggingConfigurationBuilder;
use Psr\Log\LogLevel;
use TeslaFleetManagementApiLib\Environment;
use TeslaFleetManagementApiLib\Authentication\BearerAuthCredentialsBuilder;
use TeslaFleetManagementApiLib\Authentication\ThirdpartytokenCredentialsBuilder;
use TeslaFleetManagementApiLib\Models\OAuthScopeThirdpartytoken;
use TeslaFleetManagementApiLib\TeslaFleetManagementApiClientBuilder;

$client = TeslaFleetManagementApiClientBuilder::init()
    ->bearerAuthCredentials(
        BearerAuthCredentialsBuilder::init(
            'AccessToken'
        )
    )
    ->thirdpartytokenCredentials(
        ThirdpartytokenCredentialsBuilder::init(
            'OAuthClientId',
            'OAuthClientSecret',
            'OAuthRedirectUri'
        )
            ->oAuthScopes(
                [
                    OAuthScopeThirdpartytoken::OPENID,
                    OAuthScopeThirdpartytoken::OFFLINE_ACCESS
                ]
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

## Tesla Fleet Management API Client

The gateway for the SDK. This class acts as a factory for the Controllers and also holds the configuration of the SDK.

## Controllers

| Name | Description |
|  --- | --- |
| getChargingController() | Gets ChargingController |
| getEnergyController() | Gets EnergyController |
| getPartnerController() | Gets PartnerController |
| getUserController() | Gets UserController |
| getVehiclesController() | Gets VehiclesController |
| getVehicleCommandsController() | Gets VehicleCommandsController |
| getOAuthAuthorizationController() | Gets OAuthAuthorizationController |

