# # PartnerBillingOverviewOperationalCredits

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**balance** | **float** | Credits the account holds |
**reserved_balance** | **float** | Credits committed to an operation that is still running. Not spendable. |
**available_balance** | **float** | What a new operation can use (&#x60;balance&#x60; minus &#x60;reservedBalance&#x60;, never below 0) |
**recent_transactions** | [**\WidgeticApi\Model\AccountCreditTransaction[]**](AccountCreditTransaction.md) | The ten newest ledger entries, newest first |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
