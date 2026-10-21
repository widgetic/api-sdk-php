# # EditorSession

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**token** | **string** | The credential the browser sends as &#x60;Authorization: Bearer &lt;token&gt;&#x60;. It starts with &#x60;wgt_ses_&#x60;. It works only for the calls of the session&#39;s surfaces, only for this managed user&#39;s content, and only until &#x60;expiresAt&#x60;. |
**session_id** | **string** | Identifies the session, so you can end it (&#x60;revokeManagedUserEditorSession&#x60;). It is not a credential. |
**managed_user_id** | **string** |  |
**managed_user_external_id** | **string** | Your own identifier for the managed user |
**surfaces** | **string[]** |  |
**allowed_origin** | **string** | The web page origin the session is bound to, or null when it is not bound | [optional]
**max_credits** | **int** | The most credits the session may spend on Widgetic&#39;s AI (&#x60;max_credits&#x60;), or null when it has no limit of its own | [optional]
**expires_at** | **\DateTime** |  |
**created_at** | **\DateTime** |  |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
