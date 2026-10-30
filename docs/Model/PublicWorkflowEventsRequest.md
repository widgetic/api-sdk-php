# # PublicWorkflowEventsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**version_id** | **string** |  |
**token** | **string** | The &#x60;eventToken&#x60; of the workflow, read for the same version. |
**events** | [**\WidgeticApi\Model\PublicWorkflowEventsRequestEventsInner[]**](PublicWorkflowEventsRequestEventsInner.md) | The counts of what visitors did. At least one of &#x60;events&#x60; and &#x60;heights&#x60; is needed. | [optional]
**heights** | [**\WidgeticApi\Model\PublicWorkflowEventsRequestHeightsInner[]**](PublicWorkflowEventsRequestHeightsInner.md) | How tall steps of this version settled in the visitor&#39;s browser, so that the embed code of the workflow can start its box at the height visitors saw instead of a guess. The Embed SDK sends one for a visitor who has no remembered height for the step. The gateway keeps the latest few for each composition (the median is what the code gets); a composition that this version does not show is left out. At least one of &#x60;events&#x60; and &#x60;heights&#x60; is needed. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
