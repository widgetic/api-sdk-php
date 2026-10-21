# WidgeticApi\ManagedUsersApi

All URIs are relative to https://api.widgetic.com/v1, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**copyPresetForManagedUser_0()**](ManagedUsersApi.md#copyPresetForManagedUser_0) | **POST** /managed-users/{id}/presets/{key}/copy | Give a managed user a copy of one of your presets |
| [**createCompositionFromPreset_0()**](ManagedUsersApi.md#createCompositionFromPreset_0) | **POST** /managed-users/{id}/presets/{key}/composition | Create a composition from one of your presets in one call |
| [**createManagedUserEditorSession_0()**](ManagedUsersApi.md#createManagedUserEditorSession_0) | **POST** /managed-users/{id}/editor-sessions | Create an editor session for a managed user |
| [**createManagedUser_0()**](ManagedUsersApi.md#createManagedUser_0) | **POST** /managed-users | Create Managed User |
| [**deleteManagedUser_0()**](ManagedUsersApi.md#deleteManagedUser_0) | **DELETE** /managed-users/{id} | Delete Managed User |
| [**getAllManagedUsers_0()**](ManagedUsersApi.md#getAllManagedUsers_0) | **GET** /managed-users | Get Managed Users |
| [**getManagedUserById_0()**](ManagedUsersApi.md#getManagedUserById_0) | **GET** /managed-users/{id} | Get Managed User By ID |
| [**getManagedUserDesignDefaults_0()**](ManagedUsersApi.md#getManagedUserDesignDefaults_0) | **GET** /managed-users/{id}/design-defaults | Read design defaults for one managed user |
| [**getManagedUserLimits_0()**](ManagedUsersApi.md#getManagedUserLimits_0) | **GET** /managed-users/{id}/limits | Read monthly credit cap and usage for one managed user |
| [**getManagedUserStorageUsage_0()**](ManagedUsersApi.md#getManagedUserStorageUsage_0) | **GET** /managed-users/{id}/storage-usage | Storage used by one managed user&#39;s uploads |
| [**getManagedUserUsage_0()**](ManagedUsersApi.md#getManagedUserUsage_0) | **GET** /managed-users/{id}/usage | What a managed user&#39;s editor sessions spent |
| [**getManagedUsersByManagerId_0()**](ManagedUsersApi.md#getManagedUsersByManagerId_0) | **GET** /users/{managerId}/managed-users | Get Managed Users By Manager |
| [**revokeManagedUserEditorSession_0()**](ManagedUsersApi.md#revokeManagedUserEditorSession_0) | **DELETE** /managed-users/{id}/editor-sessions/{sessionId} | End one editor session of a managed user |
| [**revokeManagedUserEditorSessions_0()**](ManagedUsersApi.md#revokeManagedUserEditorSessions_0) | **DELETE** /managed-users/{id}/editor-sessions | End every editor session of a managed user |
| [**setManagedUserDesignDefaults_0()**](ManagedUsersApi.md#setManagedUserDesignDefaults_0) | **PUT** /managed-users/{id}/design-defaults | Set or clear design defaults for one managed user |
| [**setManagedUserLimits_0()**](ManagedUsersApi.md#setManagedUserLimits_0) | **PUT** /managed-users/{id}/limits | Set or clear the monthly credit cap for one managed user |
| [**updateManagedUser_0()**](ManagedUsersApi.md#updateManagedUser_0) | **PUT** /managed-users/{id} | Update Managed User |


## `copyPresetForManagedUser_0()`

```php
copyPresetForManagedUser_0($id, $key, $idempotency_key, $copy_partner_preset_request): \WidgeticApi\Model\PartnerPresetCopyResponse
```

Give a managed user a copy of one of your presets

Copies the preset `key` (see `setPartnerPreset`) onto a new canvas for one of your managed users, so their widget creator opens on a widget of their own that starts from yours. The copy is a draft widget in your account, filed under the managed user: `getAllWidgets` with `managedUserId` lists it, and no other managed user's editor can reach it.  The copy carries the preset's code, design and content schemas, and thumbnail, and starts from a fork of its code repository, so the user's chat edits begin where yours left off. It does not carry the preset's database or its compositions. It is not a preset itself, and changing or removing the preset afterwards never touches it.  To start a composition (the content and design editor) instead, you do not need a copy: call `createComposition` with the preset's `widgetId` (from `listPartnerPresets`) and the managed user.  The `Idempotency-Key` header is required (`400` without it). Send the same key when you retry, so one copy is made, not two. A copy that could not be made leaves nothing behind (503 `PRESET_COPY_FAILED`).  The managed user must be yours and active.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The managed user to give the copy to (Widgetic's id for the user)
$key = 'key_example'; // string | The key of the preset to copy
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$copy_partner_preset_request = new \WidgeticApi\Model\CopyPartnerPresetRequest(); // \WidgeticApi\Model\CopyPartnerPresetRequest

try {
    $result = $apiInstance->copyPresetForManagedUser_0($id, $key, $idempotency_key, $copy_partner_preset_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->copyPresetForManagedUser_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The managed user to give the copy to (Widgetic&#39;s id for the user) | |
| **key** | **string**| The key of the preset to copy | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **copy_partner_preset_request** | [**\WidgeticApi\Model\CopyPartnerPresetRequest**](../Model/CopyPartnerPresetRequest.md)|  | [optional] |

### Return type

[**\WidgeticApi\Model\PartnerPresetCopyResponse**](../Model/PartnerPresetCopyResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createCompositionFromPreset_0()`

```php
createCompositionFromPreset_0($id, $key, $idempotency_key, $create_composition_from_preset_request): \WidgeticApi\Model\CreateCompositionFromWidget201Response
```

Create a composition from one of your presets in one call

Validates the name, optional content, design, embed settings and locale, then creates a draft composition filed under the managed user, built on the preset's widget, in a single insert. A failure never leaves a half-made composition.  The preset's widget must be published. The managed user must be yours and active.  A widget that keeps what visitors send (a form, a vote, a rating) declares its tables in its own source (`src/lib/meta/database.json`); they are made for the composition here, in a schema of its own, as the widget was when it was last published. A widget that keeps nothing leaves the composition without tables. If the tables cannot be made just now, or the widget's file cannot be used, the composition is still created (`201`) and `meta.warnings` says why; the tables are made the next time the widget is generated.  The `Idempotency-Key` header is required (`400` without it). Send the same key when you retry, so one composition is created, not two.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$key = 'key_example'; // string
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$create_composition_from_preset_request = {"name":"Customer rating page","embedSettings":{"width":640,"height":480},"locale":"fr-FR"}; // \WidgeticApi\Model\CreateCompositionFromPresetRequest

try {
    $result = $apiInstance->createCompositionFromPreset_0($id, $key, $idempotency_key, $create_composition_from_preset_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->createCompositionFromPreset_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **key** | **string**|  | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **create_composition_from_preset_request** | [**\WidgeticApi\Model\CreateCompositionFromPresetRequest**](../Model/CreateCompositionFromPresetRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\CreateCompositionFromWidget201Response**](../Model/CreateCompositionFromWidget201Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createManagedUserEditorSession_0()`

```php
createManagedUserEditorSession_0($id, $new_editor_session): \WidgeticApi\Model\EditorSessionResponse
```

Create an editor session for a managed user

Makes a short-lived credential that lets the browser of ONE of your managed users use Widgetic's editor pieces, such as the File Browser and the composition editor, without your API key ever reaching that browser. Call this from your server when the page that hosts the editor opens, and hand the `token` in the answer to that page.  The token is shown once. It starts with `wgt_ses_` and the browser sends it as `Authorization: Bearer <token>`. It can do only what the `surfaces` you name allow, and only for this managed user:  - `files`: upload a file (`uploadsPost`) and list the files uploaded for this user (`uploadsGet`). Every   file is filed for this user and stored in your own storage destination, never in Widgetic's: a file a   customer uploads is yours to keep, and takes none of your storage allowance. Partner storage is not   optional, so no session, whatever its surfaces, can be made until you have set a destination   (`setPartnerStorageDestination`); until then it is refused with 409 and `PARTNER_STORAGE_REQUIRED`, and   when the destination cannot be used with 503 and `STORAGE_DESTINATION_UNAVAILABLE`. A destination you   remove after the session was made stops its uploads too (the same 409; the browser is only told that   the feature is not available right now). To keep a customer from uploading, leave `files` out of the   session and hand the editors your own media library instead (`mediaLibrary`). - `editor`: edit one of this user's compositions: read it (`getCompositionById`, its content, design,   embed settings and schemas), check a content change (`validateCompositionContent`), and change its   name, content, design and embed settings (`updateComposition`, `setDynamicContent`). It can reach   only compositions you created for this managed user (tag them with `managedUserId` when you create   them); any other composition, including another of your users', answers 404. - `creator`: use Widgetic's widget creator for this user, including its AI. Draw on canvases and save   them (`getAllCanvases`, `getCanvas`, `createCanvas`, `updateCanvas`, `previewDeleteCanvas`,   `deleteCanvas`); make, change, copy and delete the widgets on them (`createWidget`, `getWidgets`,   `getWidgetsBatch`, `updateWidget`, `uploadWidgetThumbnail`, `duplicateWidget`, `deleteWidget`);   list and make the compositions of a widget it built (`getAllCompositions`, `createComposition`), which   is how it shows the widget with sample values; keep the   conversation of each widget (`getConversationsByWidgetId`, `createConversationForWidget`,   `updateConversation`, `getMessages`, `createMessage`, `updateMessage`, `restoreCheckpoint`); and read a   widget's schemas and give it its repository (`getWidgetContentSchema`, `getWidgetDesignSchema`,   `updateWidgetRepository`). The AI that builds a widget is part of it: list the models   (`agentModelsGet`), open the widget's repository (`agentRepositoriesPost`,   `agentRepositoriesRepoIdGet`), start a generation and follow or cancel it (`agentCodeGeneratePost`,   `operationsStreamGet`, `operationsIdGet`, `operationsIdCancelPost`), build and preview the result   (`agentWidgetBuilderRepoHeadWidgetIdGet`, `buildWidgetFromRepo`, `previewWidgetVersion`), publish a   version of the widget and move between its versions (`agentWidgetBuilderPublishWidgetIdPost`,   `getWidgetPublishHistory`, `setWidgetPublishHistoryLive`, `renameWidgetPublishHistoryTitle`), and   turn a stroke or a sentence into a decision (`agentShapeRecognizePost`, `agentDesignResolvePost`). It can   also offer the customer your presets as starting points: read them and ask for a copy for this customer   (`listMyPresets`, `copyMyPreset`; you choose the presets with `setPartnerPreset`).   What the session makes is filed for this managed user, and the lists it reads hold only this user's   canvases, widgets and compositions. It can reach only canvases, widgets, compositions, repositories,   uploaded files and operations made for this managed user (tag the canvases and widgets you create   with `managedUserId`); any other canvas, widget, composition, conversation, message, repository, file   or operation, including another of your users', answers 404. The creator also saves the composition   it is editing (`updateComposition`, from the `editor` surface) and attaches pictures to its chat   (`uploadsPost`, from the `files` surface), and the surfaces do not imply one another: to open the   whole creator for a user, ask for `creator`, `editor` and `files` together. A generation or a build   one user starts can be followed and cancelled by that user and by you, never by another of your   users. The AI is paid for by your account, as your own calls are: its credits and allowances are   yours. A session cannot make a widget public (publishing a version does not), file one under a   project or an organization, or set anything the creator does not set: a body with another field is   refused with 403 and `EDITOR_SESSION_FIELD_NOT_ALLOWED`.  Everything else is refused with 403 and `EDITOR_SESSION_ROUTE_NOT_ALLOWED`: a session cannot read your account, make more sessions, change your presets or delete a composition, and a session without the `creator` surface cannot create or list compositions. Create the composition yourself with your API key, then open the editor on it.  A session ends at `expiresAt` (at most four hours), when you end it (`revokeManagedUserEditorSession`), or when the managed user is switched off or deleted. A managed user can have at most 100 live sessions at once (`429 EDITOR_SESSION_LIMIT_REACHED`). A session that is bound to a web page (`allowedOrigin`) is refused from any other origin.  The AI the session runs is paid for with your credits. Set `maxCredits` to hold the session to a number of them: once its generations have taken that many (a generation that fails is refunded and does not count), the next one is refused with 402 and `EDITOR_SESSION_CREDIT_LIMIT_REACHED`, and the browser is told only that the feature is not available right now. Without it, the limit Widgetic has set for your account applies when it has set one (the same limit for every session you make, and `maxCredits: null` asks for none), and otherwise the credits of your account are the only ceiling. What each of your users' sessions has spent is in `getManagedUserUsage`.  Each call makes a new session. It does not take an `Idempotency-Key`: the answer holds the token, and the token is never stored where a retry could read it back. The answer is sent with `Cache-Control: no-store`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The managed user the session is for (Widgetic's id for the user)
$new_editor_session = new \WidgeticApi\Model\NewEditorSession(); // \WidgeticApi\Model\NewEditorSession

try {
    $result = $apiInstance->createManagedUserEditorSession_0($id, $new_editor_session);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->createManagedUserEditorSession_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The managed user the session is for (Widgetic&#39;s id for the user) | |
| **new_editor_session** | [**\WidgeticApi\Model\NewEditorSession**](../Model/NewEditorSession.md)|  | |

### Return type

[**\WidgeticApi\Model\EditorSessionResponse**](../Model/EditorSessionResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createManagedUser_0()`

```php
createManagedUser_0($idempotency_key, $new_managed_user): \WidgeticApi\Model\ManagedUserResponse
```

Create Managed User

Creates a new managed user for a partner account.  The `Idempotency-Key` header is required (`400` without it). Send the same key when you retry, so one managed user is created, not two.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$new_managed_user = {"externalId":"external-user-123","metadata":{"firstName":"John","lastName":"Doe","role":"editor"}}; // \WidgeticApi\Model\NewManagedUser

try {
    $result = $apiInstance->createManagedUser_0($idempotency_key, $new_managed_user);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->createManagedUser_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **new_managed_user** | [**\WidgeticApi\Model\NewManagedUser**](../Model/NewManagedUser.md)|  | |

### Return type

[**\WidgeticApi\Model\ManagedUserResponse**](../Model/ManagedUserResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteManagedUser_0()`

```php
deleteManagedUser_0($id): \WidgeticApi\Model\DeleteManagedUser200Response
```

Delete Managed User

Deletes a managed user by ID. Its editor sessions end with it. What was filed under it (compositions, widgets, uploads) stays in your account, untagged.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the managed user to delete

try {
    $result = $apiInstance->deleteManagedUser_0($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->deleteManagedUser_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the managed user to delete | |

### Return type

[**\WidgeticApi\Model\DeleteManagedUser200Response**](../Model/DeleteManagedUser200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getAllManagedUsers_0()`

```php
getAllManagedUsers_0($page, $size, $sort): \WidgeticApi\Model\GetAllManagedUsers200Response
```

Get Managed Users

Retrieve the managed users you manage, with pagination support. (Admins see every partner's managed users.)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$page = 1; // int | Page number for pagination
$size = 10; // int | Number of items per page
$sort = 'createdAt:desc'; // string | Sort field and direction, `<field>:<asc|desc>`. The field is `createdAt`, `updatedAt` or `externalId` (the snake_case spellings `created_at`, `updated_at` and `external_id` work too); `asc` or `desc` alone sorts by `createdAt`. Any other field is a 400.

try {
    $result = $apiInstance->getAllManagedUsers_0($page, $size, $sort);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->getAllManagedUsers_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **int**| Page number for pagination | [optional] [default to 1] |
| **size** | **int**| Number of items per page | [optional] [default to 10] |
| **sort** | **string**| Sort field and direction, &#x60;&lt;field&gt;:&lt;asc|desc&gt;&#x60;. The field is &#x60;createdAt&#x60;, &#x60;updatedAt&#x60; or &#x60;externalId&#x60; (the snake_case spellings &#x60;created_at&#x60;, &#x60;updated_at&#x60; and &#x60;external_id&#x60; work too); &#x60;asc&#x60; or &#x60;desc&#x60; alone sorts by &#x60;createdAt&#x60;. Any other field is a 400. | [optional] [default to &#39;createdAt:desc&#39;] |

### Return type

[**\WidgeticApi\Model\GetAllManagedUsers200Response**](../Model/GetAllManagedUsers200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getManagedUserById_0()`

```php
getManagedUserById_0($id): \WidgeticApi\Model\ManagedUserResponse
```

Get Managed User By ID

Retrieves a specific managed user by ID.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the managed user to retrieve

try {
    $result = $apiInstance->getManagedUserById_0($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->getManagedUserById_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the managed user to retrieve | |

### Return type

[**\WidgeticApi\Model\ManagedUserResponse**](../Model/ManagedUserResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getManagedUserDesignDefaults_0()`

```php
getManagedUserDesignDefaults_0($id): \WidgeticApi\Model\GetPartnerDesignDefaults200Response
```

Read design defaults for one managed user

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string

try {
    $result = $apiInstance->getManagedUserDesignDefaults_0($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->getManagedUserDesignDefaults_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

[**\WidgeticApi\Model\GetPartnerDesignDefaults200Response**](../Model/GetPartnerDesignDefaults200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getManagedUserLimits_0()`

```php
getManagedUserLimits_0($id): \WidgeticApi\Model\GetManagedUserLimits200Response
```

Read monthly credit cap and usage for one managed user

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string

try {
    $result = $apiInstance->getManagedUserLimits_0($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->getManagedUserLimits_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

[**\WidgeticApi\Model\GetManagedUserLimits200Response**](../Model/GetManagedUserLimits200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getManagedUserStorageUsage_0()`

```php
getManagedUserStorageUsage_0($id): \WidgeticApi\Model\GetManagedUserStorageUsage200Response
```

Storage used by one managed user's uploads

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string

try {
    $result = $apiInstance->getManagedUserStorageUsage_0($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->getManagedUserStorageUsage_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

[**\WidgeticApi\Model\GetManagedUserStorageUsage200Response**](../Model/GetManagedUserStorageUsage200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getManagedUserUsage_0()`

```php
getManagedUserUsage_0($id, $start_date, $end_date): \WidgeticApi\Model\ManagedUserUsageResponse
```

What a managed user's editor sessions spent

Says how many credits the editor sessions of one of your managed users took from your account over a period, in total and for each operation. A generation costs one credit, taken from your account when it starts; one that fails is refunded and is counted as refunded, not as spent.  Only what was spent through editor sessions is here, and only since usage was first recorded: what you spend with your API key, and anything from before, is not. Use it to see which of your users spend the most, or to charge them for it. To hold one session to a number of credits, set `max_credits` when you make it (`createManagedUserEditorSession`).  The period runs from `startDate` (included) to `endDate` (not included): the 30 days before now when you give neither, and at most 366 days. A date without a time is midnight UTC at the start of that day, so for all of October give `startDate=2026-10-01` and `endDate=2026-11-01`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The managed user whose usage you want (Widgetic's id for the user)
$start_date = 'start_date_example'; // string | Start of the period, included: an ISO 8601 date (`2026-10-01`) or date-time with its offset (`2026-10-01T08:00:00Z`). Default: 30 days before `endDate`.
$end_date = 'end_date_example'; // string | End of the period, not included, in the same forms. Default: now. It must be after `startDate`, by at most 366 days.

try {
    $result = $apiInstance->getManagedUserUsage_0($id, $start_date, $end_date);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->getManagedUserUsage_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The managed user whose usage you want (Widgetic&#39;s id for the user) | |
| **start_date** | **string**| Start of the period, included: an ISO 8601 date (&#x60;2026-10-01&#x60;) or date-time with its offset (&#x60;2026-10-01T08:00:00Z&#x60;). Default: 30 days before &#x60;endDate&#x60;. | [optional] |
| **end_date** | **string**| End of the period, not included, in the same forms. Default: now. It must be after &#x60;startDate&#x60;, by at most 366 days. | [optional] |

### Return type

[**\WidgeticApi\Model\ManagedUserUsageResponse**](../Model/ManagedUserUsageResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getManagedUsersByManagerId_0()`

```php
getManagedUsersByManagerId_0($manager_id, $page, $size, $sort): \WidgeticApi\Model\GetManagedUsersByManagerIdResponse
```

Get Managed Users By Manager

Retrieve managed users for a specific manager with pagination support.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$manager_id = 'manager_id_example'; // string | ID of the manager
$page = 1; // int | Page number for pagination
$size = 10; // int | Number of items per page
$sort = 'createdAt:desc'; // string | Sort field and direction, `<field>:<asc|desc>`. The field is `createdAt`, `updatedAt` or `externalId` (the snake_case spellings `created_at`, `updated_at` and `external_id` work too); `asc` or `desc` alone sorts by `createdAt`. Any other field is a 400.

try {
    $result = $apiInstance->getManagedUsersByManagerId_0($manager_id, $page, $size, $sort);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->getManagedUsersByManagerId_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **manager_id** | **string**| ID of the manager | |
| **page** | **int**| Page number for pagination | [optional] [default to 1] |
| **size** | **int**| Number of items per page | [optional] [default to 10] |
| **sort** | **string**| Sort field and direction, &#x60;&lt;field&gt;:&lt;asc|desc&gt;&#x60;. The field is &#x60;createdAt&#x60;, &#x60;updatedAt&#x60; or &#x60;externalId&#x60; (the snake_case spellings &#x60;created_at&#x60;, &#x60;updated_at&#x60; and &#x60;external_id&#x60; work too); &#x60;asc&#x60; or &#x60;desc&#x60; alone sorts by &#x60;createdAt&#x60;. Any other field is a 400. | [optional] [default to &#39;createdAt:desc&#39;] |

### Return type

[**\WidgeticApi\Model\GetManagedUsersByManagerIdResponse**](../Model/GetManagedUsersByManagerIdResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `revokeManagedUserEditorSession_0()`

```php
revokeManagedUserEditorSession_0($id, $session_id): \WidgeticApi\Model\DeleteManagedUser200Response
```

End one editor session of a managed user

Ends the session at once: its token stops working on the next request (on another server of ours, within a few seconds). Ending a session that has already ended is fine.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The managed user the session is for
$session_id = 'session_id_example'; // string | The `sessionId` of the session, from `createManagedUserEditorSession`

try {
    $result = $apiInstance->revokeManagedUserEditorSession_0($id, $session_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->revokeManagedUserEditorSession_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The managed user the session is for | |
| **session_id** | **string**| The &#x60;sessionId&#x60; of the session, from &#x60;createManagedUserEditorSession&#x60; | |

### Return type

[**\WidgeticApi\Model\DeleteManagedUser200Response**](../Model/DeleteManagedUser200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `revokeManagedUserEditorSessions_0()`

```php
revokeManagedUserEditorSessions_0($id): \WidgeticApi\Model\RevokeManagedUserEditorSessionsResponse
```

End every editor session of a managed user

Ends all of the managed user's live editor sessions at once, for example when the user signs out of your platform. Their tokens stop working on the next request (on another server of ours, within a few seconds). It is fine to call it for a user who has none.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The managed user whose sessions end

try {
    $result = $apiInstance->revokeManagedUserEditorSessions_0($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->revokeManagedUserEditorSessions_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The managed user whose sessions end | |

### Return type

[**\WidgeticApi\Model\RevokeManagedUserEditorSessionsResponse**](../Model/RevokeManagedUserEditorSessionsResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `setManagedUserDesignDefaults_0()`

```php
setManagedUserDesignDefaults_0($id, $set_partner_design_defaults_request): \WidgeticApi\Model\GetPartnerDesignDefaults200Response
```

Set or clear design defaults for one managed user

Send `{ \"design\": { ... } }` to store a JSON object (at most 64 KB, nesting depth 32), or `{ \"design\": null }` to remove the override. New compositions for this customer merge this layer over the partner default and under the request body.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$set_partner_design_defaults_request = {"design":{"theme":{"primary":"#336699"}}}; // \WidgeticApi\Model\SetPartnerDesignDefaultsRequest

try {
    $result = $apiInstance->setManagedUserDesignDefaults_0($id, $set_partner_design_defaults_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->setManagedUserDesignDefaults_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **set_partner_design_defaults_request** | [**\WidgeticApi\Model\SetPartnerDesignDefaultsRequest**](../Model/SetPartnerDesignDefaultsRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\GetPartnerDesignDefaults200Response**](../Model/GetPartnerDesignDefaults200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `setManagedUserLimits_0()`

```php
setManagedUserLimits_0($id, $set_managed_user_limits_request): \WidgeticApi\Model\GetManagedUserLimits200Response
```

Set or clear the monthly credit cap for one managed user

Send monthlyCredits as a whole number from 0 up to 2147483647 to cap what this customer's editor sessions may spend in a UTC calendar month, or null to remove the cap. The cap counts the credits the customer's sessions spent that month (refunded credits do not count) and applies to all of the customer's sessions together, beside any `max_credits` a single session was given. A cap of 0 stops all paid work by this customer until you raise it. The cap starts counting from the first of the month (UTC); a cap set below what was already spent this month stops further work at once.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$set_managed_user_limits_request = {"monthlyCredits":1000}; // \WidgeticApi\Model\SetManagedUserLimitsRequest

try {
    $result = $apiInstance->setManagedUserLimits_0($id, $set_managed_user_limits_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->setManagedUserLimits_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **set_managed_user_limits_request** | [**\WidgeticApi\Model\SetManagedUserLimitsRequest**](../Model/SetManagedUserLimitsRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\GetManagedUserLimits200Response**](../Model/GetManagedUserLimits200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updateManagedUser_0()`

```php
updateManagedUser_0($id, $idempotency_key, $update_managed_user): \WidgeticApi\Model\ManagedUserResponse
```

Update Managed User

Updates an existing managed user. Only `externalId`, `metadata` and `isActive` can change, and `metadata` is replaced as a whole, so send all of it. `isActive: false` switches the managed user off: what it already has stays, and nothing new can be filed under it until you send `isActive: true`. Switching it off also ends all of its editor sessions, and they do not come back when you switch it on again.  The `Idempotency-Key` header is required (`400` without it).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\ManagedUsersApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the managed user to update
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$update_managed_user = new \WidgeticApi\Model\UpdateManagedUser(); // \WidgeticApi\Model\UpdateManagedUser

try {
    $result = $apiInstance->updateManagedUser_0($id, $idempotency_key, $update_managed_user);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ManagedUsersApi->updateManagedUser_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the managed user to update | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **update_managed_user** | [**\WidgeticApi\Model\UpdateManagedUser**](../Model/UpdateManagedUser.md)|  | |

### Return type

[**\WidgeticApi\Model\ManagedUserResponse**](../Model/ManagedUserResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
