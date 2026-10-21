# # PartnerDataDatabase

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**partner_id** | **string** |  |
**host** | **string** | The Neon host of the database, as it appears in its connection string (&#x60;ep-....neon.tech&#x60;). |
**database_name** | **string** | The name of the database in your Neon project. |
**role_name** | **string** | The role Widgetic connects as. |
**verified_at** | **\DateTime** | When the database last passed the check. |
**last_verification_error** | **string** | Why the latest re-check failed, in a sentence you can act on. Null when the last check passed. |
**last_verification_failed_at** | **\DateTime** | When the latest re-check failed. Null when the last check passed. |
**updated_at** | **\DateTime** |  |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
