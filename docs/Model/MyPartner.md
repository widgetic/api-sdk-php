# # MyPartner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | The id every other partner route asks for (&#x60;/partners/{partnerId}/...&#x60;) |
**name** | **string** |  |
**status** | **string** | &#x60;active&#x60; while the partner is in force. &#x60;inactive&#x60; until Widgetic activates it (and after a deactivation). &#x60;suspended&#x60; while it is paused, which is done by hand and comes back when Widgetic resumes it. |
**contact_email** | **string** |  | [optional]
**allowed_domains** | **string[]** | The domains Widgetic added to the embeds of this partner&#39;s customers. The domains the person added themselves are on the domains route of the account. |
**platform_domain** | **string** | The website where the partner integrates Widgetic, as a bare name. It and every subdomain of it (&#x60;app.acme.com&#x60;, &#x60;learn.eu.acme.com&#x60;) can always show the partner&#39;s widgets, the ones its customers make through it included, and send entries to them, whatever &#x60;allowedDomains&#x60; and the account&#39;s own domain list say, so a list can never lock the partner&#39;s own website out. It is not an entry of &#x60;allowedDomains&#x60;, and it does not turn an empty list into a restriction: a partner that lists nothing stays unrestricted for every website. Widgetic sets it when the partner is set up; contact Widgetic to change it. &#x60;null&#x60; when none has been set. |
**suspended_at** | **\DateTime** | When the partner was paused; null unless it is paused now |
**suspension_reason** | **string** | The reason given when the partner was paused, as the partner is told it; null unless it is paused now |
**created_at** | **\DateTime** |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
