# # UpdateManagedUser

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**external_id** | **string** | Updated external identifier for the managed user. Must be unique among the managed users you manage (409 otherwise). | [optional]
**metadata** | **object** | Updated additional metadata for the managed user | [optional]
**is_active** | **bool** | Switch the managed user off (&#x60;false&#x60;) or back on (&#x60;true&#x60;). A managed user that is off keeps everything already filed under it, and that content can still be listed, but nothing new can be filed under it (&#x60;409 MANAGED_USER_INACTIVE&#x60;). Send a real boolean, not the text \&quot;false\&quot;. Switching a managed user off also ends all of its editor sessions. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
