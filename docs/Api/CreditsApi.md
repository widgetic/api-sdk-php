# WidgeticApi\CreditsApi

All URIs are relative to https://api.widgetic.com/v1, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getUserCreditBalance_0()**](CreditsApi.md#getUserCreditBalance_0) | **GET** /credits/user/{userId}/balance | Get an account&#39;s credit balance |
| [**getUserCreditTransactions_0()**](CreditsApi.md#getUserCreditTransactions_0) | **GET** /credits/user/{userId}/transactions | List an account&#39;s credit ledger |


## `getUserCreditBalance_0()`

```php
getUserCreditBalance_0($user_id): \WidgeticApi\Model\AccountCreditBalanceResponse
```

Get an account's credit balance

Returns the credits an account holds: the balance, and how much of it is reserved by operations that are still running.  An account reads its own balance; with a partner's API key, that is the account of the person who administers the partner. Widgetic administrators can read any account's. An account that has never held credits reads a balance of 0. `getPartnerCreditBalance` reads this same balance by partner id.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CreditsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$user_id = 'user_id_example'; // string | The account whose balance to read

try {
    $result = $apiInstance->getUserCreditBalance_0($user_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CreditsApi->getUserCreditBalance_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user_id** | **string**| The account whose balance to read | |

### Return type

[**\WidgeticApi\Model\AccountCreditBalanceResponse**](../Model/AccountCreditBalanceResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getUserCreditTransactions_0()`

```php
getUserCreditTransactions_0($user_id, $transaction_type, $limit, $offset): \WidgeticApi\Model\GetPartnerCreditTransactions200Response
```

List an account's credit ledger

Lists the entries of an account's credit ledger, newest first. This is also how an account's usage is read: every operation that spends credits is a `debit` entry, so summing the `debit` entries over a period gives the credits consumed in it, and the other types give what was added.  An account reads its own ledger; with a partner's API key, that is the account of the person who administers the partner. Widgetic administrators can read any account's. `getPartnerCreditTransactions` reads this same ledger by partner id.  The page is always bounded: `limit` defaults to 100 and is capped at 500, `offset` defaults to 0.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CreditsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$user_id = 'user_id_example'; // string | The account whose ledger to read
$transaction_type = 'transaction_type_example'; // string | Only entries of this type, for instance `debit` for the credits spent. The types are listed on `AccountCreditTransaction`.
$limit = 100; // int | Maximum number of entries to return
$offset = 0; // int | Number of entries to skip

try {
    $result = $apiInstance->getUserCreditTransactions_0($user_id, $transaction_type, $limit, $offset);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CreditsApi->getUserCreditTransactions_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user_id** | **string**| The account whose ledger to read | |
| **transaction_type** | **string**| Only entries of this type, for instance &#x60;debit&#x60; for the credits spent. The types are listed on &#x60;AccountCreditTransaction&#x60;. | [optional] |
| **limit** | **int**| Maximum number of entries to return | [optional] [default to 100] |
| **offset** | **int**| Number of entries to skip | [optional] [default to 0] |

### Return type

[**\WidgeticApi\Model\GetPartnerCreditTransactions200Response**](../Model/GetPartnerCreditTransactions200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
