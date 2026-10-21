# # PartnerAnalyticsTimeline

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**partner_id** | **string** |  |
**period** | [**\WidgeticApi\Model\PartnerReportPeriod**](PartnerReportPeriod.md) |  |
**managed_user_id** | **string** | The managed user the report is narrowed to. Null for the whole account. |
**days** | [**\WidgeticApi\Model\PartnerAnalyticsOfDay[]**](PartnerAnalyticsOfDay.md) | One entry for every day of the period, oldest first. A day nothing happened on is all zeros. |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
