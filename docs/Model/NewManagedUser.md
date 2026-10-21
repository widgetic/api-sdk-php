# # NewManagedUser

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**external_id** | **string** | Your own identifier for the managed user. Must be unique among the managed users you manage (409 otherwise); another partner using the same value does not matter. |
**manager_id** | **string** | ID of the user who will manage this managed user. Defaults to your own user ID; a partner can only use their own ID (403 otherwise), only an admin can name another manager. | [optional]
**metadata** | **object** | Additional metadata for the managed user | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
