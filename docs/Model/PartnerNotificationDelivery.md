# # PartnerNotificationDelivery

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**delivery_id** | **string** |  |
**notification_id** | **string** |  |
**event_type** | **string** | What the notification was about. Null when the notification has been removed. |
**title** | **string** |  |
**channel** | **string** |  |
**target** | **string** | The email address, or the host of your webhook (never the whole address, which may hold a token) |
**status** | **string** |  |
**attempt_count** | **int** |  |
**next_attempt_at** | **\DateTime** | When the next attempt is made. Null once the delivery has ended. |
**last_attempt_at** | **\DateTime** |  |
**delivered_at** | **\DateTime** |  |
**last_status_code** | **int** | The HTTP status your webhook answered with at the last attempt, when it answered |
**last_error** | **string** | Why the last attempt failed, in a few words. Never what your endpoint replied. |
**created_at** | **\DateTime** |  |
**replay_of_delivery_id** | **string** | When this row is a manual replay, the earlier delivery it sent again |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
