# # NewWidget

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Name of the widget. |
**type** | **string** | What kind of widget this is, as a label of your choosing (for example chart, form, gallery). |
**content** | **array<string,mixed>** | Starting content for the widget. An empty object is fine. |
**is_public** | **bool** | Whether the widget is public. | [optional] [default to false]
**is_draft** | **bool** | Whether the widget starts as a draft. A widget created without this is a draft. | [optional] [default to true]
**canvas_id** | **string** | Put the widget on this existing canvas instead of a new one. You must own the canvas. | [optional]
**project_id** | **string** | Project to file the widget in. You must be able to edit the project. | [optional]
**organization_id** | **string** | Organization the widget belongs to. You must be a member who may create widgets there. | [optional]
**workspace_type** | **string** | Whether the widget lives in your personal workspace or in an organization&#39;s. | [optional]
**managed_user_id** | **string** | Make the widget for one of your managed users, by Widgetic&#39;s id for the user. Send this or &#x60;managedUserExternalId&#x60;, not both. The managed user must be yours and active. The widget stays in your account; the tag lets you list one user&#39;s widgets and keeps it out of the others&#39; lists. It is set here and does not change afterwards. | [optional]
**managed_user_external_id** | **string** | The same, by your own identifier for the user, the &#x60;externalId&#x60; you gave when you created the managed user (answers show it as &#x60;externalId&#x60;). Send this or &#x60;managedUserId&#x60;, not both. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
