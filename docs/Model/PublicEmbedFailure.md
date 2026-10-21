# # PublicEmbedFailure

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  |
**message** | **string** | What happened, for a person. |
**code** | **string** | The short code a page branches on: &#x60;DOMAIN_NOT_ALLOWED&#x60;, &#x60;UNPUBLISHED&#x60;, &#x60;SUSPENDED&#x60;, &#x60;NOT_FOUND&#x60;, &#x60;RATE_LIMITED&#x60;, and for the entry route the codes listed with its answers. |
**details** | [**\WidgeticApi\Model\PublicEmbedFailureDetails**](PublicEmbedFailureDetails.md) |  | [optional]
**correlation_id** | **string** | The id of the request, for the routes that carry it. | [optional]
**error** | [**\WidgeticApi\Model\PublicEmbedFailureError**](PublicEmbedFailureError.md) |  |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
