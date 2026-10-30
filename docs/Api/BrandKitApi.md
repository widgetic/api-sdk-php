# WidgeticApi\BrandKitApi

All URIs are relative to https://api.widgetic.com/v1, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**deleteBrandKitAsset_0()**](BrandKitApi.md#deleteBrandKitAsset_0) | **DELETE** /brand-kit/assets/{assetId} | Remove a font or icon from the Brand Kit |
| [**deleteBrandKit_0()**](BrandKitApi.md#deleteBrandKit_0) | **DELETE** /brand-kit | Reset the Brand Kit to the default |
| [**getBrandKit_0()**](BrandKitApi.md#getBrandKit_0) | **GET** /brand-kit | The Brand Kit of the current workspace |
| [**patchBrandKitAsset_0()**](BrandKitApi.md#patchBrandKitAsset_0) | **PATCH** /brand-kit/assets/{assetId} | Rename an icon or relabel a font variant |
| [**patchBrandKit_0()**](BrandKitApi.md#patchBrandKit_0) | **PATCH** /brand-kit | Change part of the Brand Kit |
| [**postBrandKitFont_0()**](BrandKitApi.md#postBrandKitFont_0) | **POST** /brand-kit/fonts | Upload a font file to the Brand Kit |
| [**postBrandKitIcon_0()**](BrandKitApi.md#postBrandKitIcon_0) | **POST** /brand-kit/icons | Add a named SVG icon to the Brand Kit |
| [**putBrandKit_0()**](BrandKitApi.md#putBrandKit_0) | **PUT** /brand-kit | Save Brand Kit tokens |


## `deleteBrandKitAsset_0()`

```php
deleteBrandKitAsset_0($asset_id, $organization_id): \WidgeticApi\Model\BrandKitViewResponse
```

Remove a font or icon from the Brand Kit

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\BrandKitApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$asset_id = 'asset_id_example'; // string
$organization_id = 'organization_id_example'; // string

try {
    $result = $apiInstance->deleteBrandKitAsset_0($asset_id, $organization_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BrandKitApi->deleteBrandKitAsset_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **asset_id** | **string**|  | |
| **organization_id** | **string**|  | [optional] |

### Return type

[**\WidgeticApi\Model\BrandKitViewResponse**](../Model/BrandKitViewResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteBrandKit_0()`

```php
deleteBrandKit_0($organization_id): \WidgeticApi\Model\BrandKitViewResponse
```

Reset the Brand Kit to the default

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\BrandKitApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$organization_id = 'organization_id_example'; // string

try {
    $result = $apiInstance->deleteBrandKit_0($organization_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BrandKitApi->deleteBrandKit_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **organization_id** | **string**|  | [optional] |

### Return type

[**\WidgeticApi\Model\BrandKitViewResponse**](../Model/BrandKitViewResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getBrandKit_0()`

```php
getBrandKit_0($organization_id): \WidgeticApi\Model\BrandKitViewResponse
```

The Brand Kit of the current workspace

The colors, fonts, icons, corner radius and style notes every widget made by this account is generated with. An account that never saved a kit gets Widgetic's default one (`isDefault` is true). A partner account's kit is the default for everything its keys create, and a key reads and changes the kit of the account it belongs to; there is no kit per managed user.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\BrandKitApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$organization_id = 'organization_id_example'; // string | An organisation's kit; omit for the caller's current workspace.

try {
    $result = $apiInstance->getBrandKit_0($organization_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BrandKitApi->getBrandKit_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **organization_id** | **string**| An organisation&#39;s kit; omit for the caller&#39;s current workspace. | [optional] |

### Return type

[**\WidgeticApi\Model\BrandKitViewResponse**](../Model/BrandKitViewResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `patchBrandKitAsset_0()`

```php
patchBrandKitAsset_0($asset_id, $patch_brand_kit_asset_request, $organization_id): \WidgeticApi\Model\BrandKitViewResponse
```

Rename an icon or relabel a font variant

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\BrandKitApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$asset_id = 'asset_id_example'; // string
$patch_brand_kit_asset_request = new \WidgeticApi\Model\PatchBrandKitAssetRequest(); // \WidgeticApi\Model\PatchBrandKitAssetRequest
$organization_id = 'organization_id_example'; // string

try {
    $result = $apiInstance->patchBrandKitAsset_0($asset_id, $patch_brand_kit_asset_request, $organization_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BrandKitApi->patchBrandKitAsset_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **asset_id** | **string**|  | |
| **patch_brand_kit_asset_request** | [**\WidgeticApi\Model\PatchBrandKitAssetRequest**](../Model/PatchBrandKitAssetRequest.md)|  | |
| **organization_id** | **string**|  | [optional] |

### Return type

[**\WidgeticApi\Model\BrandKitViewResponse**](../Model/BrandKitViewResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `patchBrandKit_0()`

```php
patchBrandKit_0($patch_brand_kit_request, $organization_id): \WidgeticApi\Model\BrandKitViewResponse
```

Change part of the Brand Kit

Changes only what is sent: the colors, a font role, a spacing step, one corner radius (0 for square corners) or the style notes, and keeps the rest of the saved kit. An account that never saved a kit starts from Widgetic's default one. The response lists what is worth fixing in `warnings`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\BrandKitApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$patch_brand_kit_request = new \WidgeticApi\Model\PatchBrandKitRequest(); // \WidgeticApi\Model\PatchBrandKitRequest
$organization_id = 'organization_id_example'; // string

try {
    $result = $apiInstance->patchBrandKit_0($patch_brand_kit_request, $organization_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BrandKitApi->patchBrandKit_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **patch_brand_kit_request** | [**\WidgeticApi\Model\PatchBrandKitRequest**](../Model/PatchBrandKitRequest.md)|  | |
| **organization_id** | **string**|  | [optional] |

### Return type

[**\WidgeticApi\Model\BrandKitViewResponse**](../Model/BrandKitViewResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `postBrandKitFont_0()`

```php
postBrandKitFont_0($file, $family, $weight, $organization_id, $style): \WidgeticApi\Model\BrandKitViewResponse
```

Upload a font file to the Brand Kit

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\BrandKitApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$file = "/path/to/file.txt"; // \SplFileObject
$family = 'family_example'; // string
$weight = 56; // int
$organization_id = 'organization_id_example'; // string
$style = 'style_example'; // string

try {
    $result = $apiInstance->postBrandKitFont_0($file, $family, $weight, $organization_id, $style);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BrandKitApi->postBrandKitFont_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **file** | **\SplFileObject****\SplFileObject**|  | |
| **family** | **string**|  | |
| **weight** | **int**|  | |
| **organization_id** | **string**|  | [optional] |
| **style** | **string**|  | [optional] |

### Return type

[**\WidgeticApi\Model\BrandKitViewResponse**](../Model/BrandKitViewResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `postBrandKitIcon_0()`

```php
postBrandKitIcon_0($post_brand_kit_icon_request, $organization_id): \WidgeticApi\Model\BrandKitViewResponse
```

Add a named SVG icon to the Brand Kit

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\BrandKitApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$post_brand_kit_icon_request = new \WidgeticApi\Model\PostBrandKitIconRequest(); // \WidgeticApi\Model\PostBrandKitIconRequest
$organization_id = 'organization_id_example'; // string

try {
    $result = $apiInstance->postBrandKitIcon_0($post_brand_kit_icon_request, $organization_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BrandKitApi->postBrandKitIcon_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **post_brand_kit_icon_request** | [**\WidgeticApi\Model\PostBrandKitIconRequest**](../Model/PostBrandKitIconRequest.md)|  | |
| **organization_id** | **string**|  | [optional] |

### Return type

[**\WidgeticApi\Model\BrandKitViewResponse**](../Model/BrandKitViewResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `putBrandKit_0()`

```php
putBrandKit_0($put_brand_kit_request, $organization_id): \WidgeticApi\Model\BrandKitViewResponse
```

Save Brand Kit tokens

Replaces the colors, fonts, spacing and notes of the kit with the ones sent. To change one thing, use PATCH.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\BrandKitApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$put_brand_kit_request = new \WidgeticApi\Model\PutBrandKitRequest(); // \WidgeticApi\Model\PutBrandKitRequest
$organization_id = 'organization_id_example'; // string

try {
    $result = $apiInstance->putBrandKit_0($put_brand_kit_request, $organization_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BrandKitApi->putBrandKit_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **put_brand_kit_request** | [**\WidgeticApi\Model\PutBrandKitRequest**](../Model/PutBrandKitRequest.md)|  | |
| **organization_id** | **string**|  | [optional] |

### Return type

[**\WidgeticApi\Model\BrandKitViewResponse**](../Model/BrandKitViewResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
