# # CompositionEntryAggregatesBlock

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**column** | **string** | The numeric column &#x60;avg&#x60;, &#x60;min&#x60;, &#x60;max&#x60; and &#x60;sum&#x60; were computed over. An empty text when only &#x60;count&#x60; was asked for. |
**tallies** | [**\WidgeticApi\Model\CompositionEntryAggregateTally[]**](CompositionEntryAggregateTally.md) | One tally per value of &#x60;groupBy&#x60;, in the order of that column (a number as a number, &#x60;null&#x60; last), up to 200 groups; or ONE tally for the whole selection when no &#x60;groupBy&#x60; was asked for. Empty when &#x60;groupBy&#x60; was asked for and no entry matched. |
**truncated** | **bool** | True when more than 200 groups matched, so &#x60;tallies&#x60; lists the first 200 in that order. Absent otherwise. (Not to be mixed up with &#x60;moreGroups&#x60; on the reading, which is about the plain &#x60;tallies&#x60; of the whole table: those are 20 groups, largest first.) | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
