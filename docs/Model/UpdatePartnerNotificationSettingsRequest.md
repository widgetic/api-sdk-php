# # UpdatePartnerNotificationSettingsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email_recipients** | **string[]** | The addresses the emails go to, at most five. An empty list goes back to the defaults. | [optional]
**email_events** | [**\WidgeticApi\Model\PartnerNotificationEventType[]**](PartnerNotificationEventType.md) | The events you want by email. Null for every event. | [optional]
**webhook_events** | [**\WidgeticApi\Model\PartnerNotificationEventType[]**](PartnerNotificationEventType.md) | The events to send to your webhook. Null for every event. | [optional]
**webhook_url** | **string** | Where to send the signed calls. It must be an https address on the standard port, on a public site, and it must not redirect. Null or an empty text switches the webhook off. Setting an address when you have no secret yet makes one. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
