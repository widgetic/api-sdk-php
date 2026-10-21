# # UserApiKey

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**key_id** | **string** | The id of the key. Use it to rename, switch off, delete or read the usage of the key |
**key_preview** | **string** | The first characters of the key, to tell keys apart. Not enough to use it |
**name** | **string** | The name given to the key |
**created_at** | **\DateTime** |  |
**expires_at** | **\DateTime** | When the key stops working. Absent or null when it does not expire | [optional]
**last_used_at** | **\DateTime** | When the key was last used. Absent or null when it never was | [optional]
**is_active** | **bool** | Whether the key works. A key that is switched off is refused until it is switched on again |
**scopes** | [**\WidgeticApi\Model\ApiKeyScope[]**](ApiKeyScope.md) | What the key may do. A key with full access holds every scope. The scopes of a key are fixed when it is made |
**preset** | **string** | The name the scopes amount to. &#x60;full_access&#x60; is a key that is not limited, &#x60;read_only&#x60; and &#x60;content&#x60; are the ready-made lists, and &#x60;custom&#x60; is any other list |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
