# # PartnerNotificationSettings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**partner_id** | **string** |  |
**email_recipients** | **string[]** | The addresses the emails go to. Empty means the defaults. |
**default_email_recipients** | [**\WidgeticApi\Model\PartnerNotificationDefaultRecipients**](PartnerNotificationDefaultRecipients.md) |  |
**email_events** | [**\WidgeticApi\Model\PartnerNotificationEventType[]**](PartnerNotificationEventType.md) | The events you want by email. Null means every event. The events marked &#x60;alwaysEmailed&#x60; are emailed whatever it says. |
**webhook_url** | **string** | Where Widgetic sends a signed call for each event. Null while the webhook is switched off. |
**webhook_events** | [**\WidgeticApi\Model\PartnerNotificationEventType[]**](PartnerNotificationEventType.md) | The events sent to your webhook. Null means every event. |
**webhook_secret_set** | **bool** | Whether a signing secret exists. Calls are made only when it does. |
**webhook_secret_rotated_at** | **\DateTime** | When the current secret was made |
**webhook_signing_available** | **bool** | False when this server cannot sign webhooks, in which case a webhook cannot be set up yet |
**events** | [**\WidgeticApi\Model\PartnerNotificationEvent[]**](PartnerNotificationEvent.md) | Every event there is, for a settings screen to list |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
