# # Entitlement

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique identifier for the entitlement | [optional]
**user_id** | **string** | ID of the user (if user-level entitlement) | [optional]
**partner_id** | **string** | ID of the partner (if partner-level entitlement) | [optional]
**managed_user_id** | **string** | ID of the managed user (if managed user-level entitlement) | [optional]
**feature** | **string** | Feature identifier that this entitlement grants access to | [optional]
**value** | **string** | Value or limit for this feature | [optional]
**expires_at** | **\DateTime** | When this entitlement expires (null for permanent) | [optional]
**source** | **string** | Source of the entitlement | [optional]
**source_id** | **string** | ID of the source object that granted this entitlement | [optional]
**created_at** | **\DateTime** | When the entitlement was created | [optional]
**updated_at** | **\DateTime** | When the entitlement was last updated | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
