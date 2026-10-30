# # Widget

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique identifier for the widget. | [optional]
**creator_id** | **string** | ID of the user who created the widget. | [optional]
**name** | **string** | Name of the widget. | [optional]
**description** | **string** | Description of the widget&#39;s purpose and functionality. | [optional]
**type** | **string** | Type of widget (e.g., chart, form, gallery). | [optional]
**content** | **array<string,mixed>** | Content configuration for the widget. | [optional]
**is_public** | **bool** | Whether the widget is publicly available. | [optional]
**is_draft** | **bool** | Whether the widget is a draft. | [optional]
**share_id** | **string** | Unique ID for sharing the widget publicly. | [optional]
**created_at** | **\DateTime** | When the widget was created. | [optional]
**updated_at** | **\DateTime** | When the widget was last updated. | [optional]
**js_path** | **string** | Path to the JavaScript file for this widget. | [optional]
**canvas_id** | **string** | ID of the canvas associated with this widget. | [optional]
**repo_id** | **string** | Repository identifier for source code. | [optional]
**database_id** | **string** | Legacy. The name of a Neon database that an earlier version made for this widget. A widget has no database now (what the visitors of a composition leave is kept in the tables of that composition), so widgets made now have none. | [optional]
**version** | **float** | Version number of the widget. | [optional]
**last_commit_sha** | **string** | Latest Git commit SHA of the widget&#39;s code repository. | [optional]
**organization_id** | **string** | Organization ID if created in an organization workspace. | [optional]
**project_folder** | **string** | Project folder reference for organization widgets. | [optional]
**workspace_type** | **string** | Workspace type when created. | [optional]
**managed_user_id** | **string** | The managed user the widget was made for, or null when it is your own. List one managed user&#39;s widgets with the &#x60;managedUserId&#x60; or &#x60;managedUserExternalId&#x60; query parameter of &#x60;getWidgets&#x60;. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
