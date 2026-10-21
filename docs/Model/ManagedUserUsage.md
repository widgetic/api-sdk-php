# # ManagedUserUsage

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**managed_user_id** | **string** |  |
**managed_user_external_id** | **string** | Your own identifier for the managed user |
**from** | **\DateTime** | Start of the period, included |
**to** | **\DateTime** | End of the period, not included |
**totals** | [**\WidgeticApi\Model\ManagedUserUsageTotals**](ManagedUserUsageTotals.md) |  |
**operations** | [**\WidgeticApi\Model\ManagedUserOperationUsage[]**](ManagedUserOperationUsage.md) | One entry for each operation that was paid for in the period, in alphabetical order |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
