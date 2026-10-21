# # AdapterConnection

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**adapter_id** | **string** | The adapter the key is for (its id in the adapter catalog) |
**adapter_label** | **string** | What the adapter is called to its owner |
**credential_key** | **string** | The name of the key within the adapter. Use it, with the adapter id, to connect or remove the key |
**label** | **string** | What the key is called to its owner |
**scope** | **string** | Who may keep this key. &#x60;owner&#x60; is the person who made the widget, in their own account. &#x60;partner&#x60; is a partner, for the widgets of the customers it manages. &#x60;owner_or_partner&#x60; is either; for a widget of a managed customer the partner&#39;s key is used. |
**connected** | **bool** | Whether this account has connected the key |
**updated_at** | **\DateTime** | When the key was last set. Null when it is not connected |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
