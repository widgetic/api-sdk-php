# WidgeticApi\OperationsApi

All URIs are relative to https://api.widgetic.com/v1, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**operationsIdGet_0()**](OperationsApi.md#operationsIdGet_0) | **GET** /operations/{id} | Get operation status |


## `operationsIdGet_0()`

```php
operationsIdGet_0($id): \WidgeticApi\Model\OperationsIdGetResponse
```

Get operation status

Follows work that carries on after the response that started it. Duplicating a composition, for one, answers 202 with an `operationId`: ask for that operation until its `status` is `completed` (or `failed`, with the reason in `error`). A finished duplication names the new composition in `metadata.newCompositionId`.  An operation belongs to the user who started it. Asking for somebody else's operation answers 404, exactly as for one that does not exist. Administrators may read any operation.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearerAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\OperationsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | Operation identifier returned when the job was created.

try {
    $result = $apiInstance->operationsIdGet_0($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling OperationsApi->operationsIdGet_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| Operation identifier returned when the job was created. | |

### Return type

[**\WidgeticApi\Model\OperationsIdGetResponse**](../Model/OperationsIdGetResponse.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
