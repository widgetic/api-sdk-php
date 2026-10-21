# # PartnerContract

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  | [optional]
**partner_id** | **string** |  | [optional]
**custom_price** | **float** | The agreed price per &#x60;billingCycle&#x60;; null when the standard price applies | [optional]
**custom_credits** | **int** | Credits received each billing period (&#x60;billingCycle&#x60;); null when the standard allowance applies | [optional]
**credit_price_usd** | **float** | The agreed price of one credit, in dollars; null when the list price applies | [optional]
**effective_credit_price_usd** | **float** | What one credit costs you, in dollars. The agreed price, or the list price when none was agreed | [optional]
**period_total_usd** | **float** | What one billing period costs, in dollars before tax, &#x60;customCredits&#x60; times &#x60;effectiveCreditPriceUsd&#x60;. Null while no credits were agreed | [optional]
**additional_features** | **string[]** | Features included beyond the standard partner plan | [optional]
**billing_cycle** | **string** |  | [optional]
**minimum_commitment_months** | **int** |  | [optional]
**support_sla** | **string** |  | [optional]
**contract_start_date** | **\DateTime** |  | [optional]
**contract_end_date** | **\DateTime** | Null when the contract runs until it is ended | [optional]
**is_active_contract** | **bool** | True while the contract is in force, that is when it is open-ended or today falls between its start and end | [optional]
**created_at** | **\DateTime** |  | [optional]
**updated_at** | **\DateTime** |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
