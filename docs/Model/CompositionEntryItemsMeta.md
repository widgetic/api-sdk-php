# # CompositionEntryItemsMeta

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**next_cursor** | **string** | Pass it as &#x60;cursor&#x60; to get the next page. &#x60;null&#x60; on the last page, and for a table that cannot be paged (see &#x60;paging&#x60;). |
**total** | **int** | How many entries match the filters and the &#x60;since&#x60; / &#x60;until&#x60; window, over all pages and not only this one. |
**paging** | **string** | Present, as &#x60;unavailable&#x60;, when the table cannot be paged: it has a time column but no id column to tell two entries of the same instant apart, or it has no time column and no id column that can be paged on. The answer is one page only, and &#x60;nextCursor&#x60; stays &#x60;null&#x60; even when &#x60;total&#x60; is larger than the page. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
