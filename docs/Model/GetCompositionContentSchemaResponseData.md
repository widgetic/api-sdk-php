# # GetCompositionContentSchemaResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**version** | **string** |  | [optional]
**widget_type** | **string** |  | [optional]
**type** | **string** |  | [optional]
**content** | **object** | Widget-wide fields; enriched properties may include &#x60;role&#x60; and &#x60;roleSource&#x60;. AI-built widgets keep their widget-wide fields in &#x60;genericContent&#x60;, as a list of properties, instead | [optional]
**content_items** | **object** | Repeating list schema; list-level &#x60;role&#x60; is &#x60;list&#x60;; item fields use semantic roles. AI-built widgets store an array of default items instead, each repeating the same fields with their roles, and no list-level &#x60;role&#x60; | [optional]
**metadata** | **object** |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
