# WidgeticApi\EntitlementsApi

All URIs are relative to https://api.widgetic.com/v1, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getManagedUserEntitlements_0()**](EntitlementsApi.md#getManagedUserEntitlements_0) | **GET** /entitlements/managed-users/{managedUserId} | Get managed user entitlements |
| [**getPartnerEntitlements_0()**](EntitlementsApi.md#getPartnerEntitlements_0) | **GET** /entitlements/partners/{partnerId} | Get partner entitlements |


## `getManagedUserEntitlements_0()`

```php
getManagedUserEntitlements_0($managed_user_id, $include_expired, $feature, $source): \WidgeticApi\Model\GetManagedUserEntitlementsResponse
```

Get managed user entitlements

Retrieves all entitlements for a managed user (admin or partner access).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\EntitlementsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$managed_user_id = 'managed_user_id_example'; // string | Managed user ID
$include_expired = True; // bool | Include expired entitlements in results
$feature = 'feature_example'; // string | Filter by specific feature
$source = 'source_example'; // string | Filter by entitlement source

try {
    $result = $apiInstance->getManagedUserEntitlements_0($managed_user_id, $include_expired, $feature, $source);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EntitlementsApi->getManagedUserEntitlements_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **managed_user_id** | **string**| Managed user ID | |
| **include_expired** | **bool**| Include expired entitlements in results | [optional] |
| **feature** | **string**| Filter by specific feature | [optional] |
| **source** | **string**| Filter by entitlement source | [optional] |

### Return type

[**\WidgeticApi\Model\GetManagedUserEntitlementsResponse**](../Model/GetManagedUserEntitlementsResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerEntitlements_0()`

```php
getPartnerEntitlements_0($partner_id, $include_expired, $feature, $source): \WidgeticApi\Model\GetPartnerEntitlementsResponse
```

Get partner entitlements

Retrieves all entitlements for a partner (admin or partner access).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\EntitlementsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | Partner ID
$include_expired = True; // bool | Include expired entitlements in results
$feature = 'feature_example'; // string | Filter by specific feature
$source = 'source_example'; // string | Filter by entitlement source

try {
    $result = $apiInstance->getPartnerEntitlements_0($partner_id, $include_expired, $feature, $source);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling EntitlementsApi->getPartnerEntitlements_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| Partner ID | |
| **include_expired** | **bool**| Include expired entitlements in results | [optional] |
| **feature** | **string**| Filter by specific feature | [optional] |
| **source** | **string**| Filter by entitlement source | [optional] |

### Return type

[**\WidgeticApi\Model\GetPartnerEntitlementsResponse**](../Model/GetPartnerEntitlementsResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
