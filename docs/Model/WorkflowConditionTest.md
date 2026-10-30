# # WorkflowConditionTest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**field** | [**\WidgeticApi\Model\WorkflowFieldReference**](WorkflowFieldReference.md) |  |
**operator** | **string** | Text fields take is, isNot, contains, doesNotContain, startsWith, endsWith, isEmpty and isNotEmpty. Number fields take is, isNot, greaterThan, atLeast, lessThan, atMost, isEmpty and isNotEmpty. Yes/no fields take is and isNot. |
**value** | **mixed** | What the field is compared with; not used by isEmpty and isNotEmpty. A text for a text field, a number for a number field, true or false for a yes/no field. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
