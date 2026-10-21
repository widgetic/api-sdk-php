# # CompositionEntryAggregateTally

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**group** | **string** | The value of the &#x60;groupBy&#x60; column, as text (a number is &#x60;\&quot;5\&quot;&#x60;); &#x60;null&#x60; groups the entries that left it empty. Absent when no &#x60;groupBy&#x60; was asked for. | [optional]
**count** | **int** | How many entries are in the group (or in the selection) | [optional]
**avg** | **float** | The average of the numeric &#x60;column&#x60;, rounded to 4 decimals. &#x60;null&#x60; when no entry matched: there is no average of nothing, and it is not 0. | [optional]
**min** | **float** | The smallest value of the numeric &#x60;column&#x60;. &#x60;null&#x60; when no entry matched. | [optional]
**max** | **float** | The largest value of the numeric &#x60;column&#x60;. &#x60;null&#x60; when no entry matched. | [optional]
**sum** | **float** | The sum of the numeric &#x60;column&#x60;. &#x60;null&#x60; when no entry matched. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
