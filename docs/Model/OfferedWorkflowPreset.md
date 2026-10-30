# # OfferedWorkflowPreset

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**key** | **string** | The name your code and the picker use for the starting point. |
**workflow_id** | **string** | The workflow it is made from. What people get is its live version as it is when they start. |
**title** | **string** | What the picker shows. Null means show the workflow&#39;s name. |
**description** | **string** |  |
**position** | **int** | The list is ordered by this, smallest first, then by key. |
**available** | **bool** | Whether people can start from it now. A starting point that is not available is not shown to anyone, and says why. |
**unavailable_reason** | **string** | Why it is not available. &#x60;workflow_missing&#x60;: the workflow was deleted. &#x60;workflow_not_own&#x60;: it is no longer a workflow of your own. &#x60;workflow_archived&#x60;: unarchive it. &#x60;workflow_not_published&#x60;: it has no live version. &#x60;workflow_empty&#x60;: it shows no composition. &#x60;composition_not_own&#x60;: a block shows a composition made for a customer or a team. &#x60;too_many_widgets&#x60;: it chains more than 10 widgets. &#x60;widget_not_preset&#x60;: a widget it chains is no longer offered as a preset. |
**workflow_name** | **string** | The workflow&#39;s name. Null when the workflow is gone. |
**block_count** | **int** | How many blocks its live version has. Null when it is not available. |
**widgets** | [**\WidgeticApi\Model\OfferedWorkflowPresetWidget[]**](OfferedWorkflowPresetWidget.md) | The widgets it chains, once each, in the order they first appear. Empty when it is not available. |
**created_at** | **\DateTime** |  |
**updated_at** | **\DateTime** |  |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
