# # PartnerInvoice

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional]
**partner_id** | **string** |  | [optional]
**number** | **string** | The number printed on the invoice, once it has been issued | [optional]
**description** | **string** | What the invoice is for | [optional]
**amount** | **float** | Total, in dollars. The price plus the tax (the same number as &#x60;total&#x60;) | [optional]
**subtotal** | **float** | The price, before tax, in dollars | [optional]
**tax_amount** | **float** | The tax on the price, in dollars. 0 when there is none, for example under the EU reverse charge | [optional]
**total** | **float** | What the partner pays, in dollars. The price plus the tax | [optional]
**amount_due** | **float** | What is still owed, in dollars | [optional]
**amount_paid** | **float** | What has been paid, in dollars | [optional]
**currency** | **string** |  | [optional]
**failure_reason** | **string** | Why the last attempt to pay failed, in the payment provider&#39;s words for the card holder. Null unless the status is &#x60;failed&#x60;; the invoice stays payable from &#x60;hostedInvoiceUrl&#x60; | [optional]
**status** | **string** | &#x60;open&#x60; waits for payment, &#x60;failed&#x60; waits for payment after an attempt was refused, &#x60;paid&#x60; is settled (a payment received outside the payment provider counts), &#x60;void&#x60; was cancelled and owes nothing, and &#x60;uncollectible&#x60; was written off | [optional]
**invoice_date** | **\DateTime** |  | [optional]
**due_date** | **\DateTime** |  | [optional]
**paid_date** | **\DateTime** |  | [optional]
**period_start** | **\DateTime** |  | [optional]
**period_end** | **\DateTime** |  | [optional]
**payment_method** | **string** | How it was paid, once it was | [optional]
**hosted_invoice_url** | **string** | The page where the invoice can be viewed and paid, once it has been issued | [optional]
**pdf_url** | **string** | A PDF of the invoice, once it has been issued | [optional]
**line_items** | **array<string,mixed>[]** |  | [optional]
**created_at** | **\DateTime** |  | [optional]
**updated_at** | **\DateTime** |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
