# # UploadLimits

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**multipart_max_bytes** | **int** | The largest file &#x60;uploadsPost&#x60; takes in one request, in bytes. The same for every account. | [optional]
**multipart_mime_types** | **string[]** | The file types &#x60;uploadsPost&#x60; takes for media (&#x60;content-property&#x60; uploads) | [optional]
**tus_enabled** | **bool** | Whether resumable uploads are switched on. They need a signed-in session; an API key uses &#x60;uploadsPost&#x60;. | [optional]
**tus_max_bytes** | **int** | The largest file a resumable upload takes, in bytes (250 MB by default). The same for every account, whatever its plan. A file over &#x60;multipart_max_bytes&#x60; goes through a resumable upload. | [optional]
**tus_chunk_size_bytes** | **int** | The chunk size resumable uploads are tuned for, in bytes. A client may send smaller or larger chunks. | [optional]
**tus_mime_types** | **string[]** |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
