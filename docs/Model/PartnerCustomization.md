# # PartnerCustomization

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique identifier for the customization | [optional]
**partner_id** | **string** | ID of the partner this customization belongs to | [optional]
**custom_price** | **float** | Custom monthly price override | [optional]
**custom_credits** | **float** | Credits the partner receives each billing period (&#x60;billingCycle&#x60;). What a period costs is derived from it, see &#x60;periodTotalUsd&#x60; | [optional]
**credit_price_usd** | **float** | What the partner pays for one credit, in dollars (up to four decimals). Null means the list price | [optional]
**effective_credit_price_usd** | **float** | What one credit costs the partner, in dollars. &#x60;creditPriceUsd&#x60; when the contract names one, the list price otherwise | [optional]
**period_total_usd** | **float** | What one billing period costs, in dollars before tax. &#x60;customCredits&#x60; times &#x60;effectiveCreditPriceUsd&#x60;; null while the contract names no credits | [optional]
**additional_features** | **string[]** | Additional features beyond base partner plan | [optional]
**billing_cycle** | **string** | Billing cycle for the customization | [optional]
**minimum_commitment_months** | **float** | Minimum commitment period in months | [optional]
**support_sla** | **string** | Support SLA percentage | [optional]
**contract_start_date** | **\DateTime** | Contract start date | [optional]
**contract_end_date** | **\DateTime** | Contract end date | [optional]
**notes** | **string** | Admin notes about the customization | [optional]
**is_active_contract** | **bool** | Whether the contract is currently active | [optional]
**created_at** | **\DateTime** | Creation timestamp | [optional]
**updated_at** | **\DateTime** | Last update timestamp | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
