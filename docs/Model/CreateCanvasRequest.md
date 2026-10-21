# # CreateCanvasRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**persistence_key** | **string** | Key used for persistent storage and reference |
**canvas_content** | **object** | JSON content of the canvas, containing layout and configuration | [optional]
**primary_widget_id** | **string** | Optional primary widget id (usually set after widget create) | [optional]
**managed_user_id** | **string** | Make the canvas for this managed user (Widgetic&#39;s id for the user). Send this or &#x60;managedUserExternalId&#x60;, not both. The tag is set here and does not change afterwards. | [optional]
**managed_user_external_id** | **string** | Make the canvas for the managed user you registered with this &#x60;externalId&#x60; (your own identifier for the user). Send this or &#x60;managedUserId&#x60;, not both. | [optional]
**project_id** | **string** | Project this canvas belongs to. Empty canvases show on that project&#39;s list. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
