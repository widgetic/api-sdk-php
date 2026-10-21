# # ManagedUserOperationUsage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**operation** | **string** | The metered operation, as the credit ledger names it |
**calls** | **int** | How many runs of the operation were paid for and kept (a run that was refunded is not one) |
**credits** | **int** | The credits those runs took from your account |
**refunded_calls** | **int** | How many runs were refunded (a generation that failed), and so are not in &#x60;calls&#x60; |
**refunded_credits** | **int** | The credits the refunded runs took, which went back to your account |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
