# # SetPartnerStorageDestinationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**endpoint** | **string** | The HTTPS address of the S3-compatible service, scheme and host only (no path, port or credentials). It must be a host name, not an IP address, and must resolve to the public internet. |
**region** | **string** | The region the service signs requests for. Use auto where the service says so (such as Cloudflare R2). |
**bucket** | **string** |  |
**key_prefix** | **string** | A folder inside the bucket to write every file under, for example widgetic/uploads. Folders are made of letters, digits, dots, hyphens and underscores. Leave it out to write at the root of the bucket. | [optional] [default to '']
**public_base_url** | **string** | Where the stored files are served from: the bucket&#39;s public address, or a CDN in front of it. The address of a file is this value, a slash and the file&#39;s key in the bucket, which starts with the key prefix. A path is allowed (https://media.example.com/files/acme-widget-media). |
**force_path_style** | **bool** | Put the bucket name in the path of a request. Every S3-compatible service supports this; set it to false only for a service that needs the bucket name in the host name. | [optional] [default to true]
**access_key_id** | **string** | The id of an access key that may put objects into the bucket |
**secret_access_key** | **string** | The secret of that access key. It is stored encrypted and is never returned. |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
