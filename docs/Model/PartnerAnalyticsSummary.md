# # PartnerAnalyticsSummary

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**partner_id** | **string** |  |
**period** | [**\WidgeticApi\Model\PartnerReportPeriod**](PartnerReportPeriod.md) |  |
**managed_user_id** | **string** | The managed user the report is narrowed to. Null for the whole account. |
**views** | **int** | How many times a composition was shown to a visitor |
**interactions** | **int** | How many times a visitor did something with a composition |
**visitors** | **int** | How many different visitors viewed. A visitor is a browsing session; an event that carries no session is counted for the signed-in user instead. An event that carries neither is a view and no visitor. |
**compositions_viewed** | **int** | How many different compositions were viewed |
**managed_users_viewed** | **int** | How many different managed users had a composition viewed |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
