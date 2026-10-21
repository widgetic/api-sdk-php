# # ManagedUserEntryItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  |
**values** | **array<string,mixed>** |  |
**context** | **array<string,mixed>** | The host context the entry was stored with: what the embedding page passed in, without the two keys of a signature (&#x60;widgetic_exp&#x60; and &#x60;widgetic_sig&#x60;), which are checked when the entry comes in and are never stored. |
**created_at** | **\DateTime** |  |
**truncated_columns** | **string[]** | The columns whose value was cut: a value longer than 20,000 characters is cut there (a JSON value is cut as text, so it comes back as a string and no longer as an object), and its column is named here. Absent when nothing was cut. | [optional]
**composition_id** | **string** |  |
**table** | **string** |  |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
