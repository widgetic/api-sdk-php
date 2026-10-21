# WidgeticApi\CanvasesApi

All URIs are relative to https://api.widgetic.com/v1, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createCanvas_0()**](CanvasesApi.md#createCanvas_0) | **POST** /canvases | Create Canvas |
| [**deleteCanvas_0()**](CanvasesApi.md#deleteCanvas_0) | **DELETE** /canvases/{id} | Delete Canvas |
| [**getAllCanvases_0()**](CanvasesApi.md#getAllCanvases_0) | **GET** /canvases | Get All Canvases |
| [**getCanvas_0()**](CanvasesApi.md#getCanvas_0) | **GET** /canvases/{id} | Get Canvas |
| [**updateCanvas_0()**](CanvasesApi.md#updateCanvas_0) | **PUT** /canvases/{id} | Update Canvas |


## `createCanvas_0()`

```php
createCanvas_0($create_canvas_request): \WidgeticApi\Model\CanvasResponse
```

Create Canvas

Creates a new canvas with the specified properties.  To make the canvas for one of your managed users, send `managedUserId` or `managedUserExternalId`. The canvas stays in your account and is yours to edit; the tag lets you list one user's canvases with `getAllCanvases`. The managed user must be yours and active: one that is not yours, or does not exist, is answered with 404 and `MANAGED_USER_NOT_FOUND`, and one that is switched off with 409 and `MANAGED_USER_INACTIVE`. The tag is set here and does not change afterwards. Called with an editor session, the canvas is always made for the session's managed user.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CanvasesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$create_canvas_request = new \WidgeticApi\Model\CreateCanvasRequest(); // \WidgeticApi\Model\CreateCanvasRequest

try {
    $result = $apiInstance->createCanvas_0($create_canvas_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CanvasesApi->createCanvas_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **create_canvas_request** | [**\WidgeticApi\Model\CreateCanvasRequest**](../Model/CreateCanvasRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\CanvasResponse**](../Model/CanvasResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteCanvas_0()`

```php
deleteCanvas_0($id): \WidgeticApi\Model\CanvasResponse
```

Delete Canvas

Deletes a canvas together with every widget on it.  Called with an editor session, only a canvas whose widgets were all made for the session's managed user can be deleted; one that also holds somebody else's widgets is refused with 409 and `CANVAS_HAS_OTHER_WIDGETS`, and nothing is deleted. Delete such a canvas with your API key.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CanvasesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the canvas

try {
    $result = $apiInstance->deleteCanvas_0($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CanvasesApi->deleteCanvas_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the canvas | |

### Return type

[**\WidgeticApi\Model\CanvasResponse**](../Model/CanvasResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getAllCanvases_0()`

```php
getAllCanvases_0($page, $size, $sort, $created_after, $created_before, $updated_after, $updated_before, $managed_user_id, $managed_user_external_id): \WidgeticApi\Model\GetAllCanvasesResponse
```

Get All Canvases

Retrieves all canvases with pagination support and filtering options.  Pass `managedUserId` (Widgetic's id for one of your managed users) or `managedUserExternalId` (your own identifier for the user) to list only the canvases made for that managed user. The canvases of your other managed users, and your own, are left out. A managed user that is not yours, or does not exist, is answered with 404 and `MANAGED_USER_NOT_FOUND`. Called with an editor session, the list is always the session's managed user's.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CanvasesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$page = 1; // int | Page number for pagination
$size = 20; // int | Number of items per page
$sort = 'created_at:desc'; // string | Sort field and direction (e.g., \"created_at:desc\")
$created_after = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Filter canvases created after the specified date (ISO 8601 format)
$created_before = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Filter canvases created before the specified date (ISO 8601 format)
$updated_after = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Filter canvases updated after the specified date (ISO 8601 format)
$updated_before = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Filter canvases updated before the specified date (ISO 8601 format)
$managed_user_id = 'managed_user_id_example'; // string | List only the canvases made for this managed user (Widgetic's id for the user). Send this or `managedUserExternalId`, not both.
$managed_user_external_id = 'managed_user_external_id_example'; // string | List only the canvases made for the managed user you registered with this `externalId` (your own identifier for the user). Send this or `managedUserId`, not both.

try {
    $result = $apiInstance->getAllCanvases_0($page, $size, $sort, $created_after, $created_before, $updated_after, $updated_before, $managed_user_id, $managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CanvasesApi->getAllCanvases_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **int**| Page number for pagination | [optional] [default to 1] |
| **size** | **int**| Number of items per page | [optional] [default to 20] |
| **sort** | **string**| Sort field and direction (e.g., \&quot;created_at:desc\&quot;) | [optional] [default to &#39;created_at:desc&#39;] |
| **created_after** | **\DateTime**| Filter canvases created after the specified date (ISO 8601 format) | [optional] |
| **created_before** | **\DateTime**| Filter canvases created before the specified date (ISO 8601 format) | [optional] |
| **updated_after** | **\DateTime**| Filter canvases updated after the specified date (ISO 8601 format) | [optional] |
| **updated_before** | **\DateTime**| Filter canvases updated before the specified date (ISO 8601 format) | [optional] |
| **managed_user_id** | **string**| List only the canvases made for this managed user (Widgetic&#39;s id for the user). Send this or &#x60;managedUserExternalId&#x60;, not both. | [optional] |
| **managed_user_external_id** | **string**| List only the canvases made for the managed user you registered with this &#x60;externalId&#x60; (your own identifier for the user). Send this or &#x60;managedUserId&#x60;, not both. | [optional] |

### Return type

[**\WidgeticApi\Model\GetAllCanvasesResponse**](../Model/GetAllCanvasesResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCanvas_0()`

```php
getCanvas_0($id): \WidgeticApi\Model\CanvasResponse
```

Get Canvas

Retrieves a specific canvas by ID.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CanvasesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the canvas

try {
    $result = $apiInstance->getCanvas_0($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CanvasesApi->getCanvas_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the canvas | |

### Return type

[**\WidgeticApi\Model\CanvasResponse**](../Model/CanvasResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updateCanvas_0()`

```php
updateCanvas_0($id, $update_canvas_request): \WidgeticApi\Model\CanvasResponse
```

Update Canvas

Updates an existing canvas with the specified properties.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CanvasesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the canvas to update
$update_canvas_request = new \WidgeticApi\Model\UpdateCanvasRequest(); // \WidgeticApi\Model\UpdateCanvasRequest

try {
    $result = $apiInstance->updateCanvas_0($id, $update_canvas_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CanvasesApi->updateCanvas_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the canvas to update | |
| **update_canvas_request** | [**\WidgeticApi\Model\UpdateCanvasRequest**](../Model/UpdateCanvasRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\CanvasResponse**](../Model/CanvasResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
