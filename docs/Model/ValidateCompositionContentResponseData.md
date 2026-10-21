# # ValidateCompositionContentResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**valid** | **bool** | False when there is at least one error. Warnings do not change it. |
**errors** | [**\WidgeticApi\Model\ContentCheckFinding[]**](ContentCheckFinding.md) | What is wrong, at most 100. Absent when &#x60;valid&#x60; is true. | [optional]
**warnings** | [**\WidgeticApi\Model\ContentCheckFinding[]**](ContentCheckFinding.md) | What is worth a look but does not stop the content from being saved, at most 100. | [optional]
**sanitized_content** | **array<string,mixed>** | The body as it was sent; nothing is changed. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
