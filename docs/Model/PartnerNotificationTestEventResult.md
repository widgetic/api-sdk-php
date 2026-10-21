# # PartnerNotificationTestEventResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**delivered** | **bool** | True when your receiver answered with a 2xx status. |
**status_code** | **int** | The HTTP status your receiver answered with. Null when it did not answer (refused, unreachable or too slow). |
**duration_ms** | **int** | How long the call took, in milliseconds. A call is given up after ten seconds. |
**error** | **string** | Why the call did not arrive, in a few words (&#x60;timeout&#x60;, &#x60;status 500&#x60;, &#x60;unreachable&#x60;, a redirect). Never what your receiver replied. Left out when it arrived. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
