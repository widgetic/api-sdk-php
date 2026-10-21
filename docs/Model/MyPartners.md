# # MyPartners

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**standing** | **string** | The standing of the account as a whole, the word every gate reads: &#x60;not_a_partner&#x60; when the account administers no partner; otherwise &#x60;active&#x60; when any of its partners is in force, else &#x60;payment_arrears&#x60; when the partners that are active each have a contract invoice that is past its due date and unpaid, else &#x60;suspended&#x60; when any is paused, else &#x60;inactive&#x60;. &#x60;payment_arrears&#x60; is not set by anybody: it stops the same things a pause stops (billing, invoices, credits and the other routes a partner needs to pay stay open) and ends by itself the moment the invoice is paid. |
**overdue_since** | **\DateTime** | When the oldest overdue contract invoice was due; null unless &#x60;standing&#x60; is &#x60;payment_arrears&#x60;. Pay the invoices in the list of &#x60;GET /invoices/partner/{partnerId}&#x60; that are past their due date to end it. |
**partners** | [**\WidgeticApi\Model\MyPartner[]**](MyPartner.md) | The partners the account administers (nearly always one), the oldest first |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
