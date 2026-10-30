# # WorkflowStats

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**workflow_id** | **string** |  |
**version_id** | **string** | The version counted, or null when all versions are. | [optional]
**from** | **string** | First UTC day counted (YYYY-MM-DD). |
**to** | **string** | Last UTC day counted (YYYY-MM-DD). |
**started** | **int** | Visitors who started the workflow in the range; null when all versions are counted. | [optional]
**nodes** | [**\WidgeticApi\Model\WorkflowCounter[]**](WorkflowCounter.md) | Visitors who reached each block. |
**edges** | [**\WidgeticApi\Model\WorkflowCounter[]**](WorkflowCounter.md) | Visitors who took each connection. |
**failed** | [**\WidgeticApi\Model\WorkflowCounter[]**](WorkflowCounter.md) | Times moving on to a block failed (it did not load in time) and the visitor stayed. |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
