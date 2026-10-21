# # CreatedUserApiKey

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**key** | **string** | The secret. Send it as a bearer token, in the &#x60;Authorization&#x60; header. Shown once |
**key_id** | **string** | The id of the key |
**key_preview** | **string** |  |
**name** | **string** |  |
**created_at** | **\DateTime** |  |
**expires_at** | **\DateTime** |  | [optional]
**is_active** | **bool** |  |
**scopes** | [**\WidgeticApi\Model\ApiKeyScope[]**](ApiKeyScope.md) | What the key may do. A key made without scopes holds every scope |
**preset** | **string** | The name the scopes amount to |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
