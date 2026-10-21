# # ContentItemWriteResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** | Repeats the envelope&#39;s &#x60;success&#x60;. | [optional]
**content_version** | **int** | The content&#39;s version after the write. Send it as &#x60;If-Match&#x60; on the next write to refuse a stale one. | [optional]
**validation_result** | [**\WidgeticApi\Model\ContentItemWriteResultValidationResult**](ContentItemWriteResultValidationResult.md) |  | [optional]
**composition_updated** | **bool** |  | [optional]
**realtime_update_sent** | **bool** | Whether the open frames were told to reload the content. | [optional]
**item** | **array<string,mixed>** | The item as stored, with the &#x60;id&#x60; the list gave it. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
