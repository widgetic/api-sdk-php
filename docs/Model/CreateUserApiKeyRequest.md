# # CreateUserApiKeyRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | A name for the key, to tell it from the account&#39;s other keys |
**expires_at** | **\DateTime** | When the key stops working, as a date and time in the future with a zone. Omit it for a key that does not expire | [optional]
**preset** | **string** | A ready-made list of scopes. &#x60;read_only&#x60; looks at everything the account holds and changes nothing. &#x60;content&#x60; builds and manages widgets and compositions and runs the AI, and touches no billing, no people and no partners. &#x60;full_access&#x60; is the same as sending neither &#x60;preset&#x60; nor &#x60;scopes&#x60;. Send either &#x60;preset&#x60; or &#x60;scopes&#x60;, not both | [optional]
**scopes** | [**\WidgeticApi\Model\ApiKeyScope[]**](ApiKeyScope.md) | What the key may do, when a preset is not enough. Naming a write scope includes its read scope, and a list that holds every scope is a key with full access. Send either &#x60;scopes&#x60; or &#x60;preset&#x60;, not both | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
