# # AccountCreditBalance

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional]
**user_id** | **string** |  | [optional]
**balance** | **float** | Credits the account holds | [optional]
**reserved_balance** | **float** | Credits committed to an operation that is still running. They cannot be spent, so what a new operation can use is &#x60;balance - reservedBalance&#x60;. | [optional]
**last_updated** | **\DateTime** |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
