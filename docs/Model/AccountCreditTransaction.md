# # AccountCreditTransaction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional]
**transaction_type** | **string** | What the entry did to the balance. &#x60;debit&#x60; is credits spent (this is how consumption shows), &#x60;credit&#x60; and &#x60;subscription&#x60; are credits added, &#x60;refund&#x60; returns credits that were spent, &#x60;reserve&#x60; and &#x60;release&#x60; move credits in and out of the reserved amount, and &#x60;adjustment&#x60;, &#x60;expiration&#x60;, &#x60;transfer_out&#x60; and &#x60;transfer_in&#x60; are the remaining ways a balance changes. The list can grow, so treat an unknown type as an entry you do not need to interpret. | [optional]
**amount** | **float** | Always positive. The &#x60;transactionType&#x60; says whether the credits were added or taken. | [optional]
**balance_after** | **float** | The balance once this entry was applied | [optional]
**description** | **string** |  | [optional]
**reference_id** | **string** | The event the entry belongs to. An entry is recorded once per reference. | [optional]
**created_at** | **\DateTime** |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
