# WidgeticApi\UploadsApi

All URIs are relative to https://api.widgetic.com/v1, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**uploadsGet_0()**](UploadsApi.md#uploadsGet_0) | **GET** /uploads | List the account&#39;s uploads |
| [**uploadsIdDelete_0()**](UploadsApi.md#uploadsIdDelete_0) | **DELETE** /uploads/{id} | Delete an upload |
| [**uploadsIdGet_0()**](UploadsApi.md#uploadsIdGet_0) | **GET** /uploads/{id} | Get an upload by id |
| [**uploadsLimitsGet_0()**](UploadsApi.md#uploadsLimitsGet_0) | **GET** /uploads/limits | Upload size limits and accepted file types |
| [**uploadsPost_0()**](UploadsApi.md#uploadsPost_0) | **POST** /uploads | Upload a file |


## `uploadsGet_0()`

```php
uploadsGet_0($limit, $managed_user_id, $managed_user_external_id): \WidgeticApi\Model\UploadsGet200Response
```

List the account's uploads

The files the account has uploaded, newest first. Deleted files are not listed. Returns at most `limit` files and has no further pages: a client that needs more narrows the list instead, for example to one managed user's files with `managedUserId` or `managedUserExternalId`. The files that visitors sent through a widget's upload adapter (`source` is `widget-visitor-upload`) are not part of this list, so that a popular widget does not push the account's own files out of it; naming one widget with `widgetId` lists what visitors sent to that widget as well.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\UploadsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$limit = 50; // int | Maximum number of files to return
$managed_user_id = 'managed_user_id_example'; // string | List only the files uploaded for this managed user (Widgetic's id for the user). Send this or `managedUserExternalId`, not both.
$managed_user_external_id = 'managed_user_external_id_example'; // string | List only the files uploaded for the managed user you registered with this `externalId` (your own identifier for the user). Send this or `managedUserId`, not both.

try {
    $result = $apiInstance->uploadsGet_0($limit, $managed_user_id, $managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UploadsApi->uploadsGet_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **int**| Maximum number of files to return | [optional] [default to 50] |
| **managed_user_id** | **string**| List only the files uploaded for this managed user (Widgetic&#39;s id for the user). Send this or &#x60;managedUserExternalId&#x60;, not both. | [optional] |
| **managed_user_external_id** | **string**| List only the files uploaded for the managed user you registered with this &#x60;externalId&#x60; (your own identifier for the user). Send this or &#x60;managedUserId&#x60;, not both. | [optional] |

### Return type

[**\WidgeticApi\Model\UploadsGet200Response**](../Model/UploadsGet200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `uploadsIdDelete_0()`

```php
uploadsIdDelete_0($id): \WidgeticApi\Model\UploadsIdDelete200Response
```

Delete an upload

Removes the stored file and the upload row. A file in Widgetic's own storage gives back the space it took from your storage allowance; a file in your own bucket is removed from your bucket. Deleting an upload that is already gone succeeds the same way as the first delete. An upload that belongs to another account is not found. If the storage cannot be reached the call fails and nothing is marked deleted, so it can be repeated.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\UploadsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string

try {
    $result = $apiInstance->uploadsIdDelete_0($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UploadsApi->uploadsIdDelete_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

[**\WidgeticApi\Model\UploadsIdDelete200Response**](../Model/UploadsIdDelete200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `uploadsIdGet_0()`

```php
uploadsIdGet_0($id): \WidgeticApi\Model\UploadResponse
```

Get an upload by id

The details of one of the account's uploads. An upload that belongs to another account is not found.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\UploadsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The upload to read

try {
    $result = $apiInstance->uploadsIdGet_0($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UploadsApi->uploadsIdGet_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The upload to read | |

### Return type

[**\WidgeticApi\Model\UploadResponse**](../Model/UploadResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `uploadsLimitsGet_0()`

```php
uploadsLimitsGet_0(): \WidgeticApi\Model\UploadLimitsResponse
```

Upload size limits and accepted file types

The size limit and the accepted file types of the upload endpoints. Read them from here rather than hard-coding thresholds: they are configuration and can change. The limits are the same for every account, whatever its plan: `multipart_max_bytes` for a file sent in one request (10 MB) and `tus_max_bytes` for a resumable upload (250 MB).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\UploadsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->uploadsLimitsGet_0();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UploadsApi->uploadsLimitsGet_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\WidgeticApi\Model\UploadLimitsResponse**](../Model/UploadLimitsResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `uploadsPost_0()`

```php
uploadsPost_0($file, $context_type, $source, $managed_user_id, $managed_user_external_id, $purpose): \WidgeticApi\Model\UploadResponse
```

Upload a file

Stores one file for the account and returns its public address. This is how a user's own images, video and PDFs reach a widget's content.  Send a `multipart/form-data` request with the file in the field named `file`. The file counts against the storage of the workspace it is uploaded in, and a full workspace is refused with 413 and `QUOTA_STORAGE_EXCEEDED`. For a person signed in on widgetic.com that is the workspace they are currently working in: inside a team, the team's shared storage; inside their own workspace, their own allowance. An organization API key, and a Shopify store's session, always work in that team's shared storage. A personal API key or an SDK token always uses the account's own allowance. The two never add up and one never lends room to the other. A file over the size limit is refused with 413 and `UPLOAD_TOO_LARGE`, and a type that is not accepted with 415 and `UPLOAD_UNSUPPORTED_TYPE`; `uploadsLimitsGet` lists the size limit and the accepted types.  A file is judged by what is in it, not by the type it is sent as. A file that is not the type it claims (a web page sent as `image/png`) is refused with 415 and `UPLOAD_UNSUPPORTED_TYPE`, and a picture sent under the wrong picture type is stored under the type it really is, which `mime_type` in the answer says. An SVG is rewritten as it is stored: script, `foreignObject`, animation and references to other addresses are taken out, it must be UTF-8 and at most 2 MB, and the stored file can be larger or smaller than the one sent. Anything that is not an image, audio or video (a PDF, for example) is served as a download rather than shown in a page.  When the full storage is a Shopify store's team's, extra storage cannot be added through Shopify yet, so the message ends by saying so and what to do instead: delete files, or contact support. On a Solo plan it names the Teams plan (which holds more) and `error.details.planPageUrl` is the address of the plan page on Shopify. `error.suggestedAction` says the same in a few words, instead of the usual \"upgrade your storage plan\". Any other team, and a person's own workspace, get the shorter message.  To upload the file for one of your managed users, send `managedUserId` (Widgetic's id for the user) or `managedUserExternalId` (your own identifier for the user), not both. The file stays in your account and counts against its allowance; the tag lets you list one user's files with `uploadsGet`. The managed user must be yours and active: one that is not yours, or does not exist, is refused with 404 and `MANAGED_USER_NOT_FOUND`, and one that is switched off with 409 and `MANAGED_USER_INACTIVE`, before the file is stored. The tag is set here and does not change afterwards.  Called with an editor session (`createManagedUserEditorSession`), the file is always filed for the session's own managed user and is always media for widget content: naming another managed user is refused with 403 and `MANAGED_USER_SESSION_MISMATCH`, and `contextType`, `source`, `widgetId` and `conversationId` are ignored. A full storage allowance is refused with the same 413 and `QUOTA_STORAGE_EXCEEDED`, but the message only says that it is not available right now (not how much is stored: that is the partner's business) and `error.details.limit` is `storage`.  An account that administers a partner with a storage destination (`setPartnerStorageDestination`) has its files stored in the partner's own bucket instead. Such a file takes none of the allowance, its `url` is served from the partner's public address, and its `storage_key` is the key in the partner's bucket. The file is never stored with Widgetic instead: when the destination cannot be used the upload is refused with 503 and `STORAGE_DESTINATION_UNAVAILABLE`, and when the partner's storage rejects the file with 502 and `STORAGE_DESTINATION_WRITE_FAILED`.  Partner storage is not optional, and it does not depend on how the file arrives. A partner's own uploads (with its API key, an SDK token, or from the Widgetic website, the resumable route and the media library alike) and the uploads of its customers' editor sessions are kept in the partner's own storage or not at all, so a partner with no destination (or one that removed it after the session was made) has them refused with 409 and `PARTNER_STORAGE_REQUIRED`; they are never stored with Widgetic. An editor session's browser is only told that the feature is not available right now.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\UploadsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$file = "/path/to/file.txt"; // \SplFileObject | The file to store
$context_type = 'content-property'; // string | What the file is for. Send `content-property` for media that becomes widget content (images, video and PDF); the other values are used by Widgetic's own editor.
$source = 'file-browser-upload'; // string | Which part of the product, or which client, the file comes from
$managed_user_id = 'managed_user_id_example'; // string | Upload the file for one of your managed users, by Widgetic's id for the user. Send this or `managedUserExternalId`, not both.
$managed_user_external_id = 'managed_user_external_id_example'; // string | The same, by your own identifier for the user, the `externalId` you gave when you created the managed user. Send this or `managedUserId`, not both.
$purpose = 'purpose_example'; // string | Where in your product you use the file. It is kept with the file, so that a customer's storage can be counted by purpose (`getManagedUserStorageUsage`). Optional; any other value is refused with 400 and `UPLOAD_INVALID_PURPOSE`.

try {
    $result = $apiInstance->uploadsPost_0($file, $context_type, $source, $managed_user_id, $managed_user_external_id, $purpose);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UploadsApi->uploadsPost_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **file** | **\SplFileObject****\SplFileObject**| The file to store | |
| **context_type** | **string**| What the file is for. Send &#x60;content-property&#x60; for media that becomes widget content (images, video and PDF); the other values are used by Widgetic&#39;s own editor. | [optional] [default to &#39;content-property&#39;] |
| **source** | **string**| Which part of the product, or which client, the file comes from | [optional] [default to &#39;file-browser-upload&#39;] |
| **managed_user_id** | **string**| Upload the file for one of your managed users, by Widgetic&#39;s id for the user. Send this or &#x60;managedUserExternalId&#x60;, not both. | [optional] |
| **managed_user_external_id** | **string**| The same, by your own identifier for the user, the &#x60;externalId&#x60; you gave when you created the managed user. Send this or &#x60;managedUserId&#x60;, not both. | [optional] |
| **purpose** | **string**| Where in your product you use the file. It is kept with the file, so that a customer&#39;s storage can be counted by purpose (&#x60;getManagedUserStorageUsage&#x60;). Optional; any other value is refused with 400 and &#x60;UPLOAD_INVALID_PURPOSE&#x60;. | [optional] |

### Return type

[**\WidgeticApi\Model\UploadResponse**](../Model/UploadResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
