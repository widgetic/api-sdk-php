# # OperationsIdGetResponseData

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The operation&#39;s identifier, the &#x60;operationId&#x60; the call that started it returned | [optional]
**type** | **string** | What the operation does | [optional]
**status** | **string** | Where the operation stands. &#x60;completed&#x60;, &#x60;failed&#x60; and &#x60;cancelled&#x60; are final | [optional]
**progress** | **int** | How far the operation has got, in percent | [optional]
**metadata** | **array<string,mixed>** | What the operation tells about its work. A finished composition duplication names the new composition in &#x60;newCompositionId&#x60;, and lists any problem with its database in &#x60;warnings&#x60; (absent when there is none). | [optional]
**error** | **string** | Why a &#x60;failed&#x60; operation failed (absent otherwise) | [optional]
**created_at** | **\DateTime** |  | [optional]
**updated_at** | **\DateTime** |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
