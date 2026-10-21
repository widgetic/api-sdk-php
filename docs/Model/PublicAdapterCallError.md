# # PublicAdapterCallError

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**success** | **bool** |  |
**error** | **string** | A sentence a visitor may read. It never says why a feature is unavailable: not that its owner is out of credits, not what a balance is, not which limit was reached beyond the word &#x60;RATE_LIMITED&#x60; or &#x60;WIDGET_LIMIT_REACHED&#x60;. (On a 429 the standard rate-limit envelope is sent instead: &#x60;error&#x60; is then an object, and &#x60;code&#x60; beside it is the flat code.) |
**code** | **string** | What a module switches on. The codes of the gateway itself are &#x60;ADAPTER_BODY_INVALID&#x60;, &#x60;CAPTCHA_REQUIRED&#x60;, &#x60;ADAPTER_NOT_AVAILABLE&#x60;, &#x60;REQUEST_ALREADY_USED&#x60;, &#x60;RATE_LIMITED&#x60;, &#x60;WIDGET_LIMIT_REACHED&#x60;, &#x60;ADAPTER_FAILED&#x60;, &#x60;ADAPTER_UNAVAILABLE&#x60; and &#x60;ADAPTER_TIMEOUT&#x60;, with &#x60;ORIGIN_NOT_ALLOWED&#x60;, &#x60;PAYLOAD_TOO_LARGE&#x60;, &#x60;UNSUPPORTED_MEDIA_TYPE&#x60;, &#x60;CONTEXT_SIGNATURE_REQUIRED&#x60;, &#x60;CONTEXT_SIGNATURE_INVALID&#x60;, &#x60;CONTEXT_SIGNATURE_EXPIRED&#x60;, &#x60;CONTEXT_SIGNATURE_UNAVAILABLE&#x60; and the codes of the serving gate (&#x60;NOT_FOUND&#x60;, &#x60;UNPUBLISHED&#x60;, &#x60;SUSPENDED&#x60;) it shares with the other public embed routes. An operation may add codes of its own (capital letters and &#x60;_&#x60;) for an input it refused. |
**correlation_id** | **string** | Quote it when asking for help with a call. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
