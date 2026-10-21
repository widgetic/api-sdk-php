# # PartnerEntryContextSigning

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**partner_id** | **string** |  |
**required** | **bool** | True: an entry whose context carries no valid signature is refused (403 &#x60;CONTEXT_SIGNATURE_REQUIRED&#x60;). False: an entry that carries a signature is checked, and one that carries none is accepted as before. |
**secret_set** | **bool** | Whether you have a signing secret. Until you have, no signature is checked and none can be required. |
**secret_rotated_at** | **\DateTime** | When the current secret was made. Null while there is none. |
**previous_secret_valid_until** | **\DateTime** | While you switch to a new secret, when the secret it replaced stops being accepted. Null when there is none to wait for. |
**signing_available** | **bool** | False when this server cannot keep secrets, in which case none can be made yet. |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
