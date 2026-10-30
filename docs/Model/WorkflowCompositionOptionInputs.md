# # WorkflowCompositionOptionInputs

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  |
**reason** | **string** | Why Input added is not available. widget_keeps_no_data means the composition declares no table a visitor&#39;s entries are written to; widget_not_published means the widget has no published version. | [optional]
**tables** | **string[]** | Every table a visitor&#39;s entries are written to, including one with no field a rule may read. |
**fields** | [**\WidgeticApi\Model\WorkflowCompositionField[]**](WorkflowCompositionField.md) | The columns of those tables a rule may read. Not offered are id and created_at, columns that are not text, a number or yes/no, and columns whose name says they hold a person&#39;s private details (an email, a phone number), because a value a rule reads is handed to the visitor&#39;s page. |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
