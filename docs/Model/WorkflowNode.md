# # WorkflowNode

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  |
**type** | **string** |  |
**position** | [**\WidgeticApi\Model\WorkflowNodePosition**](WorkflowNodePosition.md) |  | [optional]
**composition_id** | **string** | The composition a &#x60;composition&#x60; block shows. | [optional]
**starts_here** | **bool** | Set on the one composition block a visitor starts at. | [optional]
**trigger** | [**\WidgeticApi\Model\WorkflowTrigger**](WorkflowTrigger.md) |  | [optional]
**cases** | [**\WidgeticApi\Model\WorkflowConditionCase[]**](WorkflowConditionCase.md) | The rules of a &#x60;condition&#x60; block, in the order they are read. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
