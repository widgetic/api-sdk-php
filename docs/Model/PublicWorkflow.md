# # PublicWorkflow

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**workflow_id** | **string** |  |
**status** | **string** |  |
**version_id** | **string** | The published version this answer is for. A visitor who starts on it finishes on it. | [optional]
**version_number** | **int** |  | [optional]
**published_at** | **\DateTime** |  | [optional]
**start_composition_id** | **string** | The composition a new visitor starts on, so the page can show it while the graph is still being read. | [optional]
**timezone** | **string** | The zone date and time triggers are read in. | [optional]
**graph** | [**\WidgeticApi\Model\WorkflowGraph**](WorkflowGraph.md) |  | [optional]
**translations** | [**array<string,\WidgeticApi\Model\PublicWorkflowTranslation>**](PublicWorkflowTranslation.md) | The languages the compositions of the graph can be shown in, by composition id: only the compositions that have an active translation with a language besides their own, so the field is absent when none has. The browser shows the copy in the visitor&#39;s language in place of the composition, at the first step and at every move, with the rules &#x60;&lt;widgetic-translations&gt;&#x60; follows (the visitor&#39;s language, then its language family, then the language the composition was written in). It is read when the answer is made, not when the version was published, so a language added to a translation reaches visitors without a new publish. Ids, counts and the visitor&#39;s place keep naming the composition of the graph, never its copy. | [optional]
**event_token** | **string** | What lets the browser report counts for this version, valid for 24 hours. Absent when this server cannot sign one, and the browser then reports nothing. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
