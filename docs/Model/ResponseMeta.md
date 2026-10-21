# # ResponseMeta

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** | The page that was read, counting from 1. | [optional]
**size** | **int** | How many items one page holds. | [optional]
**total** | **int** | How many items the whole list has. | [optional]
**limit** | **int** | The same as &#x60;size&#x60;. | [optional]
**offset** | **int** | How many items come before this page. | [optional]
**has_next_page** | **bool** |  | [optional]
**has_previous_page** | **bool** |  | [optional]
**next_cursor** | **string** | Pass this as &#x60;cursor&#x60; to read the next page of a list that is read by cursor. &#x60;null&#x60; on the last page. | [optional]
**warnings** | **string[]** | Things the call did not do, though it succeeded (for example a table that could not be created just now). | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
