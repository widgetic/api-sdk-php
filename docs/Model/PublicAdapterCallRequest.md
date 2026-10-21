# # PublicAdapterCallRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**request_id** | **string** | Names this attempt: 8 to 64 characters, letters, digits, &#x60;_&#x60; and &#x60;-&#x60;, the first a letter or a digit (a UUID fits). A module makes a new one for each action of the visitor. An operation that costs credits is charged once for each &#x60;requestId&#x60;, so a repeat of one that was charged and not given back is refused (409 &#x60;REQUEST_ALREADY_USED&#x60;) and does no work. |
**version** | **int** | The version of the adapter the widget&#39;s code was built against (the &#x60;vN&#x60; of its import). When it is left out, the newest version the widget&#39;s live manifest lists. | [optional]
**input** | **array<string,mixed>** | What the operation is asked to do. Each operation says what it accepts and answers 400, 413 or 422 with a code of its own for what it cannot use. Defaults to an empty object. | [optional]
**context** | **array<string,mixed>** | The host context the embedding page gave the widget, as the entry route takes it (see the description of &#x60;createPublicCompositionEntry&#x60;, with its **Signed context**). It is not authenticated unless the partner signs it. At most 4096 bytes of JSON, the two signature keys included. | [optional]
**captcha_token** | **string** | The visitor&#39;s CAPTCHA token, for an operation that asks for one (the answer &#x60;CAPTCHA_REQUIRED&#x60; says so). | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
