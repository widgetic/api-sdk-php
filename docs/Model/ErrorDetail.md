# # ErrorDetail

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **string** | Machine-readable error code. |
**message** | **string** | Human-readable explanation. |
**param** | **string** | The field that caused the error, when one did. | [optional]
**doc_url** | **string** | Where this error is explained. | [optional]
**suggested_action** | **string** | What to do about it. | [optional]
**retry_after** | **int** | Seconds to wait before trying again (rate limits). The same number is in the &#x60;Retry-After&#x60; header. | [optional]
**details** | **array<string,mixed>** | More about the error: the fields that failed, a limit that was reached. | [optional]
**correlation_id** | **string** | Quote this when you ask support about the call. | [optional]
**timestamp** | **\DateTime** |  |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
