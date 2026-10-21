# # PublicCompositionEntryRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**values** | **array<string,mixed>** | Column values to insert (never id or time columns). |
**context** | **object** | Host attribution from the embedding page. It is not authenticated unless the partner signs it (see the description of this operation): never use it for authorization on its own. At most 20 keys; string values up to 500 characters or finite numbers; 2048 bytes JSON total. A signed context carries two more keys, &#x60;widgetic_exp&#x60; and &#x60;widgetic_sig&#x60;: the gateway checks them and drops them, so they are neither stored nor announced. | [optional]
**write_token** | **string** | Optional per-composition write token (&#x60;entries.writeToken&#x60; from &#x60;widgetic:host&#x60;, or &#x60;entryWriteToken&#x60; from &#x60;GET /embed/compositions/{compositionId}&#x60;) when not passed in the &#x60;X-Widgetic-Write-Token&#x60; header. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
