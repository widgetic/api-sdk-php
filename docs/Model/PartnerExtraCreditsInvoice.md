# # PartnerExtraCreditsInvoice

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**invoice_id** | **string** | Stripe&#39;s id for the invoice. |
**number** | **string** | The number printed on the invoice, once Stripe has numbered it. |
**hosted_invoice_url** | **string** | The page where the invoice is viewed and paid. |
**pdf_url** | **string** | A PDF of the invoice. |
**credits** | **int** | The credits paying the invoice adds, once and for good. They do not expire. |
**credit_price_usd** | **float** | What one credit costs, in dollars. It is the list price, not the price of the contract. |
**amount_usd** | **float** | The price of those credits, in dollars, before tax. Never more than &#x60;usd&#x60; of the request. |
**tax_usd** | **float** | The tax added to the invoice, in dollars (0 when there is none). |
**total_usd** | **float** | What is paid, in dollars. The price plus the tax. |
**currency** | **string** | The currency of the invoice, in upper case (USD). |
**due_date** | **\DateTime** | When payment is due, as printed on the invoice. |
**due_days** | **int** | How many days there are to pay. |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
