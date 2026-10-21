# # PartnerStorageDestination

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**partner_id** | **string** |  |
**endpoint** | **string** | The HTTPS address of the S3-compatible service, scheme and host only |
**region** | **string** |  |
**bucket** | **string** |  |
**key_prefix** | **string** | The folder inside the bucket every file is written under. Empty, or folders each followed by a slash. |
**public_base_url** | **string** | Where the stored files are served from. A file&#39;s url is this address, a slash and the file&#39;s key. |
**force_path_style** | **bool** | Whether the bucket name goes in the path of a request (true) or in the host name (false) |
**access_key_hint** | **string** | The last four characters of the access key id, to tell which key is set. Not enough to use it. |
**verified_at** | **\DateTime** | When the destination last passed the check |
**last_verification_error** | **string** | Why the most recent re-check failed. Null while the last check passed. | [optional]
**last_verification_failed_at** | **\DateTime** |  | [optional]
**updated_at** | **\DateTime** |  |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
