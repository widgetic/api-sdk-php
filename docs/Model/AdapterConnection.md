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
**confirmation** | **string** | How this credential is proved before it is used. &#x60;email_code&#x60; means it is an email address: saving it emails a code to it, and it is used only after the code is given back (&#x60;confirmUserAdapterConnection&#x60;, &#x60;confirmPartnerAdapterConnection&#x60;). Null for a credential that is used as soon as it is saved |
**awaiting_confirmation** | **bool** | True when the credential is connected but has not been confirmed yet, so no adapter uses it. Always false when &#x60;confirmation&#x60; is null or the credential is not connected |
**confirmed_at** | **\DateTime** | When the credential was confirmed. Null when it is not connected, is awaiting its code, or needs no confirmation |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
