# # GetCompositionEmbedSchemaResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Identifier of the schema | [optional]
**name** | **string** |  | [optional]
**version** | **string** | Version of the schema; it changes when a setting is added, removed or retyped | [optional]
**type** | **string** | The tab this schema describes | [optional]
**component_groups** | **object[]** | The controls of the Embed tab, grouped as the editor shows them | [optional]
**defaults** | **array<string,mixed>** | The value of every setting that declares one, by setting name. A value is a boolean, a number or a string, as the setting&#39;s &#x60;type&#x60; says. (Written as an open map, not as a choice of three types: a generated client cannot be built from a choice between plain types.) | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
