# # UpdateComposition

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Updated name of the composition | [optional]
**widget_id** | **string** | Updated widget ID | [optional]
**content** | **object** | Updated content data | [optional]
**status** | **string** | Updated status | [optional]
**embed_settings** | **object** | Updated embed settings | [optional]
**design** | **object** | Updated design settings | [optional]
**database_schema** | **object** | Tables to make for the composition, in the shape &#x60;createComposition&#x60; takes (&#x60;{ \&quot;tables\&quot;: [ ... ] }&#x60;, with the same names, types, defaults and limits). Only the tables that are missing are made. A table that already exists is never changed or dropped: it keeps its columns, so a column added to the declaration is not added to it. A declaration that cannot be used is refused with &#x60;400&#x60; and &#x60;INVALID_DATABASE_SCHEMA&#x60;. When the composition is saved but its tables cannot be made just now, &#x60;meta.warnings&#x60; says so: send the same &#x60;databaseSchema&#x60; again to retry. | [optional]
**project_id** | **string** | Updated project ID | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
