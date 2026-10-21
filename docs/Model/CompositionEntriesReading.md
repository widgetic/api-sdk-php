# # CompositionEntriesReading

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**composition_id** | **string** | The composition whose entries these are |
**table** | **string** | The table that was read |
**total_rows** | **int** | How many entries the table holds in all. Not narrowed by &#x60;since&#x60;, &#x60;until&#x60; or a filter: only &#x60;aggregates&#x60; is. |
**tallies** | [**\WidgeticApi\Model\CompositionEntryTally[]**](CompositionEntryTally.md) | How many entries have each value of the &#x60;groupBy&#x60; column, largest group first (up to 20 groups), over the whole table. &#x60;null&#x60; when no &#x60;groupBy&#x60; was asked for. For the groups of a selection (a time window, a &#x60;context&#x60; filter) or for more than 20 groups, ask for &#x60;aggregate&#x60;: &#x60;aggregates.tallies&#x60; holds up to 200 groups. |
**more_groups** | **bool** | True when the &#x60;groupBy&#x60; column has more than the 20 groups &#x60;tallies&#x60; lists. It speaks of &#x60;tallies&#x60; only: &#x60;aggregates.truncated&#x60; is the same signal for &#x60;aggregates&#x60; (200 groups). |
**columns** | **string[]** | The name of each value of an entry in &#x60;rows&#x60;, in order, exactly as the database spells it (and as &#x60;describeCompositionEntries&#x60; lists it: &#x60;created_at&#x60; stays &#x60;created_at&#x60;). Empty when no entries were asked for, or the table has none. |
**rows** | **mixed[][]** | The newest entries, newest first (up to 25). &#x60;null&#x60; when no entries were asked for. Each entry is a list of values in the order of &#x60;columns&#x60;. A value is text (cut to 200 characters), a number, a boolean or &#x60;null&#x60;. |
**more_rows** | **bool** | True when the table holds more entries than &#x60;rows&#x60; lists |
**aggregates** | [**\WidgeticApi\Model\CompositionEntryAggregatesBlock**](CompositionEntryAggregatesBlock.md) | Only present when the read asked for &#x60;aggregate&#x60;. Unlike &#x60;totalRows&#x60;, &#x60;tallies&#x60; and &#x60;rows&#x60;, it is narrowed by &#x60;since&#x60;, &#x60;until&#x60; and the &#x60;context&#x60; and column filters of the same call: it answers \&quot;the average rating this week\&quot; where &#x60;tallies&#x60; answer \&quot;how many of each rating, ever\&quot;. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
