# # CompositionEntriesDescription

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**composition_id** | **string** | The composition whose entries these are |
**has_data** | **bool** | False when the composition keeps no entries of its own: its widget only shows content (it has no database), or nothing was set up in the database yet. That is not an error. |
**tables** | [**\WidgeticApi\Model\CompositionEntryTable[]**](CompositionEntryTable.md) | The tables entries are kept in (up to 20) |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
