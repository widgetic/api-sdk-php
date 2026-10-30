# # Workflow

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  |
**name** | **string** |  |
**managed_user_id** | **string** | The customer of a partner (a managed user) this workflow was made for, or null when it is its workspace&#39;s own. A customer&#39;s editor session lists and opens only the workflows filed under that customer; the partner&#39;s own account sees every customer&#39;s and tells them apart by this. It is set when the workflow is made and never changes. | [optional]
**status** | [**\WidgeticApi\Model\WorkflowStatus**](WorkflowStatus.md) |  |
**revision** | **int** | Rises by one with every save. A save, a publish, a discard and a restore each name the revision they started from. |
**unpublished_changes** | **bool** | Whether the draft differs from the live version. |
**composition_ids** | **string[]** |  |
**block_count** | **int** |  |
**timezone** | **string** | The zone date and time triggers are read in (stored as UTC). |
**runs_count** | **int** | Visitors who started the workflow, over its whole life. |
**live_version_id** | **string** |  | [optional]
**created_at** | **\DateTime** |  |
**updated_at** | **\DateTime** |  |
**first_published_at** | **\DateTime** |  | [optional]
**last_published_at** | **\DateTime** |  | [optional]
**paused_at** | **\DateTime** |  | [optional]
**archived_at** | **\DateTime** |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
