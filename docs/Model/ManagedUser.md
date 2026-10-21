# # ManagedUser

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique identifier for the managed user |
**manager_id** | **string** | ID of the user who manages this managed user |
**external_id** | **string** | Your own identifier for the managed user. Unique among the managed users you manage (two different partners may use the same value). |
**metadata** | **object** | Additional metadata for the managed user | [optional]
**is_active** | **bool** | Whether new compositions, widgets and uploads can be filed under this managed user. &#x60;false&#x60; means it has been switched off (&#x60;updateManagedUser&#x60; with &#x60;is_active: false&#x60;): what it already has stays, and filing anything new under it answers &#x60;409 MANAGED_USER_INACTIVE&#x60;. A record from before the switch existed may answer &#x60;null&#x60;, which counts as on. | [optional]
**created_at** | **\DateTime** | Timestamp when the managed user was created |
**updated_at** | **\DateTime** | Timestamp when the managed user was last updated |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
