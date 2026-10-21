# WidgeticApi\InvoicesApi

All URIs are relative to https://api.widgetic.com/v1, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getInvoicesByPartnerId_0()**](InvoicesApi.md#getInvoicesByPartnerId_0) | **GET** /invoices/partner/{partnerId} | List a partner&#39;s invoices |


## `getInvoicesByPartnerId_0()`

```php
getInvoicesByPartnerId_0($partner_id, $status, $limit, $offset): \WidgeticApi\Model\GetInvoicesByPartnerId200Response
```

List a partner's invoices

Lists the invoices issued to a partner, newest first. Each carries the price (`subtotal`), the tax on it (`taxAmount`) and what is paid (`total`), its status as the payment provider reports it, why the last payment failed (`failureReason`), and the page where it is paid (`hostedInvoiceUrl`).  A partner reads its own: the caller must be the person who administers the partner (an API key of that account works), and anyone else is refused with 403 whether or not the partner exists. Widgetic administrators can read any partner's and see exactly what the partner sees; the full records, with the internal fields, are `getAllInvoices` filtered by partner.  The page is always bounded: `limit` defaults to 50 and is capped at 100, `offset` defaults to 0.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\InvoicesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose invoices to list
$status = 'status_example'; // string | Only invoices with this status
$limit = 50; // int | Maximum number of invoices to return
$offset = 0; // int | Number of invoices to skip

try {
    $result = $apiInstance->getInvoicesByPartnerId_0($partner_id, $status, $limit, $offset);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling InvoicesApi->getInvoicesByPartnerId_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose invoices to list | |
| **status** | **string**| Only invoices with this status | [optional] |
| **limit** | **int**| Maximum number of invoices to return | [optional] [default to 50] |
| **offset** | **int**| Number of invoices to skip | [optional] [default to 0] |

### Return type

[**\WidgeticApi\Model\GetInvoicesByPartnerId200Response**](../Model/GetInvoicesByPartnerId200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
