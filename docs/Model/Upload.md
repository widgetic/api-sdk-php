# # Upload

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** |  |
**url** | **string** | The public address of the stored file |
**mime_type** | **string** | The type of the stored file. A HEIC or HEIF photo is stored as &#x60;image/jpeg&#x60;. |
**file_name** | **string** |  |
**file_size** | **int** | Size of the stored file, in bytes |
**width** | **int** | Width in pixels, for images | [optional]
**height** | **int** | Height in pixels, for images | [optional]
**storage_key** | **string** | Where the file sits in its storage bucket |
**context_type** | **string** | What the file was uploaded for. Media for widget content is &#x60;content-property&#x60;. |
**source** | **string** | Which part of the product, or which client, uploaded the file. &#x60;widget-visitor-upload&#x60; is a file a visitor sent through a widget&#39;s upload adapter; it cannot be asked for when uploading. |
**widget_id** | **string** |  | [optional]
**conversation_id** | **string** |  | [optional]
**managed_user_id** | **string** | The managed user the file was uploaded for, or null when it is the account&#39;s own. List one managed user&#39;s files with the &#x60;managed_user_id&#x60; or &#x60;managed_user_external_id&#x60; query parameter of &#x60;uploadsGet&#x60;. | [optional]
**purpose** | **string** | Where in the product the partner uses the file, or null when unknown | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
