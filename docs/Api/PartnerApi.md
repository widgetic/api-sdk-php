# WidgeticApi\PartnerApi

All URIs are relative to https://api.widgetic.com/v1, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**addAiAnswersKnowledgeDocument()**](PartnerApi.md#addAiAnswersKnowledgeDocument) | **POST** /compositions/{id}/adapters/ai-answers/knowledge/documents | Add a document for a widget&#39;s AI to answer from |
| [**addPersonalWorkspaceDomain()**](PartnerApi.md#addPersonalWorkspaceDomain) | **POST** /users/{id}/workspace/domains | Allow a website to show your widgets |
| [**callPublicCompositionAdapter()**](PartnerApi.md#callPublicCompositionAdapter) | **POST** /embed/compositions/{compositionId}/adapters/{adapterId}/{operation} | Call a gateway operation of an adapter a published widget uses |
| [**checkCompositionAccess()**](PartnerApi.md#checkCompositionAccess) | **GET** /compositions/{id}/access | Check Composition Access |
| [**copyPresetForManagedUser()**](PartnerApi.md#copyPresetForManagedUser) | **POST** /managed-users/{id}/presets/{key}/copy | Give a managed user a copy of one of your presets |
| [**createCanvas()**](PartnerApi.md#createCanvas) | **POST** /canvases | Create Canvas |
| [**createComposition()**](PartnerApi.md#createComposition) | **POST** /compositions | Create Composition |
| [**createCompositionContentItem()**](PartnerApi.md#createCompositionContentItem) | **POST** /compositions/{id}/content/{list}/items | Add a content list item |
| [**createCompositionDatabaseRecord()**](PartnerApi.md#createCompositionDatabaseRecord) | **POST** /compositions/{id}/database/{table} | Create Record In Composition Database |
| [**createCompositionFromPreset()**](PartnerApi.md#createCompositionFromPreset) | **POST** /managed-users/{id}/presets/{key}/composition | Create a composition from one of your presets in one call |
| [**createCompositionFromWidget()**](PartnerApi.md#createCompositionFromWidget) | **POST** /widgets/{id}/composition | Create a composition for a widget in one call |
| [**createManagedUser()**](PartnerApi.md#createManagedUser) | **POST** /managed-users | Create Managed User |
| [**createManagedUserEditorSession()**](PartnerApi.md#createManagedUserEditorSession) | **POST** /managed-users/{id}/editor-sessions | Create an editor session for a managed user |
| [**createPartnerExtraCreditsInvoice()**](PartnerApi.md#createPartnerExtraCreditsInvoice) | **POST** /partners/{partnerId}/credits/extra-invoice | Buy extra credits for a partner |
| [**createPublicCompositionEntry()**](PartnerApi.md#createPublicCompositionEntry) | **POST** /embed/compositions/{compositionId}/entries/{table} | Append a visitor entry through the gateway |
| [**createUserApiKey()**](PartnerApi.md#createUserApiKey) | **POST** /users/{id}/keys | Create an API key |
| [**createWidget()**](PartnerApi.md#createWidget) | **POST** /widgets | Create Widget |
| [**deleteCanvas()**](PartnerApi.md#deleteCanvas) | **DELETE** /canvases/{id} | Delete Canvas |
| [**deleteComposition()**](PartnerApi.md#deleteComposition) | **DELETE** /compositions/{id} | Delete Composition |
| [**deleteCompositionContentItem()**](PartnerApi.md#deleteCompositionContentItem) | **DELETE** /compositions/{id}/content/{list}/items/{itemId} | Delete a content list item |
| [**deleteCompositionDataSource()**](PartnerApi.md#deleteCompositionDataSource) | **DELETE** /compositions/{id}/data-source | Remove the composition data source binding |
| [**deleteCompositionDatabaseRecord()**](PartnerApi.md#deleteCompositionDatabaseRecord) | **DELETE** /compositions/{id}/database/{table}/{recordId} | Delete Record From Composition Database |
| [**deleteCompositionEntryItems()**](PartnerApi.md#deleteCompositionEntryItems) | **DELETE** /compositions/{id}/entries/{table}/items | Delete composition entry items by id or host context |
| [**deleteManagedUser()**](PartnerApi.md#deleteManagedUser) | **DELETE** /managed-users/{id} | Delete Managed User |
| [**deletePersonalWorkspaceDomain()**](PartnerApi.md#deletePersonalWorkspaceDomain) | **DELETE** /users/{id}/workspace/domains/{domainId} | Stop allowing a website to show your widgets |
| [**deleteUserApiKey()**](PartnerApi.md#deleteUserApiKey) | **DELETE** /users/{id}/keys/{keyId} | Delete an API key |
| [**describeCompositionEntries()**](PartnerApi.md#describeCompositionEntries) | **GET** /compositions/{id}/entries | Describe What a Composition Keeps |
| [**duplicateComposition()**](PartnerApi.md#duplicateComposition) | **POST** /compositions/{id}/duplicate | Duplicate Composition |
| [**exportCompositionEntryItems()**](PartnerApi.md#exportCompositionEntryItems) | **GET** /compositions/{id}/entries/{table}/export | Export composition entry items |
| [**getAiAnswersKnowledge()**](PartnerApi.md#getAiAnswersKnowledge) | **GET** /compositions/{id}/adapters/ai-answers/knowledge | See the documents a widget&#39;s AI answers from |
| [**getAllCanvases()**](PartnerApi.md#getAllCanvases) | **GET** /canvases | Get All Canvases |
| [**getAllCompositions()**](PartnerApi.md#getAllCompositions) | **GET** /compositions | Get All Compositions |
| [**getAllManagedUsers()**](PartnerApi.md#getAllManagedUsers) | **GET** /managed-users | Get Managed Users |
| [**getCanvas()**](PartnerApi.md#getCanvas) | **GET** /canvases/{id} | Get Canvas |
| [**getCompositionById()**](PartnerApi.md#getCompositionById) | **GET** /compositions/{id} | Get Composition |
| [**getCompositionContent()**](PartnerApi.md#getCompositionContent) | **GET** /compositions/{id}/content | Get Current Content |
| [**getCompositionContentSchema()**](PartnerApi.md#getCompositionContentSchema) | **GET** /compositions/{id}/schema/content | Get Content Schema |
| [**getCompositionDataSource()**](PartnerApi.md#getCompositionDataSource) | **GET** /compositions/{id}/data-source | Read the composition data source binding |
| [**getCompositionDatabaseRecord()**](PartnerApi.md#getCompositionDatabaseRecord) | **GET** /compositions/{id}/database/{table}/{recordId} | Get Record From Composition Database |
| [**getCompositionDatabaseRecords()**](PartnerApi.md#getCompositionDatabaseRecords) | **GET** /compositions/{id}/database/{table} | Get All Records From Composition Database Table |
| [**getCompositionDesign()**](PartnerApi.md#getCompositionDesign) | **GET** /compositions/{id}/design | Get Composition Design |
| [**getCompositionDesignSchema()**](PartnerApi.md#getCompositionDesignSchema) | **GET** /compositions/{id}/schema/design | Get Design Schema |
| [**getCompositionEmbedSchema()**](PartnerApi.md#getCompositionEmbedSchema) | **GET** /compositions/{id}/schema/embed | Get Embed Schema |
| [**getCompositionEmbedSettings()**](PartnerApi.md#getCompositionEmbedSettings) | **GET** /compositions/{id}/embed-settings | Get Composition Embed Settings |
| [**getCompositionPreview()**](PartnerApi.md#getCompositionPreview) | **GET** /compositions/{id}/preview | Get Composition Preview |
| [**getCompositionVersions()**](PartnerApi.md#getCompositionVersions) | **GET** /compositions/{id}/versions | Get Composition Versions |
| [**getCompositionsBatch()**](PartnerApi.md#getCompositionsBatch) | **POST** /compositions/batch | Get Compositions Batch |
| [**getInvoicesByPartnerId()**](PartnerApi.md#getInvoicesByPartnerId) | **GET** /invoices/partner/{partnerId} | List a partner&#39;s invoices |
| [**getManagedUserById()**](PartnerApi.md#getManagedUserById) | **GET** /managed-users/{id} | Get Managed User By ID |
| [**getManagedUserDesignDefaults()**](PartnerApi.md#getManagedUserDesignDefaults) | **GET** /managed-users/{id}/design-defaults | Read design defaults for one managed user |
| [**getManagedUserEntitlements()**](PartnerApi.md#getManagedUserEntitlements) | **GET** /entitlements/managed-users/{managedUserId} | Get managed user entitlements |
| [**getManagedUserLimits()**](PartnerApi.md#getManagedUserLimits) | **GET** /managed-users/{id}/limits | Read monthly credit cap and usage for one managed user |
| [**getManagedUserStorageUsage()**](PartnerApi.md#getManagedUserStorageUsage) | **GET** /managed-users/{id}/storage-usage | Storage used by one managed user&#39;s uploads |
| [**getManagedUserUsage()**](PartnerApi.md#getManagedUserUsage) | **GET** /managed-users/{id}/usage | What a managed user&#39;s editor sessions spent |
| [**getManagedUsersByManagerId()**](PartnerApi.md#getManagedUsersByManagerId) | **GET** /users/{managerId}/managed-users | Get Managed Users By Manager |
| [**getMyPartners()**](PartnerApi.md#getMyPartners) | **GET** /partners/mine | Find the partner you administer |
| [**getPartnerAdapterConnections()**](PartnerApi.md#getPartnerAdapterConnections) | **GET** /partners/{partnerId}/adapter-connections | See which adapter keys a partner has connected |
| [**getPartnerAnalyticsByManagedUser()**](PartnerApi.md#getPartnerAnalyticsByManagedUser) | **GET** /partners/{partnerId}/analytics/managed-users | What each managed user&#39;s widgets did |
| [**getPartnerAnalyticsSummary()**](PartnerApi.md#getPartnerAnalyticsSummary) | **GET** /partners/{partnerId}/analytics/summary | What was done with a partner&#39;s published widgets |
| [**getPartnerAnalyticsTimeline()**](PartnerApi.md#getPartnerAnalyticsTimeline) | **GET** /partners/{partnerId}/analytics/timeline | What was done with a partner&#39;s widgets, day by day |
| [**getPartnerAnalyticsTopWidgets()**](PartnerApi.md#getPartnerAnalyticsTopWidgets) | **GET** /partners/{partnerId}/analytics/top-widgets | Which widgets were viewed the most |
| [**getPartnerBillingOverview()**](PartnerApi.md#getPartnerBillingOverview) | **GET** /partners/{partnerId}/billing-overview | Get comprehensive partner billing overview |
| [**getPartnerContract()**](PartnerApi.md#getPartnerContract) | **GET** /partners/{partnerId}/contract | Get a partner&#39;s contract |
| [**getPartnerCreditBalance()**](PartnerApi.md#getPartnerCreditBalance) | **GET** /partners/{partnerId}/credits/balance | Get partner credit balance |
| [**getPartnerCreditTransactions()**](PartnerApi.md#getPartnerCreditTransactions) | **GET** /partners/{partnerId}/credits/transactions | Get partner credit transaction history |
| [**getPartnerDataDatabase()**](PartnerApi.md#getPartnerDataDatabase) | **GET** /partners/{partnerId}/data-database | See the Neon database a partner keeps the data of its compositions in |
| [**getPartnerDesignDefaults()**](PartnerApi.md#getPartnerDesignDefaults) | **GET** /partners/{partnerId}/design-defaults | Read partner-wide design defaults |
| [**getPartnerEntitlements()**](PartnerApi.md#getPartnerEntitlements) | **GET** /entitlements/partners/{partnerId} | Get partner entitlements |
| [**getPartnerEntryContextSigning()**](PartnerApi.md#getPartnerEntryContextSigning) | **GET** /partners/{partnerId}/entry-context-signing | See how the context of your embeds is signed |
| [**getPartnerNotificationSettings()**](PartnerApi.md#getPartnerNotificationSettings) | **GET** /partners/{partnerId}/notifications/settings | Where your notifications go |
| [**getPartnerStorageDestination()**](PartnerApi.md#getPartnerStorageDestination) | **GET** /partners/{partnerId}/storage | Get where a partner&#39;s uploaded files are stored |
| [**getPartnerStorageUsage()**](PartnerApi.md#getPartnerStorageUsage) | **GET** /partners/{partnerId}/storage/usage | What a partner&#39;s customers store |
| [**getPersonalWorkspaceDomains()**](PartnerApi.md#getPersonalWorkspaceDomains) | **GET** /users/{id}/workspace/domains | List the websites allowed to show your widgets |
| [**getPublicCompositionEmbed()**](PartnerApi.md#getPublicCompositionEmbed) | **GET** /embed/compositions/{compositionId} | Resolve a composition UUID to a published widget URL |
| [**getPublicCompositionIframe()**](PartnerApi.md#getPublicCompositionIframe) | **GET** /embed/compositions/{compositionId}/frame | Embed a published composition with its saved values |
| [**getUserAdapterConnections()**](PartnerApi.md#getUserAdapterConnections) | **GET** /users/{userId}/adapter-connections | See which adapter keys an account has connected |
| [**getUserApiKeyUsageLogs()**](PartnerApi.md#getUserApiKeyUsageLogs) | **GET** /users/{id}/api-keys/{keyId}/logs | Read what an API key was used for |
| [**getUserApiKeys()**](PartnerApi.md#getUserApiKeys) | **GET** /users/{id}/keys | List the API keys of an account |
| [**getUserCreditBalance()**](PartnerApi.md#getUserCreditBalance) | **GET** /credits/user/{userId}/balance | Get an account&#39;s credit balance |
| [**getUserCreditTransactions()**](PartnerApi.md#getUserCreditTransactions) | **GET** /credits/user/{userId}/transactions | List an account&#39;s credit ledger |
| [**getWidgets()**](PartnerApi.md#getWidgets) | **GET** /widgets | List Widgets |
| [**getWidgetsBatch()**](PartnerApi.md#getWidgetsBatch) | **POST** /widgets/batch | Get Widgets Batch |
| [**listCompositionEntryItems()**](PartnerApi.md#listCompositionEntryItems) | **GET** /compositions/{id}/entries/{table}/items | List composition entry items with paging and filters |
| [**listManagedUserEntries()**](PartnerApi.md#listManagedUserEntries) | **GET** /managed-users/{id}/entries | List entries across a managed user&#39;s compositions |
| [**listPartnerNotificationDeliveries()**](PartnerApi.md#listPartnerNotificationDeliveries) | **GET** /partners/{partnerId}/notifications/deliveries | How your notifications reached you |
| [**listPartnerNotifications()**](PartnerApi.md#listPartnerNotifications) | **GET** /partners/{partnerId}/notifications | What your partner account was told |
| [**listPartnerPresets()**](PartnerApi.md#listPartnerPresets) | **GET** /partners/{partnerId}/presets | List the widgets a partner offers as presets |
| [**operationsIdGet()**](PartnerApi.md#operationsIdGet) | **GET** /operations/{id} | Get operation status |
| [**patchCompositionContentItem()**](PartnerApi.md#patchCompositionContentItem) | **PATCH** /compositions/{id}/content/{list}/items/{itemId} | Update a content list item |
| [**postPublicCompositionEmbedStatus()**](PartnerApi.md#postPublicCompositionEmbedStatus) | **POST** /embed/compositions/status | Batch-check whether compositions are currently served for embed |
| [**readCompositionEntries()**](PartnerApi.md#readCompositionEntries) | **GET** /compositions/{id}/entries/{table} | Read the Entries of a Composition&#39;s Table |
| [**removeAiAnswersKnowledgeDocument()**](PartnerApi.md#removeAiAnswersKnowledgeDocument) | **DELETE** /compositions/{id}/adapters/ai-answers/knowledge/documents/{documentId} | Remove a document from a widget&#39;s knowledge base |
| [**removePartnerAdapterConnection()**](PartnerApi.md#removePartnerAdapterConnection) | **DELETE** /partners/{partnerId}/adapter-connections/{adapterId}/{credentialKey} | Remove an adapter key from a partner |
| [**removePartnerDataDatabase()**](PartnerApi.md#removePartnerDataDatabase) | **DELETE** /partners/{partnerId}/data-database | Stop keeping the data of a partner&#39;s compositions in its own database |
| [**removePartnerPreset()**](PartnerApi.md#removePartnerPreset) | **DELETE** /partners/{partnerId}/presets/{key} | Take a widget off the partner&#39;s presets |
| [**removePartnerStorageDestination()**](PartnerApi.md#removePartnerStorageDestination) | **DELETE** /partners/{partnerId}/storage | Stop storing a partner&#39;s uploaded files in its own bucket |
| [**removeUserAdapterConnection()**](PartnerApi.md#removeUserAdapterConnection) | **DELETE** /users/{userId}/adapter-connections/{adapterId}/{credentialKey} | Remove an adapter key from an account |
| [**replayPartnerNotificationDelivery()**](PartnerApi.md#replayPartnerNotificationDelivery) | **POST** /partners/{partnerId}/notifications/deliveries/{deliveryId}/replay | Send a webhook delivery again |
| [**revokeManagedUserEditorSession()**](PartnerApi.md#revokeManagedUserEditorSession) | **DELETE** /managed-users/{id}/editor-sessions/{sessionId} | End one editor session of a managed user |
| [**revokeManagedUserEditorSessions()**](PartnerApi.md#revokeManagedUserEditorSessions) | **DELETE** /managed-users/{id}/editor-sessions | End every editor session of a managed user |
| [**rotatePartnerEntryContextSecret()**](PartnerApi.md#rotatePartnerEntryContextSecret) | **POST** /partners/{partnerId}/entry-context-signing/secret | Make a secret to sign the context of your embeds |
| [**rotatePartnerWebhookSecret()**](PartnerApi.md#rotatePartnerWebhookSecret) | **POST** /partners/{partnerId}/notifications/webhook-secret | Make a new secret for your webhook |
| [**sendPartnerNotificationTestEvent()**](PartnerApi.md#sendPartnerNotificationTestEvent) | **POST** /partners/{partnerId}/notifications/test-event | Send a test event to your webhook |
| [**setCompositionDataSource()**](PartnerApi.md#setCompositionDataSource) | **PUT** /compositions/{id}/data-source | Bind a public JSON data source for embed refresh |
| [**setDynamicContent()**](PartnerApi.md#setDynamicContent) | **PUT** /compositions/{id}/content | Set Dynamic Content |
| [**setManagedUserDesignDefaults()**](PartnerApi.md#setManagedUserDesignDefaults) | **PUT** /managed-users/{id}/design-defaults | Set or clear design defaults for one managed user |
| [**setManagedUserLimits()**](PartnerApi.md#setManagedUserLimits) | **PUT** /managed-users/{id}/limits | Set or clear the monthly credit cap for one managed user |
| [**setPartnerAdapterConnection()**](PartnerApi.md#setPartnerAdapterConnection) | **PUT** /partners/{partnerId}/adapter-connections/{adapterId}/{credentialKey} | Connect an adapter key to a partner |
| [**setPartnerDataDatabase()**](PartnerApi.md#setPartnerDataDatabase) | **PUT** /partners/{partnerId}/data-database | Keep the data of a partner&#39;s compositions in a Neon database of its own |
| [**setPartnerDesignDefaults()**](PartnerApi.md#setPartnerDesignDefaults) | **PUT** /partners/{partnerId}/design-defaults | Set or clear partner-wide design defaults |
| [**setPartnerPreset()**](PartnerApi.md#setPartnerPreset) | **PUT** /partners/{partnerId}/presets/{key} | Make a widget a preset, or replace a preset |
| [**setPartnerStorageDestination()**](PartnerApi.md#setPartnerStorageDestination) | **PUT** /partners/{partnerId}/storage | Set where a partner&#39;s uploaded files are stored |
| [**setUserAdapterConnection()**](PartnerApi.md#setUserAdapterConnection) | **PUT** /users/{userId}/adapter-connections/{adapterId}/{credentialKey} | Connect an adapter key to an account |
| [**updateCanvas()**](PartnerApi.md#updateCanvas) | **PUT** /canvases/{id} | Update Canvas |
| [**updateComposition()**](PartnerApi.md#updateComposition) | **PUT** /compositions/{id} | Update Composition |
| [**updateCompositionDatabaseRecord()**](PartnerApi.md#updateCompositionDatabaseRecord) | **PUT** /compositions/{id}/database/{table}/{recordId} | Update Record In Composition Database |
| [**updateCompositionStatus()**](PartnerApi.md#updateCompositionStatus) | **PUT** /compositions/{id}/status | Update Composition Status |
| [**updateManagedUser()**](PartnerApi.md#updateManagedUser) | **PUT** /managed-users/{id} | Update Managed User |
| [**updatePartnerEntryContextSigning()**](PartnerApi.md#updatePartnerEntryContextSigning) | **PUT** /partners/{partnerId}/entry-context-signing | Require a signed context, or stop requiring it |
| [**updatePartnerNotificationSettings()**](PartnerApi.md#updatePartnerNotificationSettings) | **PUT** /partners/{partnerId}/notifications/settings | Choose where your notifications go |
| [**updatePersonalWorkspaceDomain()**](PartnerApi.md#updatePersonalWorkspaceDomain) | **PUT** /users/{id}/workspace/domains/{domainId} | Change a website on your list |
| [**updateUserApiKey()**](PartnerApi.md#updateUserApiKey) | **PUT** /users/{id}/keys/{keyId} | Rename an API key, or switch it off or on |
| [**uploadPublicCompositionAdapterFile()**](PartnerApi.md#uploadPublicCompositionAdapterFile) | **PUT** /embed/compositions/{compositionId}/adapters/upload/files/{ticket} | Send the file a visitor chose through the upload adapter of a published widget |
| [**uploadsGet()**](PartnerApi.md#uploadsGet) | **GET** /uploads | List the account&#39;s uploads |
| [**uploadsIdDelete()**](PartnerApi.md#uploadsIdDelete) | **DELETE** /uploads/{id} | Delete an upload |
| [**uploadsIdGet()**](PartnerApi.md#uploadsIdGet) | **GET** /uploads/{id} | Get an upload by id |
| [**uploadsLimitsGet()**](PartnerApi.md#uploadsLimitsGet) | **GET** /uploads/limits | Upload size limits and accepted file types |
| [**uploadsPost()**](PartnerApi.md#uploadsPost) | **POST** /uploads | Upload a file |
| [**validateCompositionContent()**](PartnerApi.md#validateCompositionContent) | **POST** /compositions/{id}/content/validate | Validate Content |
| [**validateToken()**](PartnerApi.md#validateToken) | **GET** /tokens/validate | Validate current authentication token |
| [**verifyPartnerDataDatabase()**](PartnerApi.md#verifyPartnerDataDatabase) | **POST** /partners/{partnerId}/data-database/verify | Check that a partner&#39;s own database still works |
| [**verifyPartnerStorageDestination()**](PartnerApi.md#verifyPartnerStorageDestination) | **POST** /partners/{partnerId}/storage/verify | Check that a partner&#39;s storage destination still works |


## `addAiAnswersKnowledgeDocument()`

```php
addAiAnswersKnowledgeDocument($id, $add_ai_answers_knowledge_document_request, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\AddAiAnswersKnowledgeDocument201Response
```

Add a document for a widget's AI to answer from

Gives the widget's AI a document to answer visitors' questions from. Send the title and the plain text. The call returns once the document is ready to be used, which takes a few seconds, longer for a long text.  **How it is used.** The text is cleaned, cut into short passages and each passage is turned into numbers (an embedding) so the widget can find the passages nearest to a question. When a visitor asks, the nearest passages and the question are shown to an AI model, which writes the answer from them and from nothing else; if the documents say nothing about the question the visitor is told so, and the owner is not charged for that question. The titles of the documents an answer used are shown to the visitor as its sources.  **What leaves Widgetic.** The text of a document is sent to OpenAI to be embedded when it is added, and the passages used for a question are sent to the AI model that writes the answer. Say so in your privacy policy.  **Treat every document as public.** An answer can quote or paraphrase anything a document says, to any visitor of the widget. Do not add passwords, keys, personal data or anything that must stay private.  **Limits.** A widget holds up to 20 documents, each up to 100000 characters, and up to 400000 characters in all (`getAiAnswersKnowledge` reports the current numbers). Text only: convert PDF or Word files to text first. Adding a document costs no credits. The same text cannot be added twice to one widget (409).  The caller must be allowed to change the widget. An API key needs the `content:write` scope. Adds are limited to ten in ten minutes per person.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The widget (composition) to add the document to
$add_ai_answers_knowledge_document_request = new \WidgeticApi\Model\AddAiAnswersKnowledgeDocumentRequest(); // \WidgeticApi\Model\AddAiAnswersKnowledgeDocumentRequest
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->addAiAnswersKnowledgeDocument($id, $add_ai_answers_knowledge_document_request, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->addAiAnswersKnowledgeDocument: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The widget (composition) to add the document to | |
| **add_ai_answers_knowledge_document_request** | [**\WidgeticApi\Model\AddAiAnswersKnowledgeDocumentRequest**](../Model/AddAiAnswersKnowledgeDocumentRequest.md)|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\AddAiAnswersKnowledgeDocument201Response**](../Model/AddAiAnswersKnowledgeDocument201Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `addPersonalWorkspaceDomain()`

```php
addPersonalWorkspaceDomain($id, $add_domain_request): \WidgeticApi\Model\PersonalWorkspaceDomainResultResponse
```

Allow a website to show your widgets

Adds a website to an account's own list. Give a website name such as `example.com`, or `*.example.com` for a website and all of its subdomains. A scheme, a port, a path, capital letters and a leading `www.` are dropped, so `https://www.Example.com/shop` is kept as `example.com`, and `example.com` covers `www.example.com` too. Something that is not a website name is refused, not stored. Until the first website is added nothing is restricted, and a widget can be shown anywhere. Once the list has one, a widget of the account is shown on the listed websites (and on Widgetic's own) and nowhere else. A page on your own machine (`localhost`, `127.0.0.1` or `[::1]`, on any port) is always allowed, so there is nothing to add to test locally. So is the website where a partner your account administers integrates Widgetic, with every subdomain of it (`platformDomain` in the answer of `GET /partners/mine`), so there is nothing to add for it either and a list can never lock it out. A change can take about 15 seconds to reach every server. The list is a safeguard against other websites showing your widgets in a visitor's browser. It is not access control: anyone who knows a widget's id can still fetch its published content with a plain request that names no website. There is no limit on the list of an account that administers a partner, so a partner can add the website of each of its customers as they publish on their own domain, one call each. Any other account can list at most 50 websites, and the 51st is answered with a 409 (`BUSINESS_STATE_CONFLICT`). A wildcard such as `*.example.com` counts as one website, not one per subdomain, so use it instead of listing each subdomain. A page that frames a widget can name only so many websites to the browser (about fifty of ordinary length). Past that, the browser no longer checks the list for that page; the lookup that the Embed SDK makes for the widget still refuses every website that is not on the list.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The account the list belongs to. For your own, your own user id
$add_domain_request = new \WidgeticApi\Model\AddDomainRequest(); // \WidgeticApi\Model\AddDomainRequest

try {
    $result = $apiInstance->addPersonalWorkspaceDomain($id, $add_domain_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->addPersonalWorkspaceDomain: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The account the list belongs to. For your own, your own user id | |
| **add_domain_request** | [**\WidgeticApi\Model\AddDomainRequest**](../Model/AddDomainRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\PersonalWorkspaceDomainResultResponse**](../Model/PersonalWorkspaceDomainResultResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `callPublicCompositionAdapter()`

```php
callPublicCompositionAdapter($composition_id, $adapter_id, $operation, $public_adapter_call_request): \WidgeticApi\Model\PublicAdapterCallResult
```
### URI(s):
- https://api.widgetic.com The public embed routes are served at the root of the API host, not under /v1.
Call a gateway operation of an adapter a published widget uses

The door a widget's adapter module calls, from the visitor's browser, for the operations that cannot run in the browser: anything with a secret, a charge in credits or the owner's storage behind it. A widget that uses such an adapter is handed the address of this route as `adapters.url` in its `widgetic:host` message (see the host bridge contract) and calls `{adapters.url}/{adapterId}/{operation}`. It is not meant to be called by hand, and it takes no API key. **Address.** `https://api.widgetic.com/embed/compositions/{compositionId}/adapters/{adapterId}/{operation}`: the root of the API host, NOT under `/v1`. A client generated from this description for `https://api.widgetic.com/v1` must be given the base address `https://api.widgetic.com` for the calls of the `Public Embed` tag. **What it serves.** Only an adapter, and a version of it, that the widget's LIVE manifest (what the version that is published uses) lists, and only an operation that runs on the gateway. Anything else is one 404 `ADAPTER_NOT_AVAILABLE`, whatever the reason, so the route is no way to ask what a widget contains. An adapter an administrator stopped offering to NEW widgets keeps serving the widgets that already use it. **Who may call.** The same rule as the entry route: a permitted `Origin` header, which is the artifact origin the widget runs from or a website the owner allowed (or the owner's own platform). Page script cannot forge it. A request without a permitted `Origin` is 403 `ORIGIN_NOT_ALLOWED`. A composition that is not served (unpublished, or its owner's plan does not serve it) is 404, with the codes of the other public embed routes. When the partner of the owner signs the host context, a context that is not signed as the partner requires is refused with 403 `CONTEXT_SIGNATURE_REQUIRED`, `CONTEXT_SIGNATURE_INVALID` or `CONTEXT_SIGNATURE_EXPIRED`. **Cost and retries.** An operation priced in credits is charged to the owner of the widget (for a customer a partner manages, to the partner's administrator, within the monthly credits set for that customer), once for each `requestId`, before it runs, and given back if it does not answer. A `requestId` that was charged and not given back is 409 `REQUEST_ALREADY_USED` and the operation is NOT run a second time; one whose charge was given back may be tried again with the same `requestId`. A visitor never sees an owner's balance: a feature that cannot be used because its owner has no credits left, because the customer's monthly credits are spent, or because an administrator stopped the adapter, is the same 503 `ADAPTER_UNAVAILABLE` as every other \"not right now\". The owner is told through a notice. **Limits.** In front of everything, 120 calls a minute for each visitor address and composition and 600 a minute for a composition (429 `RATE_LIMITED`). Then, for each operation of a widget, a rate for each visitor address a minute and a cap for the widget a day: 30 and 5000 for an operation that is free, 10 and 500 for one that costs credits, unless the adapter says otherwise (never above 120 and 100000). A visitor over the rate is 429 `RATE_LIMITED`; a widget over its cap is 429 `WIDGET_LIMIT_REACHED`. Both carry a `Retry-After` header. The body is at most 64 KiB (413 `PAYLOAD_TOO_LARGE`) and JSON (415 `UNSUPPORTED_MEDIA_TYPE`); an operation has 30 seconds to answer (504 `ADAPTER_TIMEOUT`, and the charge is given back).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$composition_id = 'composition_id_example'; // string
$adapter_id = 'adapter_id_example'; // string | The id of the adapter, the name its module is known by, for example `upload`.
$operation = 'operation_example'; // string | The name of one operation of the adapter, as its documentation gives it.
$public_adapter_call_request = new \WidgeticApi\Model\PublicAdapterCallRequest(); // \WidgeticApi\Model\PublicAdapterCallRequest

$hostIndex = 0;
$variables = [
];

try {
    $result = $apiInstance->callPublicCompositionAdapter($composition_id, $adapter_id, $operation, $public_adapter_call_request, $hostIndex, $variables);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->callPublicCompositionAdapter: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **composition_id** | **string**|  | |
| **adapter_id** | **string**| The id of the adapter, the name its module is known by, for example &#x60;upload&#x60;. | |
| **operation** | **string**| The name of one operation of the adapter, as its documentation gives it. | |
| **public_adapter_call_request** | [**\WidgeticApi\Model\PublicAdapterCallRequest**](../Model/PublicAdapterCallRequest.md)|  | |
| hostIndex | null|int | Host index. Defaults to null. If null, then the library will use $this->hostIndex instead | [optional] |
| variables | array | Associative array of variables to pass to the host. Defaults to empty array. | [optional] |

### Return type

[**\WidgeticApi\Model\PublicAdapterCallResult**](../Model/PublicAdapterCallResult.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `checkCompositionAccess()`

```php
checkCompositionAccess($id): \WidgeticApi\Model\CheckCompositionAccessResponse
```

Check Composition Access

Checks if the authenticated user can access a specific composition based on workspace context and permissions.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | Composition ID

try {
    $result = $apiInstance->checkCompositionAccess($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->checkCompositionAccess: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| Composition ID | |

### Return type

[**\WidgeticApi\Model\CheckCompositionAccessResponse**](../Model/CheckCompositionAccessResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `copyPresetForManagedUser()`

```php
copyPresetForManagedUser($id, $key, $idempotency_key, $copy_partner_preset_request): \WidgeticApi\Model\PartnerPresetCopyResponse
```

Give a managed user a copy of one of your presets

Copies the preset `key` (see `setPartnerPreset`) onto a new canvas for one of your managed users, so their widget creator opens on a widget of their own that starts from yours. The copy is a draft widget in your account, filed under the managed user: `getAllWidgets` with `managedUserId` lists it, and no other managed user's editor can reach it.  The copy carries the preset's code, design and content schemas, and thumbnail, and starts from a fork of its code repository, so the user's chat edits begin where yours left off. It does not carry the preset's database or its compositions. It is not a preset itself, and changing or removing the preset afterwards never touches it.  To start a composition (the content and design editor) instead, you do not need a copy: call `createComposition` with the preset's `widgetId` (from `listPartnerPresets`) and the managed user.  The `Idempotency-Key` header is required (`400` without it). Send the same key when you retry, so one copy is made, not two. A copy that could not be made leaves nothing behind (503 `PRESET_COPY_FAILED`).  The managed user must be yours and active.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The managed user to give the copy to (Widgetic's id for the user)
$key = 'key_example'; // string | The key of the preset to copy
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$copy_partner_preset_request = new \WidgeticApi\Model\CopyPartnerPresetRequest(); // \WidgeticApi\Model\CopyPartnerPresetRequest

try {
    $result = $apiInstance->copyPresetForManagedUser($id, $key, $idempotency_key, $copy_partner_preset_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->copyPresetForManagedUser: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The managed user to give the copy to (Widgetic&#39;s id for the user) | |
| **key** | **string**| The key of the preset to copy | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **copy_partner_preset_request** | [**\WidgeticApi\Model\CopyPartnerPresetRequest**](../Model/CopyPartnerPresetRequest.md)|  | [optional] |

### Return type

[**\WidgeticApi\Model\PartnerPresetCopyResponse**](../Model/PartnerPresetCopyResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createCanvas()`

```php
createCanvas($create_canvas_request): \WidgeticApi\Model\CanvasResponse
```

Create Canvas

Creates a new canvas with the specified properties.  To make the canvas for one of your managed users, send `managedUserId` or `managedUserExternalId`. The canvas stays in your account and is yours to edit; the tag lets you list one user's canvases with `getAllCanvases`. The managed user must be yours and active: one that is not yours, or does not exist, is answered with 404 and `MANAGED_USER_NOT_FOUND`, and one that is switched off with 409 and `MANAGED_USER_INACTIVE`. The tag is set here and does not change afterwards. Called with an editor session, the canvas is always made for the session's managed user.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$create_canvas_request = new \WidgeticApi\Model\CreateCanvasRequest(); // \WidgeticApi\Model\CreateCanvasRequest

try {
    $result = $apiInstance->createCanvas($create_canvas_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->createCanvas: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **create_canvas_request** | [**\WidgeticApi\Model\CreateCanvasRequest**](../Model/CreateCanvasRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\CanvasResponse**](../Model/CanvasResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createComposition()`

```php
createComposition($idempotency_key, $new_composition, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionFromWidget201Response
```

Create Composition

Creates a new composition.  To make the composition for one of your managed users, send `managedUserId` or `managedUserExternalId`. The composition stays in your account and is yours to edit; the tag lets you list one user's compositions with `getAllCompositions`. The managed user must be yours and active: one that is not yours, or does not exist, is answered with 404 and `MANAGED_USER_NOT_FOUND`, and one that is switched off with 409 and `MANAGED_USER_INACTIVE`. The tag is set here and does not change afterwards. A copy made with `duplicateComposition` keeps the tag of the original.  An editor session with the `creator` surface may call this to start a composition of a widget it built: it sends only `name`, `widgetId` (a widget made for the session's managed user) and `content`, and the composition is always made for that managed user.  Send `databaseSchema` to give the composition tables of its own for what visitors send it (the shape, the allowed types and the limits are described on the field). A `databaseSchema` that cannot be used is refused before anything is created, with `400` and `INVALID_DATABASE_SCHEMA`. If the composition is created but its tables cannot be made just now, the answer is still `201` and `meta.warnings` says so.  Leave `databaseSchema` out and the composition gets the tables its widget declares in its own source (`src/lib/meta/database.json`), if it declares any: they are made the same way, in a schema of the composition's own. A widget that keeps nothing leaves the composition without tables. If the widget's file cannot be used, or its tables cannot be made just now, the answer is still `201` and `meta.warnings` says so. The widget is read as it was when it was last published (as it is now, when it never was).  The `Idempotency-Key` header is required (`400` without it). Send the same key when you retry, so one composition is created, not two.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$new_composition = new \WidgeticApi\Model\NewComposition(); // \WidgeticApi\Model\NewComposition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->createComposition($idempotency_key, $new_composition, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->createComposition: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **new_composition** | [**\WidgeticApi\Model\NewComposition**](../Model/NewComposition.md)|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\CreateCompositionFromWidget201Response**](../Model/CreateCompositionFromWidget201Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createCompositionContentItem()`

```php
createCompositionContentItem($id, $list, $idempotency_key, $create_composition_content_item_request, $if_match, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionContentItem201Response
```

Add a content list item

Creates one item in a widget content list without replacing the whole list. Item field keys are widget data (camelCase or snake_case are kept as sent). Partners use this to keep galleries in sync.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$list = 'list_example'; // string | List name from the content schema (`contentItems`) or `items`
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$create_composition_content_item_request = new \WidgeticApi\Model\CreateCompositionContentItemRequest(); // \WidgeticApi\Model\CreateCompositionContentItemRequest
$if_match = 'if_match_example'; // string | Optional content version from ETag
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->createCompositionContentItem($id, $list, $idempotency_key, $create_composition_content_item_request, $if_match, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->createCompositionContentItem: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **list** | **string**| List name from the content schema (&#x60;contentItems&#x60;) or &#x60;items&#x60; | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **create_composition_content_item_request** | [**\WidgeticApi\Model\CreateCompositionContentItemRequest**](../Model/CreateCompositionContentItemRequest.md)|  | |
| **if_match** | **string**| Optional content version from ETag | [optional] |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\CreateCompositionContentItem201Response**](../Model/CreateCompositionContentItem201Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createCompositionDatabaseRecord()`

```php
createCompositionDatabaseRecord($id, $table, $idempotency_key, $body, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionDatabaseRecord201Response
```

Create Record In Composition Database

Creates a new record in one of the composition's tables. Only the composition's own tables (made from its `databaseSchema` or from the tables its widget declares) can be reached; any other table name answers `404`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$table = 'table_example'; // string | Name of the database table
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$body = array('key' => new \stdClass); // object
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->createCompositionDatabaseRecord($id, $table, $idempotency_key, $body, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->createCompositionDatabaseRecord: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **table** | **string**| Name of the database table | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **body** | **object**|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\CreateCompositionDatabaseRecord201Response**](../Model/CreateCompositionDatabaseRecord201Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createCompositionFromPreset()`

```php
createCompositionFromPreset($id, $key, $idempotency_key, $create_composition_from_preset_request): \WidgeticApi\Model\CreateCompositionFromWidget201Response
```

Create a composition from one of your presets in one call

Validates the name, optional content, design, embed settings and locale, then creates a draft composition filed under the managed user, built on the preset's widget, in a single insert. A failure never leaves a half-made composition.  The preset's widget must be published. The managed user must be yours and active.  A widget that keeps what visitors send (a form, a vote, a rating) declares its tables in its own source (`src/lib/meta/database.json`); they are made for the composition here, in a schema of its own, as the widget was when it was last published. A widget that keeps nothing leaves the composition without tables. If the tables cannot be made just now, or the widget's file cannot be used, the composition is still created (`201`) and `meta.warnings` says why; the tables are made the next time the widget is generated.  The `Idempotency-Key` header is required (`400` without it). Send the same key when you retry, so one composition is created, not two.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$key = 'key_example'; // string
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$create_composition_from_preset_request = {"name":"Customer rating page","embedSettings":{"width":640,"height":480},"locale":"fr-FR"}; // \WidgeticApi\Model\CreateCompositionFromPresetRequest

try {
    $result = $apiInstance->createCompositionFromPreset($id, $key, $idempotency_key, $create_composition_from_preset_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->createCompositionFromPreset: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **key** | **string**|  | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **create_composition_from_preset_request** | [**\WidgeticApi\Model\CreateCompositionFromPresetRequest**](../Model/CreateCompositionFromPresetRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\CreateCompositionFromWidget201Response**](../Model/CreateCompositionFromWidget201Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createCompositionFromWidget()`

```php
createCompositionFromWidget($id, $idempotency_key, $create_composition_from_widget_request): \WidgeticApi\Model\CreateCompositionFromWidget201Response
```

Create a composition for a widget in one call

After a managed user publishes a widget from the creator, call this with the widget id, the customer's managed user (when the widget is not already filed under one), and optional content, design, embed settings and locale. Every input is validated before a single insert; a failure never leaves a half-made composition.  When the widget is already tagged with a managed user, you may omit `managedUserId`. When you send it, it must match that tag.  A widget that keeps what visitors send (a form, a vote, a rating) declares its tables in its own source (`src/lib/meta/database.json`); they are made for the composition here, in a schema of its own, as the widget was when it was last published. A widget that keeps nothing leaves the composition without tables. If the tables cannot be made just now, or the widget's file cannot be used, the composition is still created (`201`) and `meta.warnings` says why; the tables are made the next time the widget is generated.  The widget must be published. The `Idempotency-Key` header is required.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The widget id
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$create_composition_from_widget_request = {"name":"Published widget embed","managedUserId":"123e4567-e89b-12d3-a456-426614174000","locale":"de-DE"}; // \WidgeticApi\Model\CreateCompositionFromWidgetRequest

try {
    $result = $apiInstance->createCompositionFromWidget($id, $idempotency_key, $create_composition_from_widget_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->createCompositionFromWidget: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The widget id | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **create_composition_from_widget_request** | [**\WidgeticApi\Model\CreateCompositionFromWidgetRequest**](../Model/CreateCompositionFromWidgetRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\CreateCompositionFromWidget201Response**](../Model/CreateCompositionFromWidget201Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createManagedUser()`

```php
createManagedUser($idempotency_key, $new_managed_user): \WidgeticApi\Model\ManagedUserResponse
```

Create Managed User

Creates a new managed user for a partner account.  The `Idempotency-Key` header is required (`400` without it). Send the same key when you retry, so one managed user is created, not two.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$new_managed_user = {"externalId":"external-user-123","metadata":{"firstName":"John","lastName":"Doe","role":"editor"}}; // \WidgeticApi\Model\NewManagedUser

try {
    $result = $apiInstance->createManagedUser($idempotency_key, $new_managed_user);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->createManagedUser: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **new_managed_user** | [**\WidgeticApi\Model\NewManagedUser**](../Model/NewManagedUser.md)|  | |

### Return type

[**\WidgeticApi\Model\ManagedUserResponse**](../Model/ManagedUserResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createManagedUserEditorSession()`

```php
createManagedUserEditorSession($id, $new_editor_session): \WidgeticApi\Model\EditorSessionResponse
```

Create an editor session for a managed user

Makes a short-lived credential that lets the browser of ONE of your managed users use Widgetic's editor pieces, such as the File Browser and the composition editor, without your API key ever reaching that browser. Call this from your server when the page that hosts the editor opens, and hand the `token` in the answer to that page.  The token is shown once. It starts with `wgt_ses_` and the browser sends it as `Authorization: Bearer <token>`. It can do only what the `surfaces` you name allow, and only for this managed user:  - `files`: upload a file (`uploadsPost`) and list the files uploaded for this user (`uploadsGet`). Every   file is filed for this user and stored in your own storage destination, never in Widgetic's: a file a   customer uploads is yours to keep, and takes none of your storage allowance. Partner storage is not   optional, so no session, whatever its surfaces, can be made until you have set a destination   (`setPartnerStorageDestination`); until then it is refused with 409 and `PARTNER_STORAGE_REQUIRED`, and   when the destination cannot be used with 503 and `STORAGE_DESTINATION_UNAVAILABLE`. A destination you   remove after the session was made stops its uploads too (the same 409; the browser is only told that   the feature is not available right now). To keep a customer from uploading, leave `files` out of the   session and hand the editors your own media library instead (`mediaLibrary`). - `editor`: edit one of this user's compositions: read it (`getCompositionById`, its content, design,   embed settings and schemas), check a content change (`validateCompositionContent`), and change its   name, content, design and embed settings (`updateComposition`, `setDynamicContent`). It can reach   only compositions you created for this managed user (tag them with `managedUserId` when you create   them); any other composition, including another of your users', answers 404. - `creator`: use Widgetic's widget creator for this user, including its AI. Draw on canvases and save   them (`getAllCanvases`, `getCanvas`, `createCanvas`, `updateCanvas`, `previewDeleteCanvas`,   `deleteCanvas`); make, change, copy and delete the widgets on them (`createWidget`, `getWidgets`,   `getWidgetsBatch`, `updateWidget`, `uploadWidgetThumbnail`, `duplicateWidget`, `deleteWidget`);   list and make the compositions of a widget it built (`getAllCompositions`, `createComposition`), which   is how it shows the widget with sample values; keep the   conversation of each widget (`getConversationsByWidgetId`, `createConversationForWidget`,   `updateConversation`, `getMessages`, `createMessage`, `updateMessage`, `restoreCheckpoint`); and read a   widget's schemas and give it its repository (`getWidgetContentSchema`, `getWidgetDesignSchema`,   `updateWidgetRepository`). The AI that builds a widget is part of it: list the models   (`agentModelsGet`), open the widget's repository (`agentRepositoriesPost`,   `agentRepositoriesRepoIdGet`), start a generation and follow or cancel it (`agentCodeGeneratePost`,   `operationsStreamGet`, `operationsIdGet`, `operationsIdCancelPost`), build and preview the result   (`agentWidgetBuilderRepoHeadWidgetIdGet`, `buildWidgetFromRepo`, `previewWidgetVersion`), publish a   version of the widget and move between its versions (`agentWidgetBuilderPublishWidgetIdPost`,   `getWidgetPublishHistory`, `setWidgetPublishHistoryLive`, `renameWidgetPublishHistoryTitle`), and   turn a stroke or a sentence into a decision (`agentShapeRecognizePost`, `agentDesignResolvePost`). It can   also offer the customer your presets as starting points: read them and ask for a copy for this customer   (`listMyPresets`, `copyMyPreset`; you choose the presets with `setPartnerPreset`).   What the session makes is filed for this managed user, and the lists it reads hold only this user's   canvases, widgets and compositions. It can reach only canvases, widgets, compositions, repositories,   uploaded files and operations made for this managed user (tag the canvases and widgets you create   with `managedUserId`); any other canvas, widget, composition, conversation, message, repository, file   or operation, including another of your users', answers 404. The creator also saves the composition   it is editing (`updateComposition`, from the `editor` surface) and attaches pictures to its chat   (`uploadsPost`, from the `files` surface), and the surfaces do not imply one another: to open the   whole creator for a user, ask for `creator`, `editor` and `files` together. A generation or a build   one user starts can be followed and cancelled by that user and by you, never by another of your   users. The AI is paid for by your account, as your own calls are: its credits and allowances are   yours. A session cannot make a widget public (publishing a version does not), file one under a   project or an organization, or set anything the creator does not set: a body with another field is   refused with 403 and `EDITOR_SESSION_FIELD_NOT_ALLOWED`.  Everything else is refused with 403 and `EDITOR_SESSION_ROUTE_NOT_ALLOWED`: a session cannot read your account, make more sessions, change your presets or delete a composition, and a session without the `creator` surface cannot create or list compositions. Create the composition yourself with your API key, then open the editor on it.  A session ends at `expiresAt` (at most four hours), when you end it (`revokeManagedUserEditorSession`), or when the managed user is switched off or deleted. A managed user can have at most 100 live sessions at once (`429 EDITOR_SESSION_LIMIT_REACHED`). A session that is bound to a web page (`allowedOrigin`) is refused from any other origin.  The AI the session runs is paid for with your credits. Set `maxCredits` to hold the session to a number of them: once its generations have taken that many (a generation that fails is refunded and does not count), the next one is refused with 402 and `EDITOR_SESSION_CREDIT_LIMIT_REACHED`, and the browser is told only that the feature is not available right now. Without it, the limit Widgetic has set for your account applies when it has set one (the same limit for every session you make, and `maxCredits: null` asks for none), and otherwise the credits of your account are the only ceiling. What each of your users' sessions has spent is in `getManagedUserUsage`.  Each call makes a new session. It does not take an `Idempotency-Key`: the answer holds the token, and the token is never stored where a retry could read it back. The answer is sent with `Cache-Control: no-store`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The managed user the session is for (Widgetic's id for the user)
$new_editor_session = new \WidgeticApi\Model\NewEditorSession(); // \WidgeticApi\Model\NewEditorSession

try {
    $result = $apiInstance->createManagedUserEditorSession($id, $new_editor_session);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->createManagedUserEditorSession: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The managed user the session is for (Widgetic&#39;s id for the user) | |
| **new_editor_session** | [**\WidgeticApi\Model\NewEditorSession**](../Model/NewEditorSession.md)|  | |

### Return type

[**\WidgeticApi\Model\EditorSessionResponse**](../Model/EditorSessionResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createPartnerExtraCreditsInvoice()`

```php
createPartnerExtraCreditsInvoice($partner_id, $idempotency_key, $request_extra_credits): \WidgeticApi\Model\PartnerExtraCreditsInvoiceResponse
```

Buy extra credits for a partner

Asks Widgetic for an invoice for extra credits, on top of the credits of the contract. Name the dollars; the invoice is for the most whole credits they buy at the **list price** of a credit (the price a contract may lower belongs to the contract), so it is never for more than you asked: 12.34 buys 123 credits and the invoice says 12.30. The smallest purchase is 10 dollars and one request buys at most 100000 (ask Widgetic for an invoice for more).  Pay the invoice with the link in the answer. When it is paid the credits are added **once, for good**, to the account of the person who administers the partner, which is the account everything the partner builds is charged to (`getPartnerCreditBalance` shows it). Extra credits **do not expire**, unlike the credits of a contract period, which end with it. Nothing is added before the invoice is paid, and an unpaid invoice for extra credits never stops the partner: only an unpaid invoice of the contract does (`payment_arrears`).  Allowed whatever the partner's standing: a partner that has run out of credits, or is stopped for an unpaid contract invoice, can still buy. No contract is needed.  An `Idempotency-Key` is required, and it is what makes a retry safe: the same key with the same body returns the invoice already issued, the same key with a different body is refused with 422, and a duplicate that arrives while the first is still running is refused with 409. Use one key per purchase you mean to make, and a new key for the next one. At most 10 requests an hour.  Who may ask: the person who administers the partner, or a Widgetic administrator. A key limited to scopes needs `billing:write`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | Partner ID
$idempotency_key = 'idempotency_key_example'; // string | A key of your own for this purchase, so that a retry cannot make a second invoice
$request_extra_credits = new \WidgeticApi\Model\RequestExtraCredits(); // \WidgeticApi\Model\RequestExtraCredits

try {
    $result = $apiInstance->createPartnerExtraCreditsInvoice($partner_id, $idempotency_key, $request_extra_credits);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->createPartnerExtraCreditsInvoice: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| Partner ID | |
| **idempotency_key** | **string**| A key of your own for this purchase, so that a retry cannot make a second invoice | |
| **request_extra_credits** | [**\WidgeticApi\Model\RequestExtraCredits**](../Model/RequestExtraCredits.md)|  | |

### Return type

[**\WidgeticApi\Model\PartnerExtraCreditsInvoiceResponse**](../Model/PartnerExtraCreditsInvoiceResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createPublicCompositionEntry()`

```php
createPublicCompositionEntry($composition_id, $table, $public_composition_entry_request, $x_widgetic_write_token): \WidgeticApi\Model\PublicCompositionEntryCreated
```
### URI(s):
- https://api.widgetic.com The public embed routes are served at the root of the API host, not under /v1.
Append a visitor entry through the gateway

Public append-only write into a published composition database. No API key. The browser must send a permitted `Origin` header (the artifact iframe origin or a website the owner allowed). When the request comes from the shared artifact origin, it must also carry the per-composition write token (`X-Widgetic-Write-Token` header or `writeToken` body field, handed to the widget in `widgetic:host` as `entries.writeToken` and returned as `entryWriteToken` on `getPublicCompositionEmbed`). Host `context` is stored for partner attribution; it is not authenticated unless the partner signs it (see **Signed context**). Request bodies are limited to 16 KB before parsing. **Address.** `https://api.widgetic.com/embed/compositions/{compositionId}/entries/{table}`: the root of the API host, NOT under `/v1`. A client generated from this description for `https://api.widgetic.com/v1` must be given the base address `https://api.widgetic.com` for the calls of the `Public Embed` tag. **Signed context.** A partner that wants to trust `context` (to bill a customer by it, say) makes a signing secret (`rotatePartnerEntryContextSecret`), and its server signs the context it hands to the embed. The signature travels inside `context` as two reserved keys, `widgetic_exp` (UTC seconds, at most seven days ahead) and `widgetic_sig`. The gateway checks them after the `Origin` and before anything else is judged, stored or announced, and keeps and announces the context WITHOUT them. A context that is not signed as the partner requires is refused with 403 `CONTEXT_SIGNATURE_REQUIRED`, `CONTEXT_SIGNATURE_INVALID` or `CONTEXT_SIGNATURE_EXPIRED`; when the check cannot be made just now the answer is a retryable 503 `CONTEXT_SIGNATURE_UNAVAILABLE`, never an unchecked entry. Until a partner makes a secret nothing changes: the two keys are dropped and the rest is taken as it came. A signature is good until its `widgetic_exp` and may be used again until then, so a partner that must count each submission once keeps a unique value of its own (a `submissionId`, say) in the context. The recipe and a test vector are in the description of `rotatePartnerEntryContextSecret`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$composition_id = 'composition_id_example'; // string
$table = 'table_example'; // string
$public_composition_entry_request = new \WidgeticApi\Model\PublicCompositionEntryRequest(); // \WidgeticApi\Model\PublicCompositionEntryRequest
$x_widgetic_write_token = 'x_widgetic_write_token_example'; // string | Signed per-composition write token handed to the widget in `widgetic:host` as `entries.writeToken` (and returned by `GET /embed/compositions/{compositionId}` as `entryWriteToken`). Required when the request comes from the shared Widgetic artifact origin; verified whenever present.

$hostIndex = 0;
$variables = [
];

try {
    $result = $apiInstance->createPublicCompositionEntry($composition_id, $table, $public_composition_entry_request, $x_widgetic_write_token, $hostIndex, $variables);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->createPublicCompositionEntry: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **composition_id** | **string**|  | |
| **table** | **string**|  | |
| **public_composition_entry_request** | [**\WidgeticApi\Model\PublicCompositionEntryRequest**](../Model/PublicCompositionEntryRequest.md)|  | |
| **x_widgetic_write_token** | **string**| Signed per-composition write token handed to the widget in &#x60;widgetic:host&#x60; as &#x60;entries.writeToken&#x60; (and returned by &#x60;GET /embed/compositions/{compositionId}&#x60; as &#x60;entryWriteToken&#x60;). Required when the request comes from the shared Widgetic artifact origin; verified whenever present. | [optional] |
| hostIndex | null|int | Host index. Defaults to null. If null, then the library will use $this->hostIndex instead | [optional] |
| variables | array | Associative array of variables to pass to the host. Defaults to empty array. | [optional] |

### Return type

[**\WidgeticApi\Model\PublicCompositionEntryCreated**](../Model/PublicCompositionEntryCreated.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createUserApiKey()`

```php
createUserApiKey($id, $idempotency_key, $create_user_api_key_request): \WidgeticApi\Model\CreatedUserApiKeyResponse
```

Create an API key

Makes a new API key for an account and returns its secret in `key`. That is the only time the secret is shown: Widgetic keeps a hash, so a key that was not stored cannot be recovered, only replaced. To rotate a key, make the new one, switch the integration over to it, then delete the old one. Only a person signed in on widgetic.com can make a key: a request made with an API key, or with an SDK token, is refused with 403. That way a leaked key cannot be used to make a second one that survives its revocation. Make keys from the dashboard; a key can still list, rename, switch off and delete keys. An `Idempotency-Key` header is required (8 to 50 characters: letters, digits, `-` and `_`). A retry with the same header and the same body returns the same answer instead of making a second key, and the same header with a different body is refused with 422. Make keys one at a time: two requests for the same account that run at the same moment can overwrite each other. A key can be limited to what it needs. Send a `preset` (`read_only`, `content` or `full_access`) or a list of `scopes`, never both. Send neither for a key that can do everything its owner can, as every key made before scopes existed. A limited key is refused with 403 and the code `API_KEY_SCOPE_MISSING` on anything outside its scopes, so a key held by a build server or by a partner's backend can be given only the part of the API it uses. The scopes of a key are fixed when it is made: to widen one, make a new key and delete the old one. A limited key cannot make, change or delete keys, exchange tokens or reach the administration routes. The list of scopes is in the `ApiKeyScope` schema. Accounts with API access (Solo, Teams and partner accounts) have no limit on how many keys they hold. An account on a plan without API access cannot make one (a partner account is not asked about a plan).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The account the key is for. For your own, your own user id
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$create_user_api_key_request = new \WidgeticApi\Model\CreateUserApiKeyRequest(); // \WidgeticApi\Model\CreateUserApiKeyRequest

try {
    $result = $apiInstance->createUserApiKey($id, $idempotency_key, $create_user_api_key_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->createUserApiKey: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The account the key is for. For your own, your own user id | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **create_user_api_key_request** | [**\WidgeticApi\Model\CreateUserApiKeyRequest**](../Model/CreateUserApiKeyRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\CreatedUserApiKeyResponse**](../Model/CreatedUserApiKeyResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `createWidget()`

```php
createWidget($idempotency_key, $new_widget): \WidgeticApi\Model\CreateWidget201Response
```

Create Widget

Creates a widget for your account: a named record with a type and some starting content, on a canvas of its own (or one of yours that you name). It costs no credits and has no code yet; the code is generated for it afterwards. The new widget is yours, and you can list it with `getWidgets`. A widget is a draft until you say otherwise (`isDraft: false`).  If a step after the widget was saved does not go through, the widget is still created, and `data.warnings` says what did not. Read it before relying on the widget.  A widget can be placed on one of your canvases (`canvasId`), in a project you can edit (`projectId`) or in an organization where you may create widgets (`organizationId`). Naming anything you cannot use is refused with 403, and the answer is the same whether it exists or not.  To make the widget for one of your managed users, send `managedUserId` or `managedUserExternalId`. The widget stays in your account and is yours to edit; the tag lets you list one user's widgets with `getWidgets`. The managed user must be yours and active: one that is not yours, or does not exist, is answered with 404 and `MANAGED_USER_NOT_FOUND`, and one that is switched off with 409 and `MANAGED_USER_INACTIVE`. The tag is set here and does not change afterwards.  This call has a limit of its own: 120 per minute for each account (ask Widgetic if you need more). Past that the call is answered with 429 and a `Retry-After`. A widget has no database of its own: what the visitors of a composition leave is kept in the tables of that composition, made when the composition is. The `Idempotency-Key` header is required; send the same key when you retry, so one widget is created, not two.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$idempotency_key = 'idempotency_key_example'; // string | A unique value (a UUID is fine) that makes a retry of this request safe.
$new_widget = new \WidgeticApi\Model\NewWidget(); // \WidgeticApi\Model\NewWidget

try {
    $result = $apiInstance->createWidget($idempotency_key, $new_widget);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->createWidget: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **idempotency_key** | **string**| A unique value (a UUID is fine) that makes a retry of this request safe. | |
| **new_widget** | [**\WidgeticApi\Model\NewWidget**](../Model/NewWidget.md)|  | |

### Return type

[**\WidgeticApi\Model\CreateWidget201Response**](../Model/CreateWidget201Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteCanvas()`

```php
deleteCanvas($id): \WidgeticApi\Model\CanvasResponse
```

Delete Canvas

Deletes a canvas together with every widget on it.  Called with an editor session, only a canvas whose widgets were all made for the session's managed user can be deleted; one that also holds somebody else's widgets is refused with 409 and `CANVAS_HAS_OTHER_WIDGETS`, and nothing is deleted. Delete such a canvas with your API key.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the canvas

try {
    $result = $apiInstance->deleteCanvas($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->deleteCanvas: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the canvas | |

### Return type

[**\WidgeticApi\Model\CanvasResponse**](../Model/CanvasResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteComposition()`

```php
deleteComposition($id, $x_managed_user_id, $x_managed_user_external_id)
```

Delete Composition

Deletes a specific composition, and the data it keeps (the tables it declared and what visitors left in them).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The ID of the composition to delete
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $apiInstance->deleteComposition($id, $x_managed_user_id, $x_managed_user_external_id);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->deleteComposition: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The ID of the composition to delete | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

void (empty response body)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteCompositionContentItem()`

```php
deleteCompositionContentItem($id, $list, $item_id, $idempotency_key, $if_match, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\DeleteCompositionContentItemResponse
```

Delete a content list item

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$list = 'list_example'; // string
$item_id = 'item_id_example'; // string
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$if_match = 'if_match_example'; // string
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->deleteCompositionContentItem($id, $list, $item_id, $idempotency_key, $if_match, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->deleteCompositionContentItem: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **list** | **string**|  | |
| **item_id** | **string**|  | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **if_match** | **string**|  | [optional] |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\DeleteCompositionContentItemResponse**](../Model/DeleteCompositionContentItemResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteCompositionDataSource()`

```php
deleteCompositionDataSource($id, $idempotency_key, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\DeleteCompositionDataSourceResponse
```

Remove the composition data source binding

Removes the binding. Asking again, or asking for a composition that had none, is not an error: the composition has no data source afterwards, and that is all `removed: true` says.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->deleteCompositionDataSource($id, $idempotency_key, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->deleteCompositionDataSource: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\DeleteCompositionDataSourceResponse**](../Model/DeleteCompositionDataSourceResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteCompositionDatabaseRecord()`

```php
deleteCompositionDatabaseRecord($id, $table, $record_id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionDatabaseRecord201Response
```

Delete Record From Composition Database

Deletes a specific record from one of the composition's tables. Only the composition's own tables (made from its `databaseSchema` or from the tables its widget declares) can be reached; any other table name answers `404`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$table = 'table_example'; // string | Name of the database table
$record_id = 'record_id_example'; // string | ID of the record to delete
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->deleteCompositionDatabaseRecord($id, $table, $record_id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->deleteCompositionDatabaseRecord: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **table** | **string**| Name of the database table | |
| **record_id** | **string**| ID of the record to delete | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\CreateCompositionDatabaseRecord201Response**](../Model/CreateCompositionDatabaseRecord201Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteCompositionEntryItems()`

```php
deleteCompositionEntryItems($id, $table, $ids, $context, $filter, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CompositionEntryDeleteSuccess
```

Delete composition entry items by id or host context

Delete by comma-separated ids (1–100) or by context filters (not both). Rate limit 30 requests per minute.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$table = 'table_example'; // string
$ids = 'ids_example'; // string
$context = array('key' => 'context_example'); // array<string,string> | Host context filters as `context[key]=value` (max 5 keys, counting dotted `context.key` too). Use `column.<name>=value` for columns whose names collide with reserved parameters.
$filter = array('key' => 'filter_example'); // array<string,string> | Column filters as `filter[columnName]=value` (same meaning as bare `columnName=value` or `column.columnName=value`; max 10 column filters counting all spellings). A plain `filter=value` still filters a column named `filter`.
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->deleteCompositionEntryItems($id, $table, $ids, $context, $filter, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->deleteCompositionEntryItems: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **table** | **string**|  | |
| **ids** | **string**|  | [optional] |
| **context** | [**array<string,string>**](../Model/string.md)| Host context filters as &#x60;context[key]&#x3D;value&#x60; (max 5 keys, counting dotted &#x60;context.key&#x60; too). Use &#x60;column.&lt;name&gt;&#x3D;value&#x60; for columns whose names collide with reserved parameters. | [optional] |
| **filter** | [**array<string,string>**](../Model/string.md)| Column filters as &#x60;filter[columnName]&#x3D;value&#x60; (same meaning as bare &#x60;columnName&#x3D;value&#x60; or &#x60;column.columnName&#x3D;value&#x60;; max 10 column filters counting all spellings). A plain &#x60;filter&#x3D;value&#x60; still filters a column named &#x60;filter&#x60;. | [optional] |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\CompositionEntryDeleteSuccess**](../Model/CompositionEntryDeleteSuccess.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteManagedUser()`

```php
deleteManagedUser($id): \WidgeticApi\Model\DeleteManagedUser200Response
```

Delete Managed User

Deletes a managed user by ID. Its editor sessions end with it. What was filed under it (compositions, widgets, uploads) stays in your account, untagged.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the managed user to delete

try {
    $result = $apiInstance->deleteManagedUser($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->deleteManagedUser: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the managed user to delete | |

### Return type

[**\WidgeticApi\Model\DeleteManagedUser200Response**](../Model/DeleteManagedUser200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deletePersonalWorkspaceDomain()`

```php
deletePersonalWorkspaceDomain($id, $domain_id): \WidgeticApi\Model\DeletePersonalWorkspaceDomainResponse
```

Stop allowing a website to show your widgets

Removes one entry from an account's own list. When it was the last one, nothing is restricted any more and a widget can be shown anywhere again. A change can take about 15 seconds to reach every server.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The account the list belongs to. For your own, your own user id
$domain_id = 'domain_id_example'; // string | The `id` of the entry, as the list shows it

try {
    $result = $apiInstance->deletePersonalWorkspaceDomain($id, $domain_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->deletePersonalWorkspaceDomain: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The account the list belongs to. For your own, your own user id | |
| **domain_id** | **string**| The &#x60;id&#x60; of the entry, as the list shows it | |

### Return type

[**\WidgeticApi\Model\DeletePersonalWorkspaceDomainResponse**](../Model/DeletePersonalWorkspaceDomainResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `deleteUserApiKey()`

```php
deleteUserApiKey($id, $key_id): \WidgeticApi\Model\DeleteUserApiKeyResponse
```

Delete an API key

Deletes a key and the record of what it was used for. The key stops working at once on the server that took the request and within a minute on the others, and cannot be brought back: make a new one instead. To stop a key without losing it, switch it off with `updateUserApiKey`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The account the key belongs to
$key_id = 'key_id_example'; // string | The `keyId` of the key, as the list shows it

try {
    $result = $apiInstance->deleteUserApiKey($id, $key_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->deleteUserApiKey: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The account the key belongs to | |
| **key_id** | **string**| The &#x60;keyId&#x60; of the key, as the list shows it | |

### Return type

[**\WidgeticApi\Model\DeleteUserApiKeyResponse**](../Model/DeleteUserApiKeyResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `describeCompositionEntries()`

```php
describeCompositionEntries($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CompositionEntriesDescriptionResponse
```

Describe What a Composition Keeps

Names the tables a composition's widget keeps entries in (the votes, ratings, answers or sign-ups its visitors left), their columns, and how many entries each holds. Call it first to learn the table and column names that `readCompositionEntries` takes.  A widget that only shows content keeps nothing of its own: the answer is `hasData: false` with no tables, and that is not an error. A table that could not be counted has `rows: null`, which is not zero.  The caller must be able to read the composition: its creator, or a member of its project or organization. An editor session cannot call this route.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->describeCompositionEntries($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->describeCompositionEntries: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\CompositionEntriesDescriptionResponse**](../Model/CompositionEntriesDescriptionResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `duplicateComposition()`

```php
duplicateComposition($id, $idempotency_key, $x_managed_user_id, $x_managed_user_external_id, $duplicate_composition_request): \WidgeticApi\Model\DuplicateComposition202Response
```

Duplicate Composition

Creates a duplicate of an existing composition for the authenticated user.  The duplicate is made after the answer: the call returns `202` with an `operationId`. Ask `GET /operations/{id}` for that operation until its `status` is `completed`; the new composition is named in `metadata.newCompositionId`. A problem with the duplicate's database (for example, tables that could not be made just now) is listed in `metadata.warnings`, which is absent when there is none.  The `Idempotency-Key` header is required (`400` without it). Send the same key when you retry, so one duplicate is made, not two.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition to duplicate
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$duplicate_composition_request = new \WidgeticApi\Model\DuplicateCompositionRequest(); // \WidgeticApi\Model\DuplicateCompositionRequest

try {
    $result = $apiInstance->duplicateComposition($id, $idempotency_key, $x_managed_user_id, $x_managed_user_external_id, $duplicate_composition_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->duplicateComposition: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition to duplicate | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **duplicate_composition_request** | [**\WidgeticApi\Model\DuplicateCompositionRequest**](../Model/DuplicateCompositionRequest.md)|  | [optional] |

### Return type

[**\WidgeticApi\Model\DuplicateComposition202Response**](../Model/DuplicateComposition202Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `exportCompositionEntryItems()`

```php
exportCompositionEntryItems($id, $table, $format, $order, $since, $until, $context, $filter, $x_managed_user_id, $x_managed_user_external_id): string
```

Export composition entry items

Streams up to 50,000 matching rows in batches of 1,000. Tables without cursor paging export at most one batch; when more rows exist the response sets `X-Widgetic-Export-Truncated: true`. Rate limit 20 requests per minute.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$table = 'table_example'; // string
$format = 'csv'; // string
$order = 'desc'; // string | `desc` (the default) lists the newest entry first, `asc` the oldest. Entries are sorted by their time, then by their id (compared as text, byte by byte) in the same direction, so the order of two entries made at the same instant is always the same; an entry with no time counts as the oldest. A table with no time column is sorted by its id. The managed-user feed sorts by time, then by composition id, table and id.
$since = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Only entries made at this time or later: `since` is INCLUSIVE (an entry made at exactly `since` is returned). A date and time with an offset, such as `2026-10-01T00:00:00Z`; anything else answers 400 `INVALID_SINCE`. An entry with no time never matches, and a table with no time column answers 400 `ENTRY_TABLE_HAS_NO_TIME`.
$until = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Only entries made before this time: `until` is EXCLUSIVE (an entry made at exactly `until` is NOT returned), so `since=A&until=B` followed by `since=B&until=C` counts every entry once. Same form and same refusals as `since` (400 `INVALID_UNTIL`).
$context = array('key' => 'context_example'); // array<string,string> | Host context filters as `context[key]=value` (max 5 keys, counting dotted `context.key` too). Use `column.<name>=value` for columns whose names collide with reserved parameters.
$filter = array('key' => 'filter_example'); // array<string,string> | Column filters as `filter[columnName]=value` (same meaning as bare `columnName=value` or `column.columnName=value`; max 10 column filters counting all spellings). A plain `filter=value` still filters a column named `filter`.
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->exportCompositionEntryItems($id, $table, $format, $order, $since, $until, $context, $filter, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->exportCompositionEntryItems: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **table** | **string**|  | |
| **format** | **string**|  | [optional] [default to &#39;csv&#39;] |
| **order** | **string**| &#x60;desc&#x60; (the default) lists the newest entry first, &#x60;asc&#x60; the oldest. Entries are sorted by their time, then by their id (compared as text, byte by byte) in the same direction, so the order of two entries made at the same instant is always the same; an entry with no time counts as the oldest. A table with no time column is sorted by its id. The managed-user feed sorts by time, then by composition id, table and id. | [optional] [default to &#39;desc&#39;] |
| **since** | **\DateTime**| Only entries made at this time or later: &#x60;since&#x60; is INCLUSIVE (an entry made at exactly &#x60;since&#x60; is returned). A date and time with an offset, such as &#x60;2026-10-01T00:00:00Z&#x60;; anything else answers 400 &#x60;INVALID_SINCE&#x60;. An entry with no time never matches, and a table with no time column answers 400 &#x60;ENTRY_TABLE_HAS_NO_TIME&#x60;. | [optional] |
| **until** | **\DateTime**| Only entries made before this time: &#x60;until&#x60; is EXCLUSIVE (an entry made at exactly &#x60;until&#x60; is NOT returned), so &#x60;since&#x3D;A&amp;until&#x3D;B&#x60; followed by &#x60;since&#x3D;B&amp;until&#x3D;C&#x60; counts every entry once. Same form and same refusals as &#x60;since&#x60; (400 &#x60;INVALID_UNTIL&#x60;). | [optional] |
| **context** | [**array<string,string>**](../Model/string.md)| Host context filters as &#x60;context[key]&#x3D;value&#x60; (max 5 keys, counting dotted &#x60;context.key&#x60; too). Use &#x60;column.&lt;name&gt;&#x3D;value&#x60; for columns whose names collide with reserved parameters. | [optional] |
| **filter** | [**array<string,string>**](../Model/string.md)| Column filters as &#x60;filter[columnName]&#x3D;value&#x60; (same meaning as bare &#x60;columnName&#x3D;value&#x60; or &#x60;column.columnName&#x3D;value&#x60;; max 10 column filters counting all spellings). A plain &#x60;filter&#x3D;value&#x60; still filters a column named &#x60;filter&#x60;. | [optional] |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

**string**

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `text/csv`, `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getAiAnswersKnowledge()`

```php
getAiAnswersKnowledge($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetAiAnswersKnowledge200Response
```

See the documents a widget's AI answers from

The `ai-answers` adapter lets a widget answer a visitor's question with text an AI model writes from documents the widget's owner provides. This lists those documents, and how much room is left for more: `totals` carries the widget's limits next to what it uses.  The list never contains what a document says, only which documents there are: their title, size and state. A `processing` document is not used to answer questions yet (or an add of it was interrupted: remove it and add it again).  Add a document with `addAiAnswersKnowledgeDocument`; remove one with `removeAiAnswersKnowledgeDocument`.  The caller must be allowed to see the widget: its owner, a partner for a customer it manages, or a Widgetic administrator. An API key needs the `content:read` scope.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The widget (composition) whose documents to list
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getAiAnswersKnowledge($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getAiAnswersKnowledge: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The widget (composition) whose documents to list | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\GetAiAnswersKnowledge200Response**](../Model/GetAiAnswersKnowledge200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getAllCanvases()`

```php
getAllCanvases($page, $size, $sort, $created_after, $created_before, $updated_after, $updated_before, $managed_user_id, $managed_user_external_id): \WidgeticApi\Model\GetAllCanvasesResponse
```

Get All Canvases

Retrieves all canvases with pagination support and filtering options.  Pass `managedUserId` (Widgetic's id for one of your managed users) or `managedUserExternalId` (your own identifier for the user) to list only the canvases made for that managed user. The canvases of your other managed users, and your own, are left out. A managed user that is not yours, or does not exist, is answered with 404 and `MANAGED_USER_NOT_FOUND`. Called with an editor session, the list is always the session's managed user's.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$page = 1; // int | Page number for pagination
$size = 20; // int | Number of items per page
$sort = 'created_at:desc'; // string | Sort field and direction (e.g., \"created_at:desc\")
$created_after = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Filter canvases created after the specified date (ISO 8601 format)
$created_before = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Filter canvases created before the specified date (ISO 8601 format)
$updated_after = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Filter canvases updated after the specified date (ISO 8601 format)
$updated_before = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Filter canvases updated before the specified date (ISO 8601 format)
$managed_user_id = 'managed_user_id_example'; // string | List only the canvases made for this managed user (Widgetic's id for the user). Send this or `managedUserExternalId`, not both.
$managed_user_external_id = 'managed_user_external_id_example'; // string | List only the canvases made for the managed user you registered with this `externalId` (your own identifier for the user). Send this or `managedUserId`, not both.

try {
    $result = $apiInstance->getAllCanvases($page, $size, $sort, $created_after, $created_before, $updated_after, $updated_before, $managed_user_id, $managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getAllCanvases: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **int**| Page number for pagination | [optional] [default to 1] |
| **size** | **int**| Number of items per page | [optional] [default to 20] |
| **sort** | **string**| Sort field and direction (e.g., \&quot;created_at:desc\&quot;) | [optional] [default to &#39;created_at:desc&#39;] |
| **created_after** | **\DateTime**| Filter canvases created after the specified date (ISO 8601 format) | [optional] |
| **created_before** | **\DateTime**| Filter canvases created before the specified date (ISO 8601 format) | [optional] |
| **updated_after** | **\DateTime**| Filter canvases updated after the specified date (ISO 8601 format) | [optional] |
| **updated_before** | **\DateTime**| Filter canvases updated before the specified date (ISO 8601 format) | [optional] |
| **managed_user_id** | **string**| List only the canvases made for this managed user (Widgetic&#39;s id for the user). Send this or &#x60;managedUserExternalId&#x60;, not both. | [optional] |
| **managed_user_external_id** | **string**| List only the canvases made for the managed user you registered with this &#x60;externalId&#x60; (your own identifier for the user). Send this or &#x60;managedUserId&#x60;, not both. | [optional] |

### Return type

[**\WidgeticApi\Model\GetAllCanvasesResponse**](../Model/GetAllCanvasesResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getAllCompositions()`

```php
getAllCompositions($page, $size, $sort, $widget_id, $workspace, $project_folder, $status, $managed_user_id, $managed_user_external_id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetAllCompositions200Response
```

Get All Compositions

Retrieves all compositions with pagination support.  Pass `managedUserId` (Widgetic's id for one of your managed users) or `managedUserExternalId` (your own identifier for the user) to list only the compositions made for that managed user. The compositions of your other managed users, and your own, are left out. It combines with the other filters and with paging. A managed user that is not yours, or does not exist, is answered with 404 and `MANAGED_USER_NOT_FOUND`.  An editor session with the `creator` surface may call this to list the compositions of ONE widget it built: it must send `widgetId`, and the answer holds only the compositions made for the session's managed user.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$page = 1; // int | Page number for pagination
$size = 20; // int | Number of items per page
$sort = createdAt:desc; // string | The order of the list, as `<field>:<asc|desc>`. The field is `createdAt`, `updatedAt`, `name` or `status` (the snake_case spelling, such as `created_at`, is read too). `asc` or `desc` alone orders by `createdAt`. Default: `createdAt:desc`. Any other field is a 400.
$widget_id = 'widget_id_example'; // string | Filter compositions by widget ID
$workspace = 'workspace_example'; // string | Filter by workspace
$project_folder = 'project_folder_example'; // string | Only the compositions in this project (the project's id).
$status = 'status_example'; // string | Only the compositions in this status. Without it, every status is listed.
$managed_user_id = 'managed_user_id_example'; // string | List only the compositions made for this managed user (Widgetic's id for the user). Send this or `managedUserExternalId`, not both. Send it as `managedUserId`; the snake_case spelling `managed_user_id` is refused with a 400, not ignored.
$managed_user_external_id = 'managed_user_external_id_example'; // string | List only the compositions made for the managed user you registered with this `externalId` (your own identifier for the user). Send this or `managedUserId`, not both.
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getAllCompositions($page, $size, $sort, $widget_id, $workspace, $project_folder, $status, $managed_user_id, $managed_user_external_id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getAllCompositions: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **int**| Page number for pagination | [optional] [default to 1] |
| **size** | **int**| Number of items per page | [optional] [default to 20] |
| **sort** | **string**| The order of the list, as &#x60;&lt;field&gt;:&lt;asc|desc&gt;&#x60;. The field is &#x60;createdAt&#x60;, &#x60;updatedAt&#x60;, &#x60;name&#x60; or &#x60;status&#x60; (the snake_case spelling, such as &#x60;created_at&#x60;, is read too). &#x60;asc&#x60; or &#x60;desc&#x60; alone orders by &#x60;createdAt&#x60;. Default: &#x60;createdAt:desc&#x60;. Any other field is a 400. | [optional] |
| **widget_id** | **string**| Filter compositions by widget ID | [optional] |
| **workspace** | **string**| Filter by workspace | [optional] |
| **project_folder** | **string**| Only the compositions in this project (the project&#39;s id). | [optional] |
| **status** | **string**| Only the compositions in this status. Without it, every status is listed. | [optional] |
| **managed_user_id** | **string**| List only the compositions made for this managed user (Widgetic&#39;s id for the user). Send this or &#x60;managedUserExternalId&#x60;, not both. Send it as &#x60;managedUserId&#x60;; the snake_case spelling &#x60;managed_user_id&#x60; is refused with a 400, not ignored. | [optional] |
| **managed_user_external_id** | **string**| List only the compositions made for the managed user you registered with this &#x60;externalId&#x60; (your own identifier for the user). Send this or &#x60;managedUserId&#x60;, not both. | [optional] |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\GetAllCompositions200Response**](../Model/GetAllCompositions200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getAllManagedUsers()`

```php
getAllManagedUsers($page, $size, $sort): \WidgeticApi\Model\GetAllManagedUsers200Response
```

Get Managed Users

Retrieve the managed users you manage, with pagination support. (Admins see every partner's managed users.)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$page = 1; // int | Page number for pagination
$size = 10; // int | Number of items per page
$sort = 'createdAt:desc'; // string | Sort field and direction, `<field>:<asc|desc>`. The field is `createdAt`, `updatedAt` or `externalId` (the snake_case spellings `created_at`, `updated_at` and `external_id` work too); `asc` or `desc` alone sorts by `createdAt`. Any other field is a 400.

try {
    $result = $apiInstance->getAllManagedUsers($page, $size, $sort);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getAllManagedUsers: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **int**| Page number for pagination | [optional] [default to 1] |
| **size** | **int**| Number of items per page | [optional] [default to 10] |
| **sort** | **string**| Sort field and direction, &#x60;&lt;field&gt;:&lt;asc|desc&gt;&#x60;. The field is &#x60;createdAt&#x60;, &#x60;updatedAt&#x60; or &#x60;externalId&#x60; (the snake_case spellings &#x60;created_at&#x60;, &#x60;updated_at&#x60; and &#x60;external_id&#x60; work too); &#x60;asc&#x60; or &#x60;desc&#x60; alone sorts by &#x60;createdAt&#x60;. Any other field is a 400. | [optional] [default to &#39;createdAt:desc&#39;] |

### Return type

[**\WidgeticApi\Model\GetAllManagedUsers200Response**](../Model/GetAllManagedUsers200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCanvas()`

```php
getCanvas($id): \WidgeticApi\Model\CanvasResponse
```

Get Canvas

Retrieves a specific canvas by ID.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the canvas

try {
    $result = $apiInstance->getCanvas($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getCanvas: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the canvas | |

### Return type

[**\WidgeticApi\Model\CanvasResponse**](../Model/CanvasResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCompositionById()`

```php
getCompositionById($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionFromWidget201Response
```

Get Composition

Retrieves a specific composition by its ID.  The answer carries `direct`, which says whether the widget the composition is made from is drawn straight into your page (`true`) or inside a frame (`false`), or `null` while the widget has no published version. Read it before you go live: a widget drawn without a frame writes its entries from your own page, so the public entry route accepts them only from a website on the composition's allowed list, and refuses them while that list is empty (the public JSON of the composition stays open to every website). A widget in a frame writes from Widgetic's own frame and is accepted whatever the list says.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | Composition ID
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionById($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getCompositionById: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| Composition ID | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\CreateCompositionFromWidget201Response**](../Model/CreateCompositionFromWidget201Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCompositionContent()`

```php
getCompositionContent($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionContentResponse
```

Get Current Content

Retrieves the current content of a composition

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionContent($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getCompositionContent: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\GetCompositionContentResponse**](../Model/GetCompositionContentResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCompositionContentSchema()`

```php
getCompositionContentSchema($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionContentSchemaResponse
```

Get Content Schema

Retrieves the content schema for a composition based on its widget type

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionContentSchema($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getCompositionContentSchema: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\GetCompositionContentSchemaResponse**](../Model/GetCompositionContentSchemaResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCompositionDataSource()`

```php
getCompositionDataSource($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionDataSourceResponse
```

Read the composition data source binding

The data source that is bound to the composition: `url` and `refreshSeconds`. The answer's `data` is `null` when none is bound, and also when what is stored does not pass the rule for a public https address (a binding written by another path, such as the general embed-settings update, is never shown to a page unless it passes the same checks as this route).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionDataSource($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getCompositionDataSource: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\GetCompositionDataSourceResponse**](../Model/GetCompositionDataSourceResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCompositionDatabaseRecord()`

```php
getCompositionDatabaseRecord($id, $table, $record_id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionDatabaseRecord201Response
```

Get Record From Composition Database

Retrieves a specific record from one of the composition's tables. Only the composition's own tables (made from its `databaseSchema` or from the tables its widget declares) can be reached; any other table name answers `404`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$table = 'table_example'; // string | Name of the database table
$record_id = 'record_id_example'; // string | ID of the record to retrieve
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionDatabaseRecord($id, $table, $record_id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getCompositionDatabaseRecord: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **table** | **string**| Name of the database table | |
| **record_id** | **string**| ID of the record to retrieve | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\CreateCompositionDatabaseRecord201Response**](../Model/CreateCompositionDatabaseRecord201Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCompositionDatabaseRecords()`

```php
getCompositionDatabaseRecords($id, $table, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionDatabaseRecords200Response
```

Get All Records From Composition Database Table

Retrieves all records from one of the composition's tables. Only the composition's own tables (made from its `databaseSchema` or from the tables its widget declares) can be reached; any other table name answers `404`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$table = 'table_example'; // string | Name of the database table
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionDatabaseRecords($id, $table, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getCompositionDatabaseRecords: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **table** | **string**| Name of the database table | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\GetCompositionDatabaseRecords200Response**](../Model/GetCompositionDatabaseRecords200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCompositionDesign()`

```php
getCompositionDesign($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionDesignResponse
```

Get Composition Design

Retrieves only the design field from a composition.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionDesign($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getCompositionDesign: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\GetCompositionDesignResponse**](../Model/GetCompositionDesignResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCompositionDesignSchema()`

```php
getCompositionDesignSchema($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionDesignSchemaResponse
```

Get Design Schema

Retrieves the design schema for a composition based on its widget type

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionDesignSchema($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getCompositionDesignSchema: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\GetCompositionDesignSchemaResponse**](../Model/GetCompositionDesignSchemaResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCompositionEmbedSchema()`

```php
getCompositionEmbedSchema($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionEmbedSchemaResponse
```

Get Embed Schema

Retrieves the definition of the composition's Embed tab: which settings exist, what each one holds, what it defaults to, and when its control is shown. It is the third tab beside `schema/content` and `schema/design`, in the same format (`componentGroups` → `components` → `propertyGroups` → `properties`, each property with a `type`, a `defaultValue` and an `inputController`), so a client that draws those two tabs draws this one with the same code.  The schema is the same for every composition (it is the one Widgetic's own Embed Editor draws). The composition id decides who may ask: the caller must be able to read the composition.  Reading and saving the values: - `GET /compositions/{id}/embed-settings` returns what the composition saved. A composition whose Embed tab   was never saved has nothing to return; seed the form from `defaults`, which holds the `defaultValue` of   every setting that declares one. - `PUT /compositions/{id}` with `embedSettings` saves them. The gateway stores `embedSettings` as given and   does not check it against this schema; the schema is how a client knows what to put there.  A property's `visibilityCondition` says when its control is shown: `condition` is a comparison of the current values of the properties named in `dependsOn` (`useIframe === false`, `embedTarget === 'mixed' && keepDimensions === false`). While it is false the Embed Editor does not show the control.  A colour picker with `showOpacityControls` saves its opacity next to the colour, under the key `<name>_opacity` as a number from 0 to 1 (`overlayBackgroundColor` → `overlayBackgroundColor_opacity`). Its `defaultTransparency` is a percentage and the saved value a fraction (50 → 0.5).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionEmbedSchema($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getCompositionEmbedSchema: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\GetCompositionEmbedSchemaResponse**](../Model/GetCompositionEmbedSchemaResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCompositionEmbedSettings()`

```php
getCompositionEmbedSettings($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionEmbedSettingsResponse
```

Get Composition Embed Settings

Retrieves only the embedSettings field from a composition.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionEmbedSettings($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getCompositionEmbedSettings: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\GetCompositionEmbedSettingsResponse**](../Model/GetCompositionEmbedSettingsResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCompositionPreview()`

```php
getCompositionPreview($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionPreviewResponse
```

Get Composition Preview

Returns the address of the page an editor shows the composition in: the page of the widget's published version on the CDN, with the widget and version it is. Load it in a frame, then send the frame what to show (the content, design and embed settings you read from the composition, and every change the user makes) with `postMessage`: `{ type: 'widgetic:update', design }`, `{ type: 'widgetic:update', content }` or `{ type: 'widgetic:update', contentItems }`.  The version is the one embeds show, so the editor previews what a visitor gets. The address does not carry the composition id: an embed uses the id to fetch the saved composition itself, while an editor sends the current state (unsaved changes included).  A widget that has never been published has no page to show: the answer is 409 `WIDGET_NOT_PUBLISHED`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionPreview($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getCompositionPreview: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\GetCompositionPreviewResponse**](../Model/GetCompositionPreviewResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCompositionVersions()`

```php
getCompositionVersions($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionVersions200Response
```

Get Composition Versions

Retrieves version history for a specific composition.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | Composition ID
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionVersions($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getCompositionVersions: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| Composition ID | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\GetCompositionVersions200Response**](../Model/GetCompositionVersions200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getCompositionsBatch()`

```php
getCompositionsBatch($get_compositions_batch_request): \WidgeticApi\Model\GetCompositionsBatchResponse
```

Get Compositions Batch

Retrieves multiple compositions by their IDs in a single request. This endpoint includes domain validation for embed contexts and is used by the embed SDK.  Each composition is checked on its own. If its owner listed the websites it may appear on (the workspace's domain list, or the `allowedDomains` of a partner the owner administers) and the request comes from another website (the `Origin` header, or the host of `Referer` when there is no `Origin`), that composition is left out of `compositions` and reported in `errors` as `Domain access denied: <reason>`; the others are still returned. A request that names no website, and an owner who listed nothing, are not restricted, and a page on the visitor's own machine (`localhost`, `127.0.0.1` or `[::1]`, on any port) is always allowed. So is the website where a partner integrates Widgetic, with every subdomain of it (`platformDomain` in the answer of `GET /partners/mine`), for the compositions of that partner: a partner's list never has to name it.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$get_compositions_batch_request = new \WidgeticApi\Model\GetCompositionsBatchRequest(); // \WidgeticApi\Model\GetCompositionsBatchRequest

try {
    $result = $apiInstance->getCompositionsBatch($get_compositions_batch_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getCompositionsBatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **get_compositions_batch_request** | [**\WidgeticApi\Model\GetCompositionsBatchRequest**](../Model/GetCompositionsBatchRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\GetCompositionsBatchResponse**](../Model/GetCompositionsBatchResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getInvoicesByPartnerId()`

```php
getInvoicesByPartnerId($partner_id, $status, $limit, $offset): \WidgeticApi\Model\GetInvoicesByPartnerId200Response
```

List a partner's invoices

Lists the invoices issued to a partner, newest first. Each carries the price (`subtotal`), the tax on it (`taxAmount`) and what is paid (`total`), its status as the payment provider reports it, why the last payment failed (`failureReason`), and the page where it is paid (`hostedInvoiceUrl`).  A partner reads its own: the caller must be the person who administers the partner (an API key of that account works), and anyone else is refused with 403 whether or not the partner exists. Widgetic administrators can read any partner's and see exactly what the partner sees; the full records, with the internal fields, are `getAllInvoices` filtered by partner.  The page is always bounded: `limit` defaults to 50 and is capped at 100, `offset` defaults to 0.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose invoices to list
$status = 'status_example'; // string | Only invoices with this status
$limit = 50; // int | Maximum number of invoices to return
$offset = 0; // int | Number of invoices to skip

try {
    $result = $apiInstance->getInvoicesByPartnerId($partner_id, $status, $limit, $offset);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getInvoicesByPartnerId: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose invoices to list | |
| **status** | **string**| Only invoices with this status | [optional] |
| **limit** | **int**| Maximum number of invoices to return | [optional] [default to 50] |
| **offset** | **int**| Number of invoices to skip | [optional] [default to 0] |

### Return type

[**\WidgeticApi\Model\GetInvoicesByPartnerId200Response**](../Model/GetInvoicesByPartnerId200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getManagedUserById()`

```php
getManagedUserById($id): \WidgeticApi\Model\ManagedUserResponse
```

Get Managed User By ID

Retrieves a specific managed user by ID.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the managed user to retrieve

try {
    $result = $apiInstance->getManagedUserById($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getManagedUserById: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the managed user to retrieve | |

### Return type

[**\WidgeticApi\Model\ManagedUserResponse**](../Model/ManagedUserResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getManagedUserDesignDefaults()`

```php
getManagedUserDesignDefaults($id): \WidgeticApi\Model\GetPartnerDesignDefaults200Response
```

Read design defaults for one managed user

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string

try {
    $result = $apiInstance->getManagedUserDesignDefaults($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getManagedUserDesignDefaults: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

[**\WidgeticApi\Model\GetPartnerDesignDefaults200Response**](../Model/GetPartnerDesignDefaults200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getManagedUserEntitlements()`

```php
getManagedUserEntitlements($managed_user_id, $include_expired, $feature, $source): \WidgeticApi\Model\GetManagedUserEntitlementsResponse
```

Get managed user entitlements

Retrieves all entitlements for a managed user (admin or partner access).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$managed_user_id = 'managed_user_id_example'; // string | Managed user ID
$include_expired = True; // bool | Include expired entitlements in results
$feature = 'feature_example'; // string | Filter by specific feature
$source = 'source_example'; // string | Filter by entitlement source

try {
    $result = $apiInstance->getManagedUserEntitlements($managed_user_id, $include_expired, $feature, $source);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getManagedUserEntitlements: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **managed_user_id** | **string**| Managed user ID | |
| **include_expired** | **bool**| Include expired entitlements in results | [optional] |
| **feature** | **string**| Filter by specific feature | [optional] |
| **source** | **string**| Filter by entitlement source | [optional] |

### Return type

[**\WidgeticApi\Model\GetManagedUserEntitlementsResponse**](../Model/GetManagedUserEntitlementsResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getManagedUserLimits()`

```php
getManagedUserLimits($id): \WidgeticApi\Model\GetManagedUserLimits200Response
```

Read monthly credit cap and usage for one managed user

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string

try {
    $result = $apiInstance->getManagedUserLimits($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getManagedUserLimits: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

[**\WidgeticApi\Model\GetManagedUserLimits200Response**](../Model/GetManagedUserLimits200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getManagedUserStorageUsage()`

```php
getManagedUserStorageUsage($id): \WidgeticApi\Model\GetManagedUserStorageUsage200Response
```

Storage used by one managed user's uploads

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string

try {
    $result = $apiInstance->getManagedUserStorageUsage($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getManagedUserStorageUsage: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

[**\WidgeticApi\Model\GetManagedUserStorageUsage200Response**](../Model/GetManagedUserStorageUsage200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getManagedUserUsage()`

```php
getManagedUserUsage($id, $start_date, $end_date): \WidgeticApi\Model\ManagedUserUsageResponse
```

What a managed user's editor sessions spent

Says how many credits the editor sessions of one of your managed users took from your account over a period, in total and for each operation. A generation costs one credit, taken from your account when it starts; one that fails is refunded and is counted as refunded, not as spent.  Only what was spent through editor sessions is here, and only since usage was first recorded: what you spend with your API key, and anything from before, is not. Use it to see which of your users spend the most, or to charge them for it. To hold one session to a number of credits, set `max_credits` when you make it (`createManagedUserEditorSession`).  The period runs from `startDate` (included) to `endDate` (not included): the 30 days before now when you give neither, and at most 366 days. A date without a time is midnight UTC at the start of that day, so for all of October give `startDate=2026-10-01` and `endDate=2026-11-01`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The managed user whose usage you want (Widgetic's id for the user)
$start_date = 'start_date_example'; // string | Start of the period, included: an ISO 8601 date (`2026-10-01`) or date-time with its offset (`2026-10-01T08:00:00Z`). Default: 30 days before `endDate`.
$end_date = 'end_date_example'; // string | End of the period, not included, in the same forms. Default: now. It must be after `startDate`, by at most 366 days.

try {
    $result = $apiInstance->getManagedUserUsage($id, $start_date, $end_date);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getManagedUserUsage: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The managed user whose usage you want (Widgetic&#39;s id for the user) | |
| **start_date** | **string**| Start of the period, included: an ISO 8601 date (&#x60;2026-10-01&#x60;) or date-time with its offset (&#x60;2026-10-01T08:00:00Z&#x60;). Default: 30 days before &#x60;endDate&#x60;. | [optional] |
| **end_date** | **string**| End of the period, not included, in the same forms. Default: now. It must be after &#x60;startDate&#x60;, by at most 366 days. | [optional] |

### Return type

[**\WidgeticApi\Model\ManagedUserUsageResponse**](../Model/ManagedUserUsageResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getManagedUsersByManagerId()`

```php
getManagedUsersByManagerId($manager_id, $page, $size, $sort): \WidgeticApi\Model\GetManagedUsersByManagerIdResponse
```

Get Managed Users By Manager

Retrieve managed users for a specific manager with pagination support.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$manager_id = 'manager_id_example'; // string | ID of the manager
$page = 1; // int | Page number for pagination
$size = 10; // int | Number of items per page
$sort = 'createdAt:desc'; // string | Sort field and direction, `<field>:<asc|desc>`. The field is `createdAt`, `updatedAt` or `externalId` (the snake_case spellings `created_at`, `updated_at` and `external_id` work too); `asc` or `desc` alone sorts by `createdAt`. Any other field is a 400.

try {
    $result = $apiInstance->getManagedUsersByManagerId($manager_id, $page, $size, $sort);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getManagedUsersByManagerId: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **manager_id** | **string**| ID of the manager | |
| **page** | **int**| Page number for pagination | [optional] [default to 1] |
| **size** | **int**| Number of items per page | [optional] [default to 10] |
| **sort** | **string**| Sort field and direction, &#x60;&lt;field&gt;:&lt;asc|desc&gt;&#x60;. The field is &#x60;createdAt&#x60;, &#x60;updatedAt&#x60; or &#x60;externalId&#x60; (the snake_case spellings &#x60;created_at&#x60;, &#x60;updated_at&#x60; and &#x60;external_id&#x60; work too); &#x60;asc&#x60; or &#x60;desc&#x60; alone sorts by &#x60;createdAt&#x60;. Any other field is a 400. | [optional] [default to &#39;createdAt:desc&#39;] |

### Return type

[**\WidgeticApi\Model\GetManagedUsersByManagerIdResponse**](../Model/GetManagedUsersByManagerIdResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getMyPartners()`

```php
getMyPartners(): \WidgeticApi\Model\MyPartnersResponse
```

Find the partner you administer

Returns the partner (nearly always one) that the signed-in account administers, with the id every other partner route asks for and the standing it is in: `active`, `inactive` (not activated yet), `suspended` (paused, with the reason Widgetic gave) or `payment_arrears` (a contract invoice is past its due date and unpaid, since `overdueSince`; the partner is stopped until it is paid). A partner API key is that account's key, so it reads its own partner here.  An account that administers no partner is not refused: it gets `standing: not_a_partner` and an empty list, so a dashboard can tell \"this is not a partner account\" from \"something failed\".  The call stays open while the partner is paused, not yet active or in payment arrears: that is when its dashboard has to say why.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->getMyPartners();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getMyPartners: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\WidgeticApi\Model\MyPartnersResponse**](../Model/MyPartnersResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerAdapterConnections()`

```php
getPartnerAdapterConnections($partner_id): \WidgeticApi\Model\GetUserAdapterConnections200Response
```

See which adapter keys a partner has connected

Widget adapters are capabilities a widget can use, and some of them act through a service the account that made the widget has with a provider: an adapter that sends email needs an email provider key, one that sends texts needs an SMS provider key. For the widgets of the customers a partner manages, those keys are the partner's. This lists every key an adapter takes from a partner and whether the partner has connected it.  An empty list means no adapter takes a key from a partner at the moment. The list never contains a key: only whether one is connected and when it was last set.  Connect a key with `setPartnerAdapterConnection`; take it away with `removePartnerAdapterConnection`. A managed customer never holds a key: the widgets of a managed customer use the partner's, and never the personal key of the person who administers the partner.  The caller must be the person who administers the partner (an API key of that account works, with the `partner:read` scope), or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose adapter keys to list

try {
    $result = $apiInstance->getPartnerAdapterConnections($partner_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerAdapterConnections: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose adapter keys to list | |

### Return type

[**\WidgeticApi\Model\GetUserAdapterConnections200Response**](../Model/GetUserAdapterConnections200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerAnalyticsByManagedUser()`

```php
getPartnerAnalyticsByManagedUser($partner_id, $start_date, $end_date, $limit, $offset): \WidgeticApi\Model\PartnerAnalyticsByManagedUserResponse
```

What each managed user's widgets did

Lists every one of your managed users with what their widgets and compositions did in a period: views, interactions and visitors, and how many widgets and compositions they have made. A managed user whose widgets were not viewed is listed too, with zeros. The most viewed come first, and `page.hasMore` says whether more follow.  Only the compositions made for a managed user count for it: file them under the user when you create them (`managedUserId` on `createComposition`), or let the user's editor session do it, which files everything under its user. What a visitor did with a composition that is not filed under anyone is in the summary of the whole account (`getPartnerAnalyticsSummary`) and in no managed user's row.  The period works as it does for `getPartnerAnalyticsSummary`. The caller must be the person who administers the partner (an API key of that account works, with the `partner:read` scope), or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose managed users to report on
$start_date = 'start_date_example'; // string | Start of the period, included. An ISO 8601 date (`2026-10-01`) or date-time with its offset. Default 30 days before `endDate`.
$end_date = 'end_date_example'; // string | End of the period, not included, in the same forms. Default now. At most 366 days after `startDate`.
$limit = 50; // int | How many managed users to list at most
$offset = 0; // int | How many managed users to skip

try {
    $result = $apiInstance->getPartnerAnalyticsByManagedUser($partner_id, $start_date, $end_date, $limit, $offset);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerAnalyticsByManagedUser: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose managed users to report on | |
| **start_date** | **string**| Start of the period, included. An ISO 8601 date (&#x60;2026-10-01&#x60;) or date-time with its offset. Default 30 days before &#x60;endDate&#x60;. | [optional] |
| **end_date** | **string**| End of the period, not included, in the same forms. Default now. At most 366 days after &#x60;startDate&#x60;. | [optional] |
| **limit** | **int**| How many managed users to list at most | [optional] [default to 50] |
| **offset** | **int**| How many managed users to skip | [optional] [default to 0] |

### Return type

[**\WidgeticApi\Model\PartnerAnalyticsByManagedUserResponse**](../Model/PartnerAnalyticsByManagedUserResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerAnalyticsSummary()`

```php
getPartnerAnalyticsSummary($partner_id, $start_date, $end_date, $managed_user_id, $managed_user_external_id): \WidgeticApi\Model\PartnerAnalyticsSummaryResponse
```

What was done with a partner's published widgets

Counts what the visitors of the compositions made through your account did in a period: how many times a composition was **viewed**, how many times a visitor **interacted** with one, and how many different visitors there were. It covers every composition of your account, your own and the ones made for your managed users; narrow it to one managed user with `managedUserId` or `managedUserExternalId` (not both).  The numbers come from the events the embedded widgets send while they are shown (the Widgetic embed SDK sends them by itself), counted when you ask. Only views and interactions are counted; the events that describe a visit (its start, its end, the device and the referrer) are not.  The period runs from `startDate` (included) to `endDate` (not included): the 30 days before now when you give neither, and at most 366 days. A date without a time is midnight UTC at the start of that day, so for all of October give `startDate=2026-10-01` and `endDate=2026-11-01`.  The caller must be the person who administers the partner (an API key of that account works, with the `partner:read` scope), or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose widgets to report on
$start_date = 'start_date_example'; // string | Start of the period, included. An ISO 8601 date (`2026-10-01`) or date-time with its offset (`2026-10-01T08:00:00Z`). Default 30 days before `endDate`.
$end_date = 'end_date_example'; // string | End of the period, not included, in the same forms. Default now. It must be after `startDate`, by at most 366 days.
$managed_user_id = 'managed_user_id_example'; // string | Report only on this managed user (Widgetic's id for the user). Send this or `managedUserExternalId`, not both.
$managed_user_external_id = 'managed_user_external_id_example'; // string | Report only on the managed user you registered with this `externalId` (your own identifier for the user). Send this or `managedUserId`, not both.

try {
    $result = $apiInstance->getPartnerAnalyticsSummary($partner_id, $start_date, $end_date, $managed_user_id, $managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerAnalyticsSummary: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose widgets to report on | |
| **start_date** | **string**| Start of the period, included. An ISO 8601 date (&#x60;2026-10-01&#x60;) or date-time with its offset (&#x60;2026-10-01T08:00:00Z&#x60;). Default 30 days before &#x60;endDate&#x60;. | [optional] |
| **end_date** | **string**| End of the period, not included, in the same forms. Default now. It must be after &#x60;startDate&#x60;, by at most 366 days. | [optional] |
| **managed_user_id** | **string**| Report only on this managed user (Widgetic&#39;s id for the user). Send this or &#x60;managedUserExternalId&#x60;, not both. | [optional] |
| **managed_user_external_id** | **string**| Report only on the managed user you registered with this &#x60;externalId&#x60; (your own identifier for the user). Send this or &#x60;managedUserId&#x60;, not both. | [optional] |

### Return type

[**\WidgeticApi\Model\PartnerAnalyticsSummaryResponse**](../Model/PartnerAnalyticsSummaryResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerAnalyticsTimeline()`

```php
getPartnerAnalyticsTimeline($partner_id, $start_date, $end_date, $managed_user_id, $managed_user_external_id): \WidgeticApi\Model\PartnerAnalyticsTimelineResponse
```

What was done with a partner's widgets, day by day

Counts views, interactions and visitors for each day of a period (UTC days), oldest first, for a chart. Every day of the period is in the list, also one on which nothing happened (all zeros), so the list can be drawn as it is. Narrow it to one managed user with `managedUserId` or `managedUserExternalId` (not both).  The period works as it does for `getPartnerAnalyticsSummary`; `startDate` and `endDate` are best given as dates, so that the first and the last day are whole days. The caller must be the person who administers the partner (an API key of that account works, with the `partner:read` scope), or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose widgets to report on
$start_date = 'start_date_example'; // string | Start of the period, included. An ISO 8601 date (`2026-10-01`) or date-time with its offset. Default 30 days before `endDate`.
$end_date = 'end_date_example'; // string | End of the period, not included, in the same forms. Default now. At most 366 days after `startDate`.
$managed_user_id = 'managed_user_id_example'; // string | Report only on this managed user (Widgetic's id for the user). Send this or `managedUserExternalId`, not both.
$managed_user_external_id = 'managed_user_external_id_example'; // string | Report only on the managed user you registered with this `externalId`. Send this or `managedUserId`, not both.

try {
    $result = $apiInstance->getPartnerAnalyticsTimeline($partner_id, $start_date, $end_date, $managed_user_id, $managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerAnalyticsTimeline: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose widgets to report on | |
| **start_date** | **string**| Start of the period, included. An ISO 8601 date (&#x60;2026-10-01&#x60;) or date-time with its offset. Default 30 days before &#x60;endDate&#x60;. | [optional] |
| **end_date** | **string**| End of the period, not included, in the same forms. Default now. At most 366 days after &#x60;startDate&#x60;. | [optional] |
| **managed_user_id** | **string**| Report only on this managed user (Widgetic&#39;s id for the user). Send this or &#x60;managedUserExternalId&#x60;, not both. | [optional] |
| **managed_user_external_id** | **string**| Report only on the managed user you registered with this &#x60;externalId&#x60;. Send this or &#x60;managedUserId&#x60;, not both. | [optional] |

### Return type

[**\WidgeticApi\Model\PartnerAnalyticsTimelineResponse**](../Model/PartnerAnalyticsTimelineResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerAnalyticsTopWidgets()`

```php
getPartnerAnalyticsTopWidgets($partner_id, $start_date, $end_date, $managed_user_id, $managed_user_external_id, $limit): \WidgeticApi\Model\PartnerAnalyticsTopWidgetsResponse
```

Which widgets were viewed the most

Lists the widgets whose compositions were viewed the most in a period, with their views, interactions, visitors and how many of their compositions were viewed. A widget that nobody viewed or used is not listed. The most viewed come first (then the most used), and at most `limit` are listed. Narrow it to one managed user with `managedUserId` or `managedUserExternalId` (not both).  The period works as it does for `getPartnerAnalyticsSummary`. The caller must be the person who administers the partner (an API key of that account works, with the `partner:read` scope), or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose widgets to report on
$start_date = 'start_date_example'; // string | Start of the period, included. An ISO 8601 date (`2026-10-01`) or date-time with its offset. Default 30 days before `endDate`.
$end_date = 'end_date_example'; // string | End of the period, not included, in the same forms. Default now. At most 366 days after `startDate`.
$managed_user_id = 'managed_user_id_example'; // string | Report only on this managed user (Widgetic's id for the user). Send this or `managedUserExternalId`, not both.
$managed_user_external_id = 'managed_user_external_id_example'; // string | Report only on the managed user you registered with this `externalId`. Send this or `managedUserId`, not both.
$limit = 10; // int | How many widgets to list at most

try {
    $result = $apiInstance->getPartnerAnalyticsTopWidgets($partner_id, $start_date, $end_date, $managed_user_id, $managed_user_external_id, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerAnalyticsTopWidgets: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose widgets to report on | |
| **start_date** | **string**| Start of the period, included. An ISO 8601 date (&#x60;2026-10-01&#x60;) or date-time with its offset. Default 30 days before &#x60;endDate&#x60;. | [optional] |
| **end_date** | **string**| End of the period, not included, in the same forms. Default now. At most 366 days after &#x60;startDate&#x60;. | [optional] |
| **managed_user_id** | **string**| Report only on this managed user (Widgetic&#39;s id for the user). Send this or &#x60;managedUserExternalId&#x60;, not both. | [optional] |
| **managed_user_external_id** | **string**| Report only on the managed user you registered with this &#x60;externalId&#x60;. Send this or &#x60;managedUserId&#x60;, not both. | [optional] |
| **limit** | **int**| How many widgets to list at most | [optional] [default to 10] |

### Return type

[**\WidgeticApi\Model\PartnerAnalyticsTopWidgetsResponse**](../Model/PartnerAnalyticsTopWidgetsResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerBillingOverview()`

```php
getPartnerBillingOverview($partner_id): \WidgeticApi\Model\GetPartnerBillingOverview200Response
```

Get comprehensive partner billing overview

Retrieves the partner's credits (`operationalCredits`), the partner's contract terms (`partnerCustomization`, the same fields as `getPartnerContract`) and billing integration status. Internal negotiation notes are not part of it. `operationalCredits` is the one account a partner has for its credits: the account of the person who administers it. It holds `balance` (the same balance `getPartnerCreditBalance` reads), `reservedBalance`, `availableBalance` (what a new operation can use) and `recentTransactions` (the ten newest entries of the ledger `getPartnerCreditTransactions` lists). A partner with no administrator has no account, and reads 0 and an empty list.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | Partner ID

try {
    $result = $apiInstance->getPartnerBillingOverview($partner_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerBillingOverview: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| Partner ID | |

### Return type

[**\WidgeticApi\Model\GetPartnerBillingOverview200Response**](../Model/GetPartnerBillingOverview200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerContract()`

```php
getPartnerContract($partner_id): \WidgeticApi\Model\PartnerContractResponse
```

Get a partner's contract

Returns the commercial terms agreed with the partner: price, included credits and storage, billing cycle, commitment, support level, and the dates the contract runs between.  A partner reads its own: the caller must be the person who administers the partner (an API key of that account works), and anyone else is refused with 403 whether or not the partner exists. Widgetic administrators can read any partner's. Responds 404 while no contract has been recorded for the partner, which is the case until Widgetic sets its terms.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose contract to read

try {
    $result = $apiInstance->getPartnerContract($partner_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerContract: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose contract to read | |

### Return type

[**\WidgeticApi\Model\PartnerContractResponse**](../Model/PartnerContractResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerCreditBalance()`

```php
getPartnerCreditBalance($partner_id): \WidgeticApi\Model\AccountCreditBalanceResponse
```

Get partner credit balance

Returns the credits the partner has, and how much of that is reserved by operations that are still running. A partner has ONE account for its credits: the account of the person who administers it, the same account its API key acts as. There is nothing else to create or to fund. What its customers' editor sessions and its own API calls spend comes out of that account, and the credits a paid invoice carries are added to it, so this is the same balance `getUserCreditBalance` reads for that person.  A partner with no administrator has no account to hold credits, and reads a balance of 0.  Access: the person who administers the partner, or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | Partner ID

try {
    $result = $apiInstance->getPartnerCreditBalance($partner_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerCreditBalance: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| Partner ID | |

### Return type

[**\WidgeticApi\Model\AccountCreditBalanceResponse**](../Model/AccountCreditBalanceResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerCreditTransactions()`

```php
getPartnerCreditTransactions($partner_id, $limit, $offset, $type): \WidgeticApi\Model\GetPartnerCreditTransactions200Response
```

Get partner credit transaction history

Lists what happened to the partner's credits, newest first: the entries of the credit ledger of the account of the person who administers it, the one account a partner has for its credits. Every operation that spends credits is a `debit` entry, and the credits an invoice carried arrive as `credit` entries when the invoice is paid, so this is also how the partner's usage is read. It is the same ledger `getUserCreditTransactions` reads for that person.  A partner with no administrator has no account, and an empty ledger.  The page is always bounded: `limit` defaults to 20 and is capped at 100, `offset` defaults to 0.  Access: the person who administers the partner, or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | Partner ID
$limit = 20; // int | Number of transactions to return
$offset = 0; // int | Number of transactions to skip
$type = 'type_example'; // string | Only entries of this type, for instance `debit` for the credits spent. The types are listed on `AccountCreditTransaction`.

try {
    $result = $apiInstance->getPartnerCreditTransactions($partner_id, $limit, $offset, $type);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerCreditTransactions: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| Partner ID | |
| **limit** | **int**| Number of transactions to return | [optional] [default to 20] |
| **offset** | **int**| Number of transactions to skip | [optional] [default to 0] |
| **type** | **string**| Only entries of this type, for instance &#x60;debit&#x60; for the credits spent. The types are listed on &#x60;AccountCreditTransaction&#x60;. | [optional] |

### Return type

[**\WidgeticApi\Model\GetPartnerCreditTransactions200Response**](../Model/GetPartnerCreditTransactions200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerDataDatabase()`

```php
getPartnerDataDatabase($partner_id): \WidgeticApi\Model\PartnerDataDatabaseResponse
```

See the Neon database a partner keeps the data of its compositions in

Returns the database set with `setPartnerDataDatabase`, without its password: the host, the database and the role, when it last passed the check, and why the latest re-check failed if it did. Responds 404 while the partner has no database of its own, which means the data of its compositions is kept by Widgetic.  The caller must be the person who administers the partner (an API key of that account works, with the `partner:read` scope), or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose database to read

try {
    $result = $apiInstance->getPartnerDataDatabase($partner_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerDataDatabase: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose database to read | |

### Return type

[**\WidgeticApi\Model\PartnerDataDatabaseResponse**](../Model/PartnerDataDatabaseResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerDesignDefaults()`

```php
getPartnerDesignDefaults($partner_id): \WidgeticApi\Model\GetPartnerDesignDefaults200Response
```

Read partner-wide design defaults

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string

try {
    $result = $apiInstance->getPartnerDesignDefaults($partner_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerDesignDefaults: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**|  | |

### Return type

[**\WidgeticApi\Model\GetPartnerDesignDefaults200Response**](../Model/GetPartnerDesignDefaults200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerEntitlements()`

```php
getPartnerEntitlements($partner_id, $include_expired, $feature, $source): \WidgeticApi\Model\GetPartnerEntitlementsResponse
```

Get partner entitlements

Retrieves all entitlements for a partner (admin or partner access).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | Partner ID
$include_expired = True; // bool | Include expired entitlements in results
$feature = 'feature_example'; // string | Filter by specific feature
$source = 'source_example'; // string | Filter by entitlement source

try {
    $result = $apiInstance->getPartnerEntitlements($partner_id, $include_expired, $feature, $source);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerEntitlements: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| Partner ID | |
| **include_expired** | **bool**| Include expired entitlements in results | [optional] |
| **feature** | **string**| Filter by specific feature | [optional] |
| **source** | **string**| Filter by entitlement source | [optional] |

### Return type

[**\WidgeticApi\Model\GetPartnerEntitlementsResponse**](../Model/GetPartnerEntitlementsResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerEntryContextSigning()`

```php
getPartnerEntryContextSigning($partner_id): \WidgeticApi\Model\PartnerEntryContextSigningResponse
```

See how the context of your embeds is signed

Says whether you have a secret to sign the `context` of your embeds with, when it was made, whether the secret it replaced is still accepted, and whether an entry without a valid signature is refused (`required`). The secret itself is never part of the answer: it is shown once, when it is made (`rotatePartnerEntryContextSecret`, which also explains what signing is for and how to sign).  Signing covers the entries written through the gateway into the compositions of your managed users and into those of your own account. The caller must be the person who administers the partner (an API key of that account works, with the `partner:read` scope), or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose context signing to read

try {
    $result = $apiInstance->getPartnerEntryContextSigning($partner_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerEntryContextSigning: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose context signing to read | |

### Return type

[**\WidgeticApi\Model\PartnerEntryContextSigningResponse**](../Model/PartnerEntryContextSigningResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerNotificationSettings()`

```php
getPartnerNotificationSettings($partner_id): \WidgeticApi\Model\PartnerNotificationSettingsResponse
```

Where your notifications go

Returns who gets the emails, which events you want by email and by webhook, the address of your webhook, and whether it has a secret to sign with. The secret itself is never returned: it is shown once, when it is made. `events` lists every kind of event there is, for a settings screen.  The caller must be the person who administers the partner (an API key of that account works, with the `partner:read` scope), or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose notification settings to read

try {
    $result = $apiInstance->getPartnerNotificationSettings($partner_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerNotificationSettings: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose notification settings to read | |

### Return type

[**\WidgeticApi\Model\PartnerNotificationSettingsResponse**](../Model/PartnerNotificationSettingsResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerStorageDestination()`

```php
getPartnerStorageDestination($partner_id): \WidgeticApi\Model\PartnerStorageDestinationResponse
```

Get where a partner's uploaded files are stored

Returns the partner's storage destination without its secret: the endpoint, bucket, folder and public address, the last four characters of the access key id, when the destination last passed the check, and why the latest re-check failed if it did. Responds 404 while the partner has no destination, which means the partner cannot be activated, its uploads are refused, and no editor session is made for its customers until a destination is set.  The caller must be the person who administers the partner, or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose storage destination to read

try {
    $result = $apiInstance->getPartnerStorageDestination($partner_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerStorageDestination: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose storage destination to read | |

### Return type

[**\WidgeticApi\Model\PartnerStorageDestinationResponse**](../Model/PartnerStorageDestinationResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPartnerStorageUsage()`

```php
getPartnerStorageUsage($partner_id, $limit, $offset): \WidgeticApi\Model\PartnerStorageUsageResponse
```

What a partner's customers store

Says how many files, and how many bytes, your account keeps, in total and for each of your managed users, and how much of it is in Widgetic's storage and how much in your own storage destination (`setPartnerStorageDestination`). Use it to see which customers store the most, or to charge them for it.  A file is counted for a managed user when it was filed under that user: by naming `managed_user_id` or `managed_user_external_id` when you upload it (`uploadsPost`, or the metadata of a resumable upload), or because it was uploaded through that user's editor session, which files everything under its user. The files that are not filed under anyone (your own, and the ones uploaded without naming a managed user) are the row whose `managedUserId` is null. Deleted files are not counted. To list the files of one managed user, use the `managed_user_id` filter of `uploadsGet`.  The answer is counted when you ask, so it is always current. The groups are ordered by size, the heaviest first, and `page.hasMore` says whether more follow.  The caller must be the person who administers the partner (an API key of that account works, with the `partner:read` scope), or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose storage to report on
$limit = 50; // int | How many managed users to list at most
$offset = 0; // int | How many managed users to skip

try {
    $result = $apiInstance->getPartnerStorageUsage($partner_id, $limit, $offset);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPartnerStorageUsage: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose storage to report on | |
| **limit** | **int**| How many managed users to list at most | [optional] [default to 50] |
| **offset** | **int**| How many managed users to skip | [optional] [default to 0] |

### Return type

[**\WidgeticApi\Model\PartnerStorageUsageResponse**](../Model/PartnerStorageUsageResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPersonalWorkspaceDomains()`

```php
getPersonalWorkspaceDomains($id): \WidgeticApi\Model\GetPersonalWorkspaceDomains200Response
```

List the websites allowed to show your widgets

Lists the websites on an account's own list, newest first. It is the list Widgetic checks when a widget of the account is embedded: when it holds at least one website, the widget is shown on those websites (and on Widgetic's own) and nowhere else; when it is empty, the widget can be shown anywhere. If the account administers a partner, the websites set on the partner record by Widgetic are added to them. Widgets that belong to an organization use the organization's list instead. The answer holds the whole list, however long it is: a partner's list has no limit.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The account the list belongs to. For your own, your own user id

try {
    $result = $apiInstance->getPersonalWorkspaceDomains($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPersonalWorkspaceDomains: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The account the list belongs to. For your own, your own user id | |

### Return type

[**\WidgeticApi\Model\GetPersonalWorkspaceDomains200Response**](../Model/GetPersonalWorkspaceDomains200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPublicCompositionEmbed()`

```php
getPublicCompositionEmbed($composition_id): \WidgeticApi\Model\GetPublicCompositionEmbed200Response
```
### URI(s):
- https://api.widgetic.com The public embed routes are served at the root of the API host, not under /v1.
Resolve a composition UUID to a published widget URL

Public customer embed lookup. No API key. Used by embed-sdk.js on third-party sites. If the composition's owner listed the websites it may appear on (the workspace's domain list, or the `allowedDomains` of a partner the owner administers), a request from any other website is refused with 403 `DOMAIN_NOT_ALLOWED`. The website is read from the `Origin` header, or the host of `Referer` when there is no `Origin`; a request that names neither (a server, a tool) is not refused. An owner who listed nothing is not restricted, and a page on the visitor's own machine (`localhost`, `127.0.0.1` or `[::1]`, on any port) is always allowed. So is the website where a partner integrates Widgetic, with every subdomain of it (`platformDomain` in the answer of `GET /partners/mine`), for the widgets of that partner: a partner's list never has to name it. The list stops other websites from showing the embed in a visitor's browser; it does not hide the published content from someone who holds the composition ID. **Address.** `https://api.widgetic.com/embed/compositions/{compositionId}`: the root of the API host, NOT under `/v1`. A client generated from this description for `https://api.widgetic.com/v1` must be given the base address `https://api.widgetic.com` for the calls of the `Public Embed` tag. **Limit.** 500 calls for each visitor address and browser in one counting window, shared with the frame and the status routes. Over it the answer is 429 `RATE_LIMITED` with a `Retry-After` header.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$composition_id = 'composition_id_example'; // string

$hostIndex = 0;
$variables = [
];

try {
    $result = $apiInstance->getPublicCompositionEmbed($composition_id, $hostIndex, $variables);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPublicCompositionEmbed: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **composition_id** | **string**|  | |
| hostIndex | null|int | Host index. Defaults to null. If null, then the library will use $this->hostIndex instead | [optional] |
| variables | array | Associative array of variables to pass to the host. Defaults to empty array. | [optional] |

### Return type

[**\WidgeticApi\Model\GetPublicCompositionEmbed200Response**](../Model/GetPublicCompositionEmbed200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getPublicCompositionIframe()`

```php
getPublicCompositionIframe($composition_id): string
```
### URI(s):
- https://api.widgetic.com The public embed routes are served at the root of the API host, not under /v1.
Embed a published composition with its saved values

Public HTML wrapper with an inner published artifact iframe. No API key or SDK required. If the composition's owner listed the websites it may appear on, the page is sent with `Content-Security-Policy: frame-ancestors` naming those websites (and Widgetic's own, and the website where the partner the owner administers integrates Widgetic, with its subdomains), so a browser refuses to show it inside any other website whatever `Referer` policy that website uses. Opening the address directly still works. An owner who listed nothing is not restricted. **Address.** `https://api.widgetic.com/embed/compositions/{compositionId}/frame`: the root of the API host, NOT under `/v1`. A client generated from this description for `https://api.widgetic.com/v1` must be given the base address `https://api.widgetic.com` for the calls of the `Public Embed` tag.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$composition_id = 'composition_id_example'; // string

$hostIndex = 0;
$variables = [
];

try {
    $result = $apiInstance->getPublicCompositionIframe($composition_id, $hostIndex, $variables);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getPublicCompositionIframe: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **composition_id** | **string**|  | |
| hostIndex | null|int | Host index. Defaults to null. If null, then the library will use $this->hostIndex instead | [optional] |
| variables | array | Associative array of variables to pass to the host. Defaults to empty array. | [optional] |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `text/html`, `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getUserAdapterConnections()`

```php
getUserAdapterConnections($user_id): \WidgeticApi\Model\GetUserAdapterConnections200Response
```

See which adapter keys an account has connected

Widget adapters are capabilities a widget can use, and some of them act through a service the owner has an account with: an adapter that sends email needs the owner's email provider key, one that sends texts needs the owner's SMS provider key. This lists every key an adapter takes from an owner and whether this account has connected it, so a settings page can show what is missing.  An empty list means no adapter takes a key from an owner at the moment. The list never contains a key: only whether one is connected and when it was last set.  Connect a key with `setUserAdapterConnection`; take it away with `removeUserAdapterConnection`. The widgets of customers a partner manages use the partner's keys instead (`getPartnerAdapterConnections`).  The caller must be the account itself (an API key of that account works, with the `account:read` scope), or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$user_id = 'user_id_example'; // string | The account whose adapter keys to list. For your own, your own user id

try {
    $result = $apiInstance->getUserAdapterConnections($user_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getUserAdapterConnections: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user_id** | **string**| The account whose adapter keys to list. For your own, your own user id | |

### Return type

[**\WidgeticApi\Model\GetUserAdapterConnections200Response**](../Model/GetUserAdapterConnections200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getUserApiKeyUsageLogs()`

```php
getUserApiKeyUsageLogs($id, $key_id, $limit): \WidgeticApi\Model\GetUserApiKeyUsageLogsResponse
```

Read what an API key was used for

Lists the calls made with one key, newest first: when, which path and method, and the status each ended with. Use it to see whether a key is still in use before deleting it, or to see what a key that should not be in use has been doing.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The account the key belongs to
$key_id = 'key_id_example'; // string | The `keyId` of the key, as the list shows it
$limit = 500; // int | How many calls to return, newest first

try {
    $result = $apiInstance->getUserApiKeyUsageLogs($id, $key_id, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getUserApiKeyUsageLogs: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The account the key belongs to | |
| **key_id** | **string**| The &#x60;keyId&#x60; of the key, as the list shows it | |
| **limit** | **int**| How many calls to return, newest first | [optional] [default to 500] |

### Return type

[**\WidgeticApi\Model\GetUserApiKeyUsageLogsResponse**](../Model/GetUserApiKeyUsageLogsResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getUserApiKeys()`

```php
getUserApiKeys($id): \WidgeticApi\Model\GetUserApiKeys200Response
```

List the API keys of an account

Lists the API keys of an account, in the order they were made: name, the first characters of the key, when it was made, when it expires, when it was last used, whether it is switched on and what it is limited to (`scopes` and `preset`). The secret of a key is never part of the list. A caller can list its own account's keys; Widgetic staff can list any account's.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The account the keys belong to. For your own keys, your own user id

try {
    $result = $apiInstance->getUserApiKeys($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getUserApiKeys: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The account the keys belong to. For your own keys, your own user id | |

### Return type

[**\WidgeticApi\Model\GetUserApiKeys200Response**](../Model/GetUserApiKeys200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getUserCreditBalance()`

```php
getUserCreditBalance($user_id): \WidgeticApi\Model\AccountCreditBalanceResponse
```

Get an account's credit balance

Returns the credits an account holds: the balance, and how much of it is reserved by operations that are still running.  An account reads its own balance; with a partner's API key, that is the account of the person who administers the partner. Widgetic administrators can read any account's. An account that has never held credits reads a balance of 0. `getPartnerCreditBalance` reads this same balance by partner id.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$user_id = 'user_id_example'; // string | The account whose balance to read

try {
    $result = $apiInstance->getUserCreditBalance($user_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getUserCreditBalance: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user_id** | **string**| The account whose balance to read | |

### Return type

[**\WidgeticApi\Model\AccountCreditBalanceResponse**](../Model/AccountCreditBalanceResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getUserCreditTransactions()`

```php
getUserCreditTransactions($user_id, $transaction_type, $limit, $offset): \WidgeticApi\Model\GetPartnerCreditTransactions200Response
```

List an account's credit ledger

Lists the entries of an account's credit ledger, newest first. This is also how an account's usage is read: every operation that spends credits is a `debit` entry, so summing the `debit` entries over a period gives the credits consumed in it, and the other types give what was added.  An account reads its own ledger; with a partner's API key, that is the account of the person who administers the partner. Widgetic administrators can read any account's. `getPartnerCreditTransactions` reads this same ledger by partner id.  The page is always bounded: `limit` defaults to 100 and is capped at 500, `offset` defaults to 0.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$user_id = 'user_id_example'; // string | The account whose ledger to read
$transaction_type = 'transaction_type_example'; // string | Only entries of this type, for instance `debit` for the credits spent. The types are listed on `AccountCreditTransaction`.
$limit = 100; // int | Maximum number of entries to return
$offset = 0; // int | Number of entries to skip

try {
    $result = $apiInstance->getUserCreditTransactions($user_id, $transaction_type, $limit, $offset);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getUserCreditTransactions: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user_id** | **string**| The account whose ledger to read | |
| **transaction_type** | **string**| Only entries of this type, for instance &#x60;debit&#x60; for the credits spent. The types are listed on &#x60;AccountCreditTransaction&#x60;. | [optional] |
| **limit** | **int**| Maximum number of entries to return | [optional] [default to 100] |
| **offset** | **int**| Number of entries to skip | [optional] [default to 0] |

### Return type

[**\WidgeticApi\Model\GetPartnerCreditTransactions200Response**](../Model/GetPartnerCreditTransactions200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getWidgets()`

```php
getWidgets($page, $size, $canvas_id, $managed_user_id, $managed_user_external_id): \WidgeticApi\Model\GetWidgets200Response
```

List Widgets

Lists the widgets your account owns, newest first. A widget is the reusable piece a composition is made from; this is your own library, not a catalogue of Widgetic's widgets.  Pass `page` (counting from 1) and `size` (1 to 100, 20 when left out) to read the list one page at a time. `meta` then carries `total`, `hasNextPage` and `hasPreviousPage`, so a client can walk the list to its end. A page past the end is an empty list. Without `page` and `size` the call returns the whole list in one response, which only suits an account with a few widgets.  Pass `canvasId` to list only the widgets on one of your canvases. That list is always returned whole, whatever `page` and `size` say.  Pass `managedUserId` (Widgetic's id for one of your managed users) or `managedUserExternalId` (your own identifier for the user) to list only the widgets made for that managed user. The widgets of your other managed users, and your own, are left out. It combines with `page`, `size` and `canvasId`. A managed user that is not yours, or does not exist, is answered with 404 and `MANAGED_USER_NOT_FOUND`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$page = 56; // int | Page to return, counting from 1. Giving `page` or `size` turns paging on.
$size = 56; // int | How many widgets a page holds (20 when `page` is given without it). Giving `page` or `size` turns paging on.
$canvas_id = 'canvas_id_example'; // string | List only the widgets on this canvas. The list is returned whole.
$managed_user_id = 'managed_user_id_example'; // string | List only the widgets made for this managed user (Widgetic's id for the user). Send this or `managedUserExternalId`, not both.
$managed_user_external_id = 'managed_user_external_id_example'; // string | List only the widgets made for the managed user you registered with this `externalId` (your own identifier for the user). Send this or `managedUserId`, not both.

try {
    $result = $apiInstance->getWidgets($page, $size, $canvas_id, $managed_user_id, $managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getWidgets: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **int**| Page to return, counting from 1. Giving &#x60;page&#x60; or &#x60;size&#x60; turns paging on. | [optional] |
| **size** | **int**| How many widgets a page holds (20 when &#x60;page&#x60; is given without it). Giving &#x60;page&#x60; or &#x60;size&#x60; turns paging on. | [optional] |
| **canvas_id** | **string**| List only the widgets on this canvas. The list is returned whole. | [optional] |
| **managed_user_id** | **string**| List only the widgets made for this managed user (Widgetic&#39;s id for the user). Send this or &#x60;managedUserExternalId&#x60;, not both. | [optional] |
| **managed_user_external_id** | **string**| List only the widgets made for the managed user you registered with this &#x60;externalId&#x60; (your own identifier for the user). Send this or &#x60;managedUserId&#x60;, not both. | [optional] |

### Return type

[**\WidgeticApi\Model\GetWidgets200Response**](../Model/GetWidgets200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `getWidgetsBatch()`

```php
getWidgetsBatch($get_widgets_batch_request): \WidgeticApi\Model\GetWidgetsBatchResponse
```

Get Widgets Batch

Retrieves multiple widgets by their IDs in a single request. An id that is not found, or that is not yours, is reported in `errors` exactly like one that does not exist. Called with an editor session, only the widgets made for the session's managed user are returned.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$get_widgets_batch_request = new \WidgeticApi\Model\GetWidgetsBatchRequest(); // \WidgeticApi\Model\GetWidgetsBatchRequest

try {
    $result = $apiInstance->getWidgetsBatch($get_widgets_batch_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->getWidgetsBatch: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **get_widgets_batch_request** | [**\WidgeticApi\Model\GetWidgetsBatchRequest**](../Model/GetWidgetsBatchRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\GetWidgetsBatchResponse**](../Model/GetWidgetsBatchResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listCompositionEntryItems()`

```php
listCompositionEntryItems($id, $table, $limit, $order, $since, $until, $cursor, $context, $filter, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CompositionEntryItemsPageSuccess
```

List composition entry items with paging and filters

Reads one widget table with cursor paging (time then id in byte order), optional since/until on the time column, and up to five context filters plus ten column filters. Rate limit 120 requests per minute. Each read batch uses a 5 s statement timeout.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$table = 'table_example'; // string
$limit = 25; // int
$order = 'desc'; // string | `desc` (the default) lists the newest entry first, `asc` the oldest. Entries are sorted by their time, then by their id (compared as text, byte by byte) in the same direction, so the order of two entries made at the same instant is always the same; an entry with no time counts as the oldest. A table with no time column is sorted by its id. The managed-user feed sorts by time, then by composition id, table and id.
$since = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Only entries made at this time or later: `since` is INCLUSIVE (an entry made at exactly `since` is returned). A date and time with an offset, such as `2026-10-01T00:00:00Z`; anything else answers 400 `INVALID_SINCE`. An entry with no time never matches, and a table with no time column answers 400 `ENTRY_TABLE_HAS_NO_TIME`.
$until = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Only entries made before this time: `until` is EXCLUSIVE (an entry made at exactly `until` is NOT returned), so `since=A&until=B` followed by `since=B&until=C` counts every entry once. Same form and same refusals as `since` (400 `INVALID_UNTIL`).
$cursor = 'cursor_example'; // string
$context = array('key' => 'context_example'); // array<string,string> | Host context filters as `context[key]=value` (max 5 keys, counting dotted `context.key` too). Use `column.<name>=value` for columns whose names collide with reserved parameters.
$filter = array('key' => 'filter_example'); // array<string,string> | Column filters as `filter[columnName]=value` (same meaning as bare `columnName=value` or `column.columnName=value`; max 10 column filters counting all spellings). A plain `filter=value` still filters a column named `filter`.
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->listCompositionEntryItems($id, $table, $limit, $order, $since, $until, $cursor, $context, $filter, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->listCompositionEntryItems: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **table** | **string**|  | |
| **limit** | **int**|  | [optional] [default to 25] |
| **order** | **string**| &#x60;desc&#x60; (the default) lists the newest entry first, &#x60;asc&#x60; the oldest. Entries are sorted by their time, then by their id (compared as text, byte by byte) in the same direction, so the order of two entries made at the same instant is always the same; an entry with no time counts as the oldest. A table with no time column is sorted by its id. The managed-user feed sorts by time, then by composition id, table and id. | [optional] [default to &#39;desc&#39;] |
| **since** | **\DateTime**| Only entries made at this time or later: &#x60;since&#x60; is INCLUSIVE (an entry made at exactly &#x60;since&#x60; is returned). A date and time with an offset, such as &#x60;2026-10-01T00:00:00Z&#x60;; anything else answers 400 &#x60;INVALID_SINCE&#x60;. An entry with no time never matches, and a table with no time column answers 400 &#x60;ENTRY_TABLE_HAS_NO_TIME&#x60;. | [optional] |
| **until** | **\DateTime**| Only entries made before this time: &#x60;until&#x60; is EXCLUSIVE (an entry made at exactly &#x60;until&#x60; is NOT returned), so &#x60;since&#x3D;A&amp;until&#x3D;B&#x60; followed by &#x60;since&#x3D;B&amp;until&#x3D;C&#x60; counts every entry once. Same form and same refusals as &#x60;since&#x60; (400 &#x60;INVALID_UNTIL&#x60;). | [optional] |
| **cursor** | **string**|  | [optional] |
| **context** | [**array<string,string>**](../Model/string.md)| Host context filters as &#x60;context[key]&#x3D;value&#x60; (max 5 keys, counting dotted &#x60;context.key&#x60; too). Use &#x60;column.&lt;name&gt;&#x3D;value&#x60; for columns whose names collide with reserved parameters. | [optional] |
| **filter** | [**array<string,string>**](../Model/string.md)| Column filters as &#x60;filter[columnName]&#x3D;value&#x60; (same meaning as bare &#x60;columnName&#x3D;value&#x60; or &#x60;column.columnName&#x3D;value&#x60;; max 10 column filters counting all spellings). A plain &#x60;filter&#x3D;value&#x60; still filters a column named &#x60;filter&#x60;. | [optional] |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\CompositionEntryItemsPageSuccess**](../Model/CompositionEntryItemsPageSuccess.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listManagedUserEntries()`

```php
listManagedUserEntries($id, $composition_id, $table, $limit, $order, $since, $until, $cursor, $context, $filter): \WidgeticApi\Model\ManagedUserEntriesPageSuccess
```

List entries across a managed user's compositions

Merges eligible tables (time and id columns) across the managed user's compositions in global time order, then compositionId, table, and id (byte order). Only tables with both a time and an id column take part. Rate limit 30 requests per minute.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$composition_id = 'composition_id_example'; // string
$table = 'table_example'; // string
$limit = 25; // int
$order = 'desc'; // string | `desc` (the default) lists the newest entry first, `asc` the oldest. Entries are sorted by their time, then by their id (compared as text, byte by byte) in the same direction, so the order of two entries made at the same instant is always the same; an entry with no time counts as the oldest. A table with no time column is sorted by its id. The managed-user feed sorts by time, then by composition id, table and id.
$since = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Only entries made at this time or later: `since` is INCLUSIVE (an entry made at exactly `since` is returned). A date and time with an offset, such as `2026-10-01T00:00:00Z`; anything else answers 400 `INVALID_SINCE`. An entry with no time never matches, and a table with no time column answers 400 `ENTRY_TABLE_HAS_NO_TIME`.
$until = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Only entries made before this time: `until` is EXCLUSIVE (an entry made at exactly `until` is NOT returned), so `since=A&until=B` followed by `since=B&until=C` counts every entry once. Same form and same refusals as `since` (400 `INVALID_UNTIL`).
$cursor = 'cursor_example'; // string
$context = array('key' => 'context_example'); // array<string,string> | Host context filters as `context[key]=value` (max 5 keys, counting dotted `context.key` too). Use `column.<name>=value` for columns whose names collide with reserved parameters.
$filter = array('key' => 'filter_example'); // array<string,string> | Column filters as `filter[columnName]=value` (same meaning as bare `columnName=value` or `column.columnName=value`; max 10 column filters counting all spellings). A plain `filter=value` still filters a column named `filter`.

try {
    $result = $apiInstance->listManagedUserEntries($id, $composition_id, $table, $limit, $order, $since, $until, $cursor, $context, $filter);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->listManagedUserEntries: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **composition_id** | **string**|  | [optional] |
| **table** | **string**|  | [optional] |
| **limit** | **int**|  | [optional] [default to 25] |
| **order** | **string**| &#x60;desc&#x60; (the default) lists the newest entry first, &#x60;asc&#x60; the oldest. Entries are sorted by their time, then by their id (compared as text, byte by byte) in the same direction, so the order of two entries made at the same instant is always the same; an entry with no time counts as the oldest. A table with no time column is sorted by its id. The managed-user feed sorts by time, then by composition id, table and id. | [optional] [default to &#39;desc&#39;] |
| **since** | **\DateTime**| Only entries made at this time or later: &#x60;since&#x60; is INCLUSIVE (an entry made at exactly &#x60;since&#x60; is returned). A date and time with an offset, such as &#x60;2026-10-01T00:00:00Z&#x60;; anything else answers 400 &#x60;INVALID_SINCE&#x60;. An entry with no time never matches, and a table with no time column answers 400 &#x60;ENTRY_TABLE_HAS_NO_TIME&#x60;. | [optional] |
| **until** | **\DateTime**| Only entries made before this time: &#x60;until&#x60; is EXCLUSIVE (an entry made at exactly &#x60;until&#x60; is NOT returned), so &#x60;since&#x3D;A&amp;until&#x3D;B&#x60; followed by &#x60;since&#x3D;B&amp;until&#x3D;C&#x60; counts every entry once. Same form and same refusals as &#x60;since&#x60; (400 &#x60;INVALID_UNTIL&#x60;). | [optional] |
| **cursor** | **string**|  | [optional] |
| **context** | [**array<string,string>**](../Model/string.md)| Host context filters as &#x60;context[key]&#x3D;value&#x60; (max 5 keys, counting dotted &#x60;context.key&#x60; too). Use &#x60;column.&lt;name&gt;&#x3D;value&#x60; for columns whose names collide with reserved parameters. | [optional] |
| **filter** | [**array<string,string>**](../Model/string.md)| Column filters as &#x60;filter[columnName]&#x3D;value&#x60; (same meaning as bare &#x60;columnName&#x3D;value&#x60; or &#x60;column.columnName&#x3D;value&#x60;; max 10 column filters counting all spellings). A plain &#x60;filter&#x3D;value&#x60; still filters a column named &#x60;filter&#x60;. | [optional] |

### Return type

[**\WidgeticApi\Model\ManagedUserEntriesPageSuccess**](../Model/ManagedUserEntriesPageSuccess.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listPartnerNotificationDeliveries()`

```php
listPartnerNotificationDeliveries($partner_id, $limit): \WidgeticApi\Model\PartnerNotificationDeliveryLogResponse
```

How your notifications reached you

Lists the sends of your notifications, the newest first: each email to one address and each call to your webhook, with whether it was delivered, when it is tried again if not, how many attempts it had, and why the last one failed. Use it to find out why a webhook of yours did not receive an event.  An email counts as delivered when it was handed to the mail service; a call to your webhook counts as delivered when your endpoint answered with a 2xx status. Anything else is tried again, after 1 minute, then 5 minutes, 30 minutes, 2 hours, 6 hours, 12 hours and a day, eight attempts in all, because your address is read again at each attempt and you may have mended it. Two answers end the delivery at once: `410 Gone` and `413 Payload Too Large`.  The caller must be the person who administers the partner (an API key of that account works, with the `partner:read` scope), or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose deliveries to list
$limit = 100; // int | How many deliveries to list at most

try {
    $result = $apiInstance->listPartnerNotificationDeliveries($partner_id, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->listPartnerNotificationDeliveries: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose deliveries to list | |
| **limit** | **int**| How many deliveries to list at most | [optional] [default to 100] |

### Return type

[**\WidgeticApi\Model\PartnerNotificationDeliveryLogResponse**](../Model/PartnerNotificationDeliveryLogResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listPartnerNotifications()`

```php
listPartnerNotifications($partner_id, $limit, $before): \WidgeticApi\Model\PartnerNotificationPageResponse
```

What your partner account was told

Lists the notifications of a partner, the newest first: the invoices Widgetic issued and their payments, the reminders to pay them, a warning when your credits run low, and the changes to the standing of the account (activated, paused, resumed). It is the same list your dashboard shows, and each entry is what your webhook receives as `data` when you have one (`updatePartnerNotificationSettings`).  A page holds `limit` notifications (20 by default, at most 100). When there are older ones `nextBefore` is set: ask again with it as `before` to get the next page.  The caller must be the person who administers the partner (an API key of that account works, with the `partner:read` scope), or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose notifications to list
$limit = 20; // int | How many notifications to list at most
$before = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Only the notifications made before this moment. Give the `nextBefore` of the previous page.

try {
    $result = $apiInstance->listPartnerNotifications($partner_id, $limit, $before);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->listPartnerNotifications: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose notifications to list | |
| **limit** | **int**| How many notifications to list at most | [optional] [default to 20] |
| **before** | **\DateTime**| Only the notifications made before this moment. Give the &#x60;nextBefore&#x60; of the previous page. | [optional] |

### Return type

[**\WidgeticApi\Model\PartnerNotificationPageResponse**](../Model/PartnerNotificationPageResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `listPartnerPresets()`

```php
listPartnerPresets($partner_id): \WidgeticApi\Model\ListPartnerPresets200Response
```

List the widgets a partner offers as presets

Returns the partner's presets, ordered by `position` and then by `key`: the widgets it offers its managed users as starting points. The list is the same for every managed user.  Use a preset in one of two ways: - **Make a composition of it** (the content and design editor): call `createComposition` with the preset's   `widgetId` and the managed user. The widget itself stays yours; a composition is the user's own content. - **Give the user a copy to build on** (the widget creator): call `copyPresetForManagedUser`. The user gets   a widget and a canvas of their own.  Presets are not the same as the widgets Widgetic puts on every new Widgetic account. Those are chosen by Widgetic and are copied at sign-up. A preset here is yours, and is copied only when you ask.  The caller must be the person who administers the partner (an API key of that account works), or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose presets to list

try {
    $result = $apiInstance->listPartnerPresets($partner_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->listPartnerPresets: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose presets to list | |

### Return type

[**\WidgeticApi\Model\ListPartnerPresets200Response**](../Model/ListPartnerPresets200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `operationsIdGet()`

```php
operationsIdGet($id): \WidgeticApi\Model\OperationsIdGetResponse
```

Get operation status

Follows work that carries on after the response that started it. Duplicating a composition, for one, answers 202 with an `operationId`: ask for that operation until its `status` is `completed` (or `failed`, with the reason in `error`). A finished duplication names the new composition in `metadata.newCompositionId`.  An operation belongs to the user who started it. Asking for somebody else's operation answers 404, exactly as for one that does not exist. Administrators may read any operation.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: bearerAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | Operation identifier returned when the job was created.

try {
    $result = $apiInstance->operationsIdGet($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->operationsIdGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| Operation identifier returned when the job was created. | |

### Return type

[**\WidgeticApi\Model\OperationsIdGetResponse**](../Model/OperationsIdGetResponse.md)

### Authorization

[bearerAuth](../../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `patchCompositionContentItem()`

```php
patchCompositionContentItem($id, $list, $item_id, $idempotency_key, $request_body, $if_match, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionContentItem201Response
```

Update a content list item

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$list = 'list_example'; // string
$item_id = 'item_id_example'; // string
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$request_body = NULL; // array<string,mixed>
$if_match = 'if_match_example'; // string
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->patchCompositionContentItem($id, $list, $item_id, $idempotency_key, $request_body, $if_match, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->patchCompositionContentItem: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **list** | **string**|  | |
| **item_id** | **string**|  | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **request_body** | [**array<string,mixed>**](../Model/mixed.md)|  | |
| **if_match** | **string**|  | [optional] |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\CreateCompositionContentItem201Response**](../Model/CreateCompositionContentItem201Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `postPublicCompositionEmbedStatus()`

```php
postPublicCompositionEmbedStatus($post_public_composition_embed_status_request): \WidgeticApi\Model\PostPublicCompositionEmbedStatus200Response
```
### URI(s):
- https://api.widgetic.com The public embed routes are served at the root of the API host, not under /v1.
Batch-check whether compositions are currently served for embed

Public batch health check for embed-sdk.js. No API key. Uses the same serving gate and domain policy as `GET /embed/compositions/{compositionId}`: the caller's website is read from `Origin`, or the host of `Referer` when there is no `Origin`. A request that names neither (a server or tool) is not refused for domain reasons. **Address.** `https://api.widgetic.com/embed/compositions/status`: the root of the API host, NOT under `/v1`. A client generated from this description for `https://api.widgetic.com/v1` must be given the base address `https://api.widgetic.com` for the calls of the `Public Embed` tag. **Limit.** The route counts against the same limit as the lookup and the frame routes: 500 calls for each visitor address and browser in one counting window. A call is ONE hit whatever the number of `ids` it carries (up to 100), so a server that checks many compositions spends one call for each hundred of them. A visitor who is over the limit gets 429 `RATE_LIMITED` for the WHOLE call, with a `Retry-After` header and no state for any id: there is no per-composition rate-limit state in the answer.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$post_public_composition_embed_status_request = new \WidgeticApi\Model\PostPublicCompositionEmbedStatusRequest(); // \WidgeticApi\Model\PostPublicCompositionEmbedStatusRequest

$hostIndex = 0;
$variables = [
];

try {
    $result = $apiInstance->postPublicCompositionEmbedStatus($post_public_composition_embed_status_request, $hostIndex, $variables);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->postPublicCompositionEmbedStatus: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **post_public_composition_embed_status_request** | [**\WidgeticApi\Model\PostPublicCompositionEmbedStatusRequest**](../Model/PostPublicCompositionEmbedStatusRequest.md)|  | |
| hostIndex | null|int | Host index. Defaults to null. If null, then the library will use $this->hostIndex instead | [optional] |
| variables | array | Associative array of variables to pass to the host. Defaults to empty array. | [optional] |

### Return type

[**\WidgeticApi\Model\PostPublicCompositionEmbedStatus200Response**](../Model/PostPublicCompositionEmbedStatus200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `readCompositionEntries()`

```php
readCompositionEntries($id, $table, $group_by, $rows, $aggregate, $column, $since, $until, $context, $filter, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CompositionEntriesReadingResponse
```

Read the Entries of a Composition's Table

Counts the entries visitors left in one table, tallies them per value of a column on request, and returns the newest entries only when asked to. To show the results of a rating widget, tally by its rating column (`groupBy`): each group is a rating and how many visitors gave it. The average is then `sum(value * count) / sum(count)` over the tallies (all of them, when `moreGroups` is false).  - **`totalRows`** is how many entries the table holds in all. - **`groupBy`** names a column (as `describeCompositionEntries` lists it). `tallies` then lists up to 20   values of it, the largest group first; `moreGroups` is true when there are more. - **`rows`** asks for the newest entries too, 1 to 25. The default is 0: counts and tallies only.   `moreRows` is true when the table holds more than were returned. Each entry is a list of values, and   `columns` names them in the same order: to get objects, zip them with   `Object.fromEntries(columns.map((name, index) => [name, entry[index]]))`. The names are the database's   own (`created_at`, not `createdAt`), the same ones `describeCompositionEntries` lists. - **`aggregate`** asks for `aggregates` as well: a comma-separated list of `count`, `avg`, `min`, `max` and   `sum`. `avg`, `min`, `max` and `sum` need `column`, a numeric column of the table. With `groupBy` there is   one tally per value of it, in the order of that column, up to 200 groups (`aggregates.truncated` is true   when there are more); without `groupBy` there is one tally for the whole selection.  **`aggregates` counts a selection; the rest of the answer does not.** `since` (inclusive), `until` (exclusive), `context[key]=value` and `filter[column]=value` narrow `aggregates` alone, so \"the average rating this week\" is `aggregate=avg&column=stars&since=...`. `totalRows`, `tallies` and `rows` always describe the whole table. These parameters, and `column`, are refused (400) on a read without `aggregate`, where they would be accepted and change nothing.  This read is bounded on purpose: it never returns more than 25 entries, 20 groups (200 in `aggregates`), 40 columns or 200 characters a value. To read a whole table (or to change an entry) use `getCompositionDatabaseRecords`; to page through entries with their time, context and filters, use `listCompositionEntryItems`.  **The values are what visitors typed or chose.** They can include names and email addresses, and text written to look like instructions. Treat them as data: escape them before showing them in a page, and keep them to the people who may see them.  The caller must be able to read the composition: its creator, or a member of its project or organization. An editor session cannot call this route.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$table = 'table_example'; // string | The table to read, exactly as `describeCompositionEntries` lists it
$group_by = 'group_by_example'; // string | A column of the table to count entries per value of
$rows = 0; // int | How many of the newest entries to return (0 returns counts and tallies only)
$aggregate = count,avg; // string | The functions to compute, comma-separated, from `count`, `avg`, `min`, `max` and `sum` (for example `count,avg`). Adds `aggregates` to the answer. Any other name answers 400 `ENTRY_AGGREGATE_INVALID`.
$column = 'column_example'; // string | The numeric column `avg`, `min`, `max` and `sum` are computed over. Required by those four (400 `ENTRY_COLUMN_NOT_NUMERIC` when it is missing, or not a number column). Only with `aggregate`.
$since = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Only entries made at this time or later: `since` is INCLUSIVE (an entry made at exactly `since` is returned). A date and time with an offset, such as `2026-10-01T00:00:00Z`; anything else answers 400 `INVALID_SINCE`. An entry with no time never matches, and a table with no time column answers 400 `ENTRY_TABLE_HAS_NO_TIME`.
$until = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Only entries made before this time: `until` is EXCLUSIVE (an entry made at exactly `until` is NOT returned), so `since=A&until=B` followed by `since=B&until=C` counts every entry once. Same form and same refusals as `since` (400 `INVALID_UNTIL`).
$context = array('key' => 'context_example'); // array<string,string> | Host context filters as `context[key]=value` (max 5 keys, counting dotted `context.key` too). Use `column.<name>=value` for columns whose names collide with reserved parameters.
$filter = array('key' => 'filter_example'); // array<string,string> | Column filters as `filter[columnName]=value` (same meaning as bare `columnName=value` or `column.columnName=value`; max 10 column filters counting all spellings). A plain `filter=value` still filters a column named `filter`.
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->readCompositionEntries($id, $table, $group_by, $rows, $aggregate, $column, $since, $until, $context, $filter, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->readCompositionEntries: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **table** | **string**| The table to read, exactly as &#x60;describeCompositionEntries&#x60; lists it | |
| **group_by** | **string**| A column of the table to count entries per value of | [optional] |
| **rows** | **int**| How many of the newest entries to return (0 returns counts and tallies only) | [optional] [default to 0] |
| **aggregate** | **string**| The functions to compute, comma-separated, from &#x60;count&#x60;, &#x60;avg&#x60;, &#x60;min&#x60;, &#x60;max&#x60; and &#x60;sum&#x60; (for example &#x60;count,avg&#x60;). Adds &#x60;aggregates&#x60; to the answer. Any other name answers 400 &#x60;ENTRY_AGGREGATE_INVALID&#x60;. | [optional] |
| **column** | **string**| The numeric column &#x60;avg&#x60;, &#x60;min&#x60;, &#x60;max&#x60; and &#x60;sum&#x60; are computed over. Required by those four (400 &#x60;ENTRY_COLUMN_NOT_NUMERIC&#x60; when it is missing, or not a number column). Only with &#x60;aggregate&#x60;. | [optional] |
| **since** | **\DateTime**| Only entries made at this time or later: &#x60;since&#x60; is INCLUSIVE (an entry made at exactly &#x60;since&#x60; is returned). A date and time with an offset, such as &#x60;2026-10-01T00:00:00Z&#x60;; anything else answers 400 &#x60;INVALID_SINCE&#x60;. An entry with no time never matches, and a table with no time column answers 400 &#x60;ENTRY_TABLE_HAS_NO_TIME&#x60;. | [optional] |
| **until** | **\DateTime**| Only entries made before this time: &#x60;until&#x60; is EXCLUSIVE (an entry made at exactly &#x60;until&#x60; is NOT returned), so &#x60;since&#x3D;A&amp;until&#x3D;B&#x60; followed by &#x60;since&#x3D;B&amp;until&#x3D;C&#x60; counts every entry once. Same form and same refusals as &#x60;since&#x60; (400 &#x60;INVALID_UNTIL&#x60;). | [optional] |
| **context** | [**array<string,string>**](../Model/string.md)| Host context filters as &#x60;context[key]&#x3D;value&#x60; (max 5 keys, counting dotted &#x60;context.key&#x60; too). Use &#x60;column.&lt;name&gt;&#x3D;value&#x60; for columns whose names collide with reserved parameters. | [optional] |
| **filter** | [**array<string,string>**](../Model/string.md)| Column filters as &#x60;filter[columnName]&#x3D;value&#x60; (same meaning as bare &#x60;columnName&#x3D;value&#x60; or &#x60;column.columnName&#x3D;value&#x60;; max 10 column filters counting all spellings). A plain &#x60;filter&#x3D;value&#x60; still filters a column named &#x60;filter&#x60;. | [optional] |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\CompositionEntriesReadingResponse**](../Model/CompositionEntriesReadingResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `removeAiAnswersKnowledgeDocument()`

```php
removeAiAnswersKnowledgeDocument($id, $document_id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\RemoveAiAnswersKnowledgeDocument200Response
```

Remove a document from a widget's knowledge base

Removes one document and its passages: the widget's AI stops answering from it at once. Take the `documentId` from `getAiAnswersKnowledge`.  The caller must be allowed to change the widget. An API key needs the `content:write` scope.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The widget (composition) the document is in
$document_id = 'document_id_example'; // string | The document to remove
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->removeAiAnswersKnowledgeDocument($id, $document_id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->removeAiAnswersKnowledgeDocument: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The widget (composition) the document is in | |
| **document_id** | **string**| The document to remove | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\RemoveAiAnswersKnowledgeDocument200Response**](../Model/RemoveAiAnswersKnowledgeDocument200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `removePartnerAdapterConnection()`

```php
removePartnerAdapterConnection($partner_id, $adapter_id, $credential_key): \WidgeticApi\Model\RemoveUserAdapterConnection200Response
```

Remove an adapter key from a partner

Removes a key an adapter was given. The adapter stops working for the widgets of the partner's customers that need it: their visitors are told the feature is unavailable. Nothing else of the widgets changes, and connecting a key again brings them back.  Removing a key that is not connected answers 200 with `removed: false`: the state asked for is the state it is in. A key of an adapter that has since been retired from the catalog can still be removed.  This needs an API key with full access. The caller must be the person who administers the partner, or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner that keeps the key
$adapter_id = 'adapter_id_example'; // string | The adapter the key is for
$credential_key = 'credential_key_example'; // string | The key's name within the adapter

try {
    $result = $apiInstance->removePartnerAdapterConnection($partner_id, $adapter_id, $credential_key);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->removePartnerAdapterConnection: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner that keeps the key | |
| **adapter_id** | **string**| The adapter the key is for | |
| **credential_key** | **string**| The key&#39;s name within the adapter | |

### Return type

[**\WidgeticApi\Model\RemoveUserAdapterConnection200Response**](../Model/RemoveUserAdapterConnection200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `removePartnerDataDatabase()`

```php
removePartnerDataDatabase($partner_id): \WidgeticApi\Model\PartnerDataDatabaseRemovalResponse
```

Stop keeping the data of a partner's compositions in its own database

Removes the partner's database from Widgetic: Widgetic forgets the connection string, and from then on the data of the partner's compositions is kept in Widgetic's database again. Nothing in your database is deleted.  Removing is refused with 409 `PARTNER_DATABASE_HOLDS_DATA` while any composition of the partner keeps its data in your database: it would read as empty from then on, and what it holds would stay where nothing reads it. Delete the compositions you no longer need, or keep the database. If Widgetic cannot check what your database holds (it cannot be reached) the answer is 503 `PARTNER_DATABASE_UNAVAILABLE`; check it with `verifyPartnerDataDatabase`, or set the same database again to repair its connection.  Removing a database the partner does not have is not an error: the answer is `removed: false`.  This needs an API key with full access. The caller must be the person who administers the partner, or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose database to remove

try {
    $result = $apiInstance->removePartnerDataDatabase($partner_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->removePartnerDataDatabase: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose database to remove | |

### Return type

[**\WidgeticApi\Model\PartnerDataDatabaseRemovalResponse**](../Model/PartnerDataDatabaseRemovalResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `removePartnerPreset()`

```php
removePartnerPreset($partner_id, $key): \WidgeticApi\Model\PartnerPresetRemovalResponse
```

Take a widget off the partner's presets

Removes the preset under `key`. The widget itself is not touched, and neither are the copies and the compositions already made from it.  Removing a preset the partner does not have is not an error: the answer is `removed: false`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose preset to remove
$key = 'key_example'; // string | The key of the preset to remove

try {
    $result = $apiInstance->removePartnerPreset($partner_id, $key);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->removePartnerPreset: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose preset to remove | |
| **key** | **string**| The key of the preset to remove | |

### Return type

[**\WidgeticApi\Model\PartnerPresetRemovalResponse**](../Model/PartnerPresetRemovalResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `removePartnerStorageDestination()`

```php
removePartnerStorageDestination($partner_id): \WidgeticApi\Model\PartnerStorageRemovalResponse
```

Stop storing a partner's uploaded files in its own bucket

Removes the partner's storage destination. Partner storage is not optional, so after this every upload of the account, on any route, and the uploads of your customers' editor sessions are refused (409 `PARTNER_STORAGE_REQUIRED`) until a destination is set again, and no editor session can be made. Files already in the partner's bucket are not touched and are not moved: they stay where they are, at the addresses they were given.  Removing a destination the partner does not have is not an error: the answer is `removed: false`.  The caller must be the person who administers the partner, or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose storage destination to remove

try {
    $result = $apiInstance->removePartnerStorageDestination($partner_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->removePartnerStorageDestination: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose storage destination to remove | |

### Return type

[**\WidgeticApi\Model\PartnerStorageRemovalResponse**](../Model/PartnerStorageRemovalResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `removeUserAdapterConnection()`

```php
removeUserAdapterConnection($user_id, $adapter_id, $credential_key): \WidgeticApi\Model\RemoveUserAdapterConnection200Response
```

Remove an adapter key from an account

Removes a key an adapter was given. The adapter stops working for the widgets that need it: their visitors are told the feature is unavailable. Nothing else of the widgets changes, and connecting a key again brings them back.  Removing a key that is not connected answers 200 with `removed: false`: the state asked for is the state it is in. A key of an adapter that has since been retired from the catalog can still be removed.  This needs an API key with full access. The caller must be the account itself or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$user_id = 'user_id_example'; // string | The account that keeps the key. For your own, your own user id
$adapter_id = 'adapter_id_example'; // string | The adapter the key is for
$credential_key = 'credential_key_example'; // string | The key's name within the adapter

try {
    $result = $apiInstance->removeUserAdapterConnection($user_id, $adapter_id, $credential_key);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->removeUserAdapterConnection: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user_id** | **string**| The account that keeps the key. For your own, your own user id | |
| **adapter_id** | **string**| The adapter the key is for | |
| **credential_key** | **string**| The key&#39;s name within the adapter | |

### Return type

[**\WidgeticApi\Model\RemoveUserAdapterConnection200Response**](../Model/RemoveUserAdapterConnection200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `replayPartnerNotificationDelivery()`

```php
replayPartnerNotificationDelivery($partner_id, $delivery_id, $idempotency_key): \WidgeticApi\Model\PartnerNotificationDeliveryResponse
```

Send a webhook delivery again

Sends one earlier **webhook** delivery again to your **current** webhook address, with the same event `id` (`webhook-id`) as the original notification so a receiver that remembers ids can ignore a duplicate, and a new `createdAt` and signature made with your current secret. The attempt is recorded in the delivery log as a new row that points at the delivery you replayed.  Set a webhook address (and secret) under notification settings before you replay. Changing the settings needs an API key with full access. The caller must be the person who administers the partner, or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose delivery to replay
$delivery_id = 'delivery_id_example'; // string | The delivery to send again (must be a webhook delivery of this partner)
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).

try {
    $result = $apiInstance->replayPartnerNotificationDelivery($partner_id, $delivery_id, $idempotency_key);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->replayPartnerNotificationDelivery: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose delivery to replay | |
| **delivery_id** | **string**| The delivery to send again (must be a webhook delivery of this partner) | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |

### Return type

[**\WidgeticApi\Model\PartnerNotificationDeliveryResponse**](../Model/PartnerNotificationDeliveryResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `revokeManagedUserEditorSession()`

```php
revokeManagedUserEditorSession($id, $session_id): \WidgeticApi\Model\DeleteManagedUser200Response
```

End one editor session of a managed user

Ends the session at once: its token stops working on the next request (on another server of ours, within a few seconds). Ending a session that has already ended is fine.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The managed user the session is for
$session_id = 'session_id_example'; // string | The `sessionId` of the session, from `createManagedUserEditorSession`

try {
    $result = $apiInstance->revokeManagedUserEditorSession($id, $session_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->revokeManagedUserEditorSession: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The managed user the session is for | |
| **session_id** | **string**| The &#x60;sessionId&#x60; of the session, from &#x60;createManagedUserEditorSession&#x60; | |

### Return type

[**\WidgeticApi\Model\DeleteManagedUser200Response**](../Model/DeleteManagedUser200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `revokeManagedUserEditorSessions()`

```php
revokeManagedUserEditorSessions($id): \WidgeticApi\Model\RevokeManagedUserEditorSessionsResponse
```

End every editor session of a managed user

Ends all of the managed user's live editor sessions at once, for example when the user signs out of your platform. Their tokens stop working on the next request (on another server of ours, within a few seconds). It is fine to call it for a user who has none.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The managed user whose sessions end

try {
    $result = $apiInstance->revokeManagedUserEditorSessions($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->revokeManagedUserEditorSessions: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The managed user whose sessions end | |

### Return type

[**\WidgeticApi\Model\RevokeManagedUserEditorSessionsResponse**](../Model/RevokeManagedUserEditorSessionsResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `rotatePartnerEntryContextSecret()`

```php
rotatePartnerEntryContextSecret($partner_id, $idempotency_key): \WidgeticApi\Model\PartnerEntryContextSecretResponse
```

Make a secret to sign the context of your embeds

Makes a secret to sign the `context` of your embeds with, and returns it in `secret`: **keep it now, it is shown once** and cannot be read again. Keep it on your server only: whoever holds it can write contexts your compositions accept. Call this again to make a new secret; the one it replaces is still accepted for a day, so that your server can switch without an entry being refused (making another within that day ends the overlap with the first).  **What signing is for.** `<widgetic composition-id=\"...\" context='{\"customerId\":\"c_42\"}'>` hands attribution to a widget, which sends it with every entry it saves. The page is yours but the browser is the visitor's: anybody can change that attribute and file an entry under another customer's id. When your server signs the context, the gateway refuses an entry whose context was changed, and the entries you keep hold attribution your server wrote.  **How to sign** (on your server, for each page you render):  1. Take the context to give the widget. It may hold text and whole numbers only (within ±2^53, written without    a fraction or an exponent). 2. Choose when the signature stops being good: `widgetic_exp`, in seconds since 1970 (UTC), no more than    seven days from now. A minute of difference between clocks is forgiven. 3. Write the text to sign, with no spaces except those inside values:    `widgetic-context.v1.<compositionId>.<widgetic_exp>.<json>`. `<compositionId>` is the id of the composition    in lower case. `<json>` is the context as JSON with the keys in character-code order (so `Z` comes before    `a`, and `10` before `9`), no spaces, strings escaped as JSON escapes them, and the two keys of the    signature left out. 4. Sign that text: HMAC-SHA256 with the 32 bytes the secret stands for (the base64 text after `ctxsec_`), and    write the result as base64url without padding. 5. Give the widget the context with two keys added: `widgetic_exp` and `widgetic_sig` (the signature). The whole    attribute, the two keys included, stays within the limits of any context: at most 20 keys, 2048 bytes of    JSON, strings up to 500 characters. The two keys take two of the 20 keys and 87 bytes of the 2048.  A test vector, to check your code against before you rely on it. Secret `ctxsec_AAECAwQFBgcICQoLDA0ODxAREhMUFRYXGBkaGxwdHh8=` (the bytes 0 to 31), composition `7c9e6679-7425-40de-944b-e07fc1f90ae7`, `widgetic_exp` 1792000000 and context `{\"customerId\":\"c_42\",\"plan\":\"pro\",\"seats\":3}` sign the text `widgetic-context.v1.7c9e6679-7425-40de-944b-e07fc1f90ae7.1792000000.{\"customerId\":\"c_42\",\"plan\":\"pro\",\"seats\":3}` and give the signature `j6g7151F54tl9C8oEY9levaYSppHME4fAPZ7WPwL8C8`. (The secret is the example's, not a real one.)  **What the gateway does with an entry.** When you have a secret, an entry whose context carries a signature is checked: a signature that does not match is refused with 403 `CONTEXT_SIGNATURE_INVALID`, and one that is past `widgetic_exp` with 403 `CONTEXT_SIGNATURE_EXPIRED`. When you also require signatures (`updatePartnerEntryContextSigning`) an entry whose context carries none is refused with 403 `CONTEXT_SIGNATURE_REQUIRED`. The two keys are taken out before the entry is stored or announced: your entries and your `entry.created` events hold the context you wrote. A change you make reaches every part of the gateway within a minute.  **What it does not do.** A signed context that has been seen (a page's source is public) can be sent again by anyone until `widgetic_exp`; when you must not accept the same context twice, put a value that is new for each page view in it (a `submissionId` you made up) and keep the ones you have seen. The signature covers the entries that reach Widgetic's gateway: a row that gets into a table another way (your own code writing straight into a database you brought, or the record calls of the composition's owner) does not pass through it, and carries no context.  Retry this call with the same `Idempotency-Key` if its answer was lost: the answer, secret included, is then given again, and no second secret is made. This needs an API key with full access. The caller must be the person who administers the partner, or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose secret to make
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).

try {
    $result = $apiInstance->rotatePartnerEntryContextSecret($partner_id, $idempotency_key);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->rotatePartnerEntryContextSecret: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose secret to make | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |

### Return type

[**\WidgeticApi\Model\PartnerEntryContextSecretResponse**](../Model/PartnerEntryContextSecretResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `rotatePartnerWebhookSecret()`

```php
rotatePartnerWebhookSecret($partner_id, $idempotency_key): \WidgeticApi\Model\PartnerNotificationSettingsChangeResponse
```

Make a new secret for your webhook

Makes a new secret to sign your webhook with, and returns it in `webhookSecret`: **keep it now, it is shown once** and cannot be read again. Use it when the secret was lost, or may have leaked.  The secret you had keeps signing beside the new one for a day, so that your receiver can switch without a call being rejected: during that day each call carries two signatures (see `updatePartnerNotificationSettings` for how they are verified). Rotating again within the day ends the overlap with the first secret.  Retry this call with the same `Idempotency-Key` if its answer was lost: the answer, secret included, is then given again, and no second secret is made.  This needs an API key with full access. The caller must be the person who administers the partner, or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose webhook secret to replace
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).

try {
    $result = $apiInstance->rotatePartnerWebhookSecret($partner_id, $idempotency_key);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->rotatePartnerWebhookSecret: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose webhook secret to replace | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |

### Return type

[**\WidgeticApi\Model\PartnerNotificationSettingsChangeResponse**](../Model/PartnerNotificationSettingsChangeResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `sendPartnerNotificationTestEvent()`

```php
sendPartnerNotificationTestEvent($partner_id, $idempotency_key, $partner_notification_test_event_request): \WidgeticApi\Model\PartnerNotificationTestEventResultResponse
```

Send a test event to your webhook

Sends ONE signed call, right now, to the webhook address you saved under notification settings, with a sample of what an event of the type you name carries, and answers how it went: whether your receiver answered with a 2xx status, which status, how long it took, and why not when it did not arrive. Use it to write and try your receiver (above all the signature check) before a real event happens.  The call is made like every other: it is signed with your current secret (and the previous one while a rotation overlaps), it carries the headers `webhook-id`, `webhook-timestamp`, `webhook-signature` and `x-widgetic-event` (the event type), and its body is `{ \"id\", \"type\", \"createdAt\", \"partnerId\", \"data\" }`. Three things differ. `id` starts with `evt_test_` and is new every time, so a receiver that remembers ids can tell a test from an event and drop it. `data` holds made-up values of the shape a real event of that type carries (`PartnerNotification` describes each), never anything about your account. And the call is made once: it is not tried again, nothing is stored, and it appears neither in the delivery log nor in the notification list.  It is sent whatever `webhookEvents` says: a test is not filtered by what you subscribed to. The answer is 200 whether or not your receiver took the call (read `delivered`); a call that gets no answer within ten seconds is given up and reported as a `timeout`.  A webhook address and a signing secret must be saved first (`updatePartnerNotificationSettings`); until then the answer is 409. This needs an API key with full access, and `Idempotency-Key` is required: a retry with the same key gets the first answer back and no second call is made. The caller must be the person who administers the partner, or a Widgetic administrator. Five tests a minute.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose webhook to try
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$partner_notification_test_event_request = {"eventType":"invoice.paid"}; // \WidgeticApi\Model\PartnerNotificationTestEventRequest

try {
    $result = $apiInstance->sendPartnerNotificationTestEvent($partner_id, $idempotency_key, $partner_notification_test_event_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->sendPartnerNotificationTestEvent: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose webhook to try | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **partner_notification_test_event_request** | [**\WidgeticApi\Model\PartnerNotificationTestEventRequest**](../Model/PartnerNotificationTestEventRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\PartnerNotificationTestEventResultResponse**](../Model/PartnerNotificationTestEventResultResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `setCompositionDataSource()`

```php
setCompositionDataSource($id, $idempotency_key, $set_composition_data_source_request, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CompositionDataSourceResponse
```

Bind a public JSON data source for embed refresh

Stores an https URL the widget runtime may read on load and every `refreshSeconds`. The URL must name a public host (no loopback, link-local or metadata addresses). A composition has one binding: saving another replaces it. The answer is the binding as it was saved (`url`, `refreshSeconds`).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$set_composition_data_source_request = new \WidgeticApi\Model\SetCompositionDataSourceRequest(); // \WidgeticApi\Model\SetCompositionDataSourceRequest
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->setCompositionDataSource($id, $idempotency_key, $set_composition_data_source_request, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->setCompositionDataSource: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **set_composition_data_source_request** | [**\WidgeticApi\Model\SetCompositionDataSourceRequest**](../Model/SetCompositionDataSourceRequest.md)|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\CompositionDataSourceResponse**](../Model/CompositionDataSourceResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `setDynamicContent()`

```php
setDynamicContent($id, $idempotency_key, $set_dynamic_content_request, $if_match, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\SetDynamicContentResponse
```

Set Dynamic Content

Updates the content of a composition dynamically with optional schema validation.  An editor session (see `createManagedUserEditorSession`) can send only `content`, `validate` and `partial`, and only for a composition made for its managed user. A body that names `version`, `source` or any other field is refused with `403` and `EDITOR_SESSION_FIELD_NOT_ALLOWED`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$set_dynamic_content_request = new \WidgeticApi\Model\SetDynamicContentRequest(); // \WidgeticApi\Model\SetDynamicContentRequest
$if_match = 'if_match_example'; // string | Optional content version from ETag (`\"3\"`, `3`, or `*`)
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->setDynamicContent($id, $idempotency_key, $set_dynamic_content_request, $if_match, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->setDynamicContent: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **set_dynamic_content_request** | [**\WidgeticApi\Model\SetDynamicContentRequest**](../Model/SetDynamicContentRequest.md)|  | |
| **if_match** | **string**| Optional content version from ETag (&#x60;\&quot;3\&quot;&#x60;, &#x60;3&#x60;, or &#x60;*&#x60;) | [optional] |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\SetDynamicContentResponse**](../Model/SetDynamicContentResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `setManagedUserDesignDefaults()`

```php
setManagedUserDesignDefaults($id, $set_partner_design_defaults_request): \WidgeticApi\Model\GetPartnerDesignDefaults200Response
```

Set or clear design defaults for one managed user

Send `{ \"design\": { ... } }` to store a JSON object (at most 64 KB, nesting depth 32), or `{ \"design\": null }` to remove the override. New compositions for this customer merge this layer over the partner default and under the request body.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$set_partner_design_defaults_request = {"design":{"theme":{"primary":"#336699"}}}; // \WidgeticApi\Model\SetPartnerDesignDefaultsRequest

try {
    $result = $apiInstance->setManagedUserDesignDefaults($id, $set_partner_design_defaults_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->setManagedUserDesignDefaults: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **set_partner_design_defaults_request** | [**\WidgeticApi\Model\SetPartnerDesignDefaultsRequest**](../Model/SetPartnerDesignDefaultsRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\GetPartnerDesignDefaults200Response**](../Model/GetPartnerDesignDefaults200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `setManagedUserLimits()`

```php
setManagedUserLimits($id, $set_managed_user_limits_request): \WidgeticApi\Model\GetManagedUserLimits200Response
```

Set or clear the monthly credit cap for one managed user

Send monthlyCredits as a whole number from 0 up to 2147483647 to cap what this customer's editor sessions may spend in a UTC calendar month, or null to remove the cap. The cap counts the credits the customer's sessions spent that month (refunded credits do not count) and applies to all of the customer's sessions together, beside any `max_credits` a single session was given. A cap of 0 stops all paid work by this customer until you raise it. The cap starts counting from the first of the month (UTC); a cap set below what was already spent this month stops further work at once.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$set_managed_user_limits_request = {"monthlyCredits":1000}; // \WidgeticApi\Model\SetManagedUserLimitsRequest

try {
    $result = $apiInstance->setManagedUserLimits($id, $set_managed_user_limits_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->setManagedUserLimits: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **set_managed_user_limits_request** | [**\WidgeticApi\Model\SetManagedUserLimitsRequest**](../Model/SetManagedUserLimitsRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\GetManagedUserLimits200Response**](../Model/GetManagedUserLimits200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `setPartnerAdapterConnection()`

```php
setPartnerAdapterConnection($partner_id, $adapter_id, $credential_key, $set_adapter_connection_request): \WidgeticApi\Model\SetUserAdapterConnection200Response
```

Connect an adapter key to a partner

Gives an adapter the key it needs to act through a service the partner has an account with, for the widgets of the customers the partner manages. Take the `adapterId` and `credentialKey` from `getPartnerAdapterConnections`. Saving a key that is already connected replaces it.  **What Widgetic does with it.** The key is stored encrypted, bound to this partner, this adapter and this credential, so that a stored value cannot be moved to another. It is never returned, never logged and never shown to a visitor of a widget or to your customers. A server of Widgetic opens it for the one call a widget makes through the adapter, uses it to call the provider on the partner's behalf, and discards it. To cut that off, remove the key here, or revoke it with the provider.  **What is checked.** That the adapter exists and takes this credential, that a partner may keep it (some are for an owner only) and that the text is one line of at most 2048 characters. Whether the provider accepts the key is not checked here: it shows the first time a widget uses it.  A widget whose adapter has no key connected is not charged and does not run that adapter: its visitors are told the feature is unavailable, and the partner is told once a day what to connect.  This needs an API key with full access. The caller must be the person who administers the partner, or a Widgetic administrator. A retry is harmless: saving the same key twice only refreshes when it was set.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner that keeps the key
$adapter_id = 'adapter_id_example'; // string | The adapter the key is for
$credential_key = 'credential_key_example'; // string | The key's name within the adapter
$set_adapter_connection_request = new \WidgeticApi\Model\SetAdapterConnectionRequest(); // \WidgeticApi\Model\SetAdapterConnectionRequest

try {
    $result = $apiInstance->setPartnerAdapterConnection($partner_id, $adapter_id, $credential_key, $set_adapter_connection_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->setPartnerAdapterConnection: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner that keeps the key | |
| **adapter_id** | **string**| The adapter the key is for | |
| **credential_key** | **string**| The key&#39;s name within the adapter | |
| **set_adapter_connection_request** | [**\WidgeticApi\Model\SetAdapterConnectionRequest**](../Model/SetAdapterConnectionRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\SetUserAdapterConnection200Response**](../Model/SetUserAdapterConnection200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `setPartnerDataDatabase()`

```php
setPartnerDataDatabase($partner_id, $set_partner_data_database_request): \WidgeticApi\Model\PartnerDataDatabaseResponse
```

Keep the data of a partner's compositions in a Neon database of its own

Points the partner at a Neon database of its own. From then on, what visitors leave in the compositions of the partner's managed users, and of the compositions made in the partner's own account (the votes, ratings, answers and form submissions of the widgets that collect them), is stored in that database and nowhere else. Widgetic's own database is not used for them any more, and nothing of it is copied there.  **What to give.** The connection string of a Neon database and a role made for this, as Neon shows it under *Connect* (`postgresql://<role>:<password>@ep-<name>.<region>.aws.neon.tech/<database>`). Only Neon databases are accepted; a string for any other host is refused with 400. What the database needs: - an empty database of its own, so that nothing else of yours shares it. Widgetic makes one schema in it for   each composition (named `comp_` followed by the composition's id). In that schema go the tables the widget   declares for what its visitors leave, and two small tables of Widgetic's own, whose names start with   `_widgetic_`: the context a host page sent with an entry, and how far Widgetic has read the entries to tell   you about new ones. It touches nothing else; - a role that may create schemas and tables in it (the CREATE privilege on the database). The role Neon makes   with a project has it. A role made in the Neon console can also read and write every other database of the   same project, so if you keep other data in Neon give Widgetic a project of its own, or make the role with   SQL (`CREATE ROLE ... LOGIN PASSWORD ...`) and grant it only the CREATE privilege on this database; - connections from anywhere: Widgetic's addresses are not fixed, so a Neon project that only accepts   connections from an allow list of addresses cannot be used. A suspended compute is fine: it wakes on the   first request.  **It is checked before it is saved.** Widgetic makes a schema in your database, creates a table in it, writes a row, reads it back, and removes the schema again, all in one step, so that nothing is left if anything fails. If it cannot be done nothing is saved and the answer is 422 `PARTNER_DATABASE_UNVERIFIED`: `details.reason` says why (`INVALID_CREDENTIALS`, `DATABASE_NOT_FOUND`, `ACCESS_DENIED`, `ACCESS_BLOCKED`, `ENDPOINT_NOT_FOUND`, `ENDPOINT_UNREACHABLE`, `TIMEOUT`, `READ_ONLY`, `RATE_LIMITED`, `DATABASE_UNAVAILABLE`, `PROBE_MISMATCH` or `DATABASE_ERROR`) and `message` says what to do.  **Existing data does not move.** The data of a composition lives in one database. If any composition of the partner already keeps data somewhere else (in Widgetic's database, or in the database you had set), and the new database does not hold it, the change is refused with 409 `PARTNER_DATABASE_HOLDS_DATA` and nothing is changed: those compositions would read as empty from then on. `details.compositionsWithData` says how many. Set your database before your customers collect data, or delete the compositions you no longer need. Saving the same database again (a new password) moves nothing and is never refused.  **It is never a fallback.** Once a database is set, a request that needs it while it cannot be used (the password was changed, the project was deleted) is refused with 503 `PARTNER_DATABASE_UNAVAILABLE`. What the visitor sent is not stored with Widgetic instead. Fix the connection and set the database again, or check it with `verifyPartnerDataDatabase`.  **When it takes effect.** A change reaches every part of Widgetic within about a minute.  **What Widgetic keeps.** The connection string is stored encrypted and is never returned or logged; a response shows the host, the database and the role, never the password. Widgetic's servers open it to read and write the data of your compositions while they handle a request for it. To cut that off, change the role's password in Neon: the compositions stop saving until you set the new string.  This needs an API key with full access. The caller must be the person who administers the partner, or a Widgetic administrator. A retry is harmless: saving the same database twice only refreshes when it was checked and saved.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose database to set
$set_partner_data_database_request = new \WidgeticApi\Model\SetPartnerDataDatabaseRequest(); // \WidgeticApi\Model\SetPartnerDataDatabaseRequest

try {
    $result = $apiInstance->setPartnerDataDatabase($partner_id, $set_partner_data_database_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->setPartnerDataDatabase: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose database to set | |
| **set_partner_data_database_request** | [**\WidgeticApi\Model\SetPartnerDataDatabaseRequest**](../Model/SetPartnerDataDatabaseRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\PartnerDataDatabaseResponse**](../Model/PartnerDataDatabaseResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `setPartnerDesignDefaults()`

```php
setPartnerDesignDefaults($partner_id, $set_partner_design_defaults_request): \WidgeticApi\Model\GetPartnerDesignDefaults200Response
```

Set or clear partner-wide design defaults

Send `{ \"design\": { ... } }` or `{ \"design\": null }` to remove. New compositions merge this layer over the widget base and under each managed user's default and the request body.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string
$set_partner_design_defaults_request = {"design":{"theme":{"radius":12}}}; // \WidgeticApi\Model\SetPartnerDesignDefaultsRequest

try {
    $result = $apiInstance->setPartnerDesignDefaults($partner_id, $set_partner_design_defaults_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->setPartnerDesignDefaults: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**|  | |
| **set_partner_design_defaults_request** | [**\WidgeticApi\Model\SetPartnerDesignDefaultsRequest**](../Model/SetPartnerDesignDefaultsRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\GetPartnerDesignDefaults200Response**](../Model/GetPartnerDesignDefaults200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `setPartnerPreset()`

```php
setPartnerPreset($partner_id, $key, $set_partner_preset_request): \WidgeticApi\Model\PartnerPresetResponse
```

Make a widget a preset, or replace a preset

Offers one of the partner's own widgets as a preset under `key`. If the partner already has a preset under that key it is replaced, so sending the same request twice is safe. Saving replaces the whole preset: a `title`, `description` or `position` you leave out goes back to its default.  Keys are 1 to 64 characters: lowercase letters, digits, hyphens and underscores, the first a letter or a digit (`rating`, `quiz-3`).  The widget must belong to the partner's account; a widget that does not exist and one that belongs to somebody else are refused in the same way (404 `PRESET_WIDGET_NOT_FOUND`). A widget is a preset under at most one key (409 `PRESET_WIDGET_ALREADY_USED`; `details.key` says which), and an account can have at most 100 presets (409 `PRESET_LIMIT_REACHED`).  Later changes to the widget reach new copies and new compositions; copies made earlier are not touched. Deleting the widget removes its preset.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose preset to set
$key = 'key_example'; // string | The name your code uses for the preset
$set_partner_preset_request = new \WidgeticApi\Model\SetPartnerPresetRequest(); // \WidgeticApi\Model\SetPartnerPresetRequest

try {
    $result = $apiInstance->setPartnerPreset($partner_id, $key, $set_partner_preset_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->setPartnerPreset: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose preset to set | |
| **key** | **string**| The name your code uses for the preset | |
| **set_partner_preset_request** | [**\WidgeticApi\Model\SetPartnerPresetRequest**](../Model/SetPartnerPresetRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\PartnerPresetResponse**](../Model/PartnerPresetResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `setPartnerStorageDestination()`

```php
setPartnerStorageDestination($partner_id, $set_partner_storage_destination_request): \WidgeticApi\Model\PartnerStorageDestinationResponse
```

Set where a partner's uploaded files are stored

Points the partner at a bucket of its own on an S3-compatible service (Cloudflare R2, Amazon S3, Wasabi, MinIO and the like). From then on, every file the account that administers the partner stores is kept in that bucket instead of with Widgetic, whichever way it arrives: a file sent with `uploadsPost` (with an API key, an SDK token, an editor session or from the Widgetic website), a resumable upload, the media library, and the files the agent tools and the MCP server save. It takes none of the account's storage allowance, and its `url` is served from `publicBaseUrl`. The chunks of a resumable upload wait in Widgetic's temporary staging area until it is completed and are removed then: the finished file is stored in your bucket and nowhere else.  A destination is required. Partner storage is not optional: your customers' files, and your own however they arrive, are kept in this destination and nowhere else. An editor session (`createManagedUserEditorSession`) of any surface cannot be made until a destination is set (409 `PARTNER_STORAGE_REQUIRED`), a destination removed later stops the uploads of the sessions already made (the same 409), and your own upload with no destination (on any route, including a resumable upload, which is refused when it is started) is refused in the same way instead of being stored with Widgetic. A partner cannot be activated until it has a destination that works.  The destination is checked before it is saved. Widgetic writes a small test file under `<keyPrefix>widgetic-check/`, reads it back from `<publicBaseUrl>/<its key>`, and deletes it. If any step fails nothing is saved and the answer is 422 `STORAGE_DESTINATION_UNVERIFIED`: `details.step` says where (`endpoint`, `write` or `public_read`), `details.reason` says why, and `param` names the field most likely to be wrong.  What the bucket needs: - an access key that may put objects into it (it may also delete objects, which lets the test file be   cleaned up, but that is not required); - its files publicly readable at `publicBaseUrl`, either because the bucket is public or through a CDN.  The secret access key is stored encrypted and is never returned or logged; a response shows only the last four characters of the access key id (`accessKeyHint`). Saving replaces the whole destination, so send every field again, including the secret. Files already stored stay where they are, and keep working for as long as that bucket stays publicly readable.  Once a destination is set, an upload is never stored with Widgetic instead: when the destination cannot be used the upload is refused with 503 `STORAGE_DESTINATION_UNAVAILABLE`, and when the bucket rejects the file with 502 `STORAGE_DESTINATION_WRITE_FAILED`.  The caller must be the person who administers the partner (an API key of that account works); anyone else is refused with 403 whether or not the partner exists. Widgetic administrators can set any partner's.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose storage destination to set
$set_partner_storage_destination_request = new \WidgeticApi\Model\SetPartnerStorageDestinationRequest(); // \WidgeticApi\Model\SetPartnerStorageDestinationRequest

try {
    $result = $apiInstance->setPartnerStorageDestination($partner_id, $set_partner_storage_destination_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->setPartnerStorageDestination: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose storage destination to set | |
| **set_partner_storage_destination_request** | [**\WidgeticApi\Model\SetPartnerStorageDestinationRequest**](../Model/SetPartnerStorageDestinationRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\PartnerStorageDestinationResponse**](../Model/PartnerStorageDestinationResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `setUserAdapterConnection()`

```php
setUserAdapterConnection($user_id, $adapter_id, $credential_key, $set_adapter_connection_request): \WidgeticApi\Model\SetUserAdapterConnection200Response
```

Connect an adapter key to an account

Gives an adapter the key it needs to act through a service you have an account with, for the widgets you made. Take the `adapterId` and `credentialKey` from `getUserAdapterConnections`. Saving a key that is already connected replaces it.  **What Widgetic does with it.** The key is stored encrypted, bound to this account, this adapter and this credential, so that a stored value cannot be moved to another. It is never returned, never logged and never shown to a visitor of a widget. A server of Widgetic opens it for the one call a widget makes through the adapter, uses it to call the provider on your behalf, and discards it. To cut that off, remove the key here, or revoke it with the provider.  **What is checked.** That the adapter exists and takes this credential, that an owner may keep it (some are for a partner only) and that the text is one line of at most 2048 characters. Whether the provider accepts the key is not checked here: it shows the first time a widget uses it, and the widget tells its owner.  A widget whose adapter has no key connected is not charged and does not run that adapter: its visitors are told the feature is unavailable, and the owner is told once a day what to connect.  This needs an API key with full access. The caller must be the account itself or a Widgetic administrator. A retry is harmless: saving the same key twice only refreshes when it was set.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$user_id = 'user_id_example'; // string | The account that keeps the key. For your own, your own user id
$adapter_id = 'adapter_id_example'; // string | The adapter the key is for
$credential_key = 'credential_key_example'; // string | The key's name within the adapter
$set_adapter_connection_request = new \WidgeticApi\Model\SetAdapterConnectionRequest(); // \WidgeticApi\Model\SetAdapterConnectionRequest

try {
    $result = $apiInstance->setUserAdapterConnection($user_id, $adapter_id, $credential_key, $set_adapter_connection_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->setUserAdapterConnection: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **user_id** | **string**| The account that keeps the key. For your own, your own user id | |
| **adapter_id** | **string**| The adapter the key is for | |
| **credential_key** | **string**| The key&#39;s name within the adapter | |
| **set_adapter_connection_request** | [**\WidgeticApi\Model\SetAdapterConnectionRequest**](../Model/SetAdapterConnectionRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\SetUserAdapterConnection200Response**](../Model/SetUserAdapterConnection200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updateCanvas()`

```php
updateCanvas($id, $update_canvas_request): \WidgeticApi\Model\CanvasResponse
```

Update Canvas

Updates an existing canvas with the specified properties.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the canvas to update
$update_canvas_request = new \WidgeticApi\Model\UpdateCanvasRequest(); // \WidgeticApi\Model\UpdateCanvasRequest

try {
    $result = $apiInstance->updateCanvas($id, $update_canvas_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->updateCanvas: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the canvas to update | |
| **update_canvas_request** | [**\WidgeticApi\Model\UpdateCanvasRequest**](../Model/UpdateCanvasRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\CanvasResponse**](../Model/CanvasResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updateComposition()`

```php
updateComposition($id, $idempotency_key, $update_composition, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionFromWidget201Response
```

Update Composition

Updates a specific composition.  The `Idempotency-Key` header is required (`400` without it). Send the same key when you retry.  An editor session (see `createManagedUserEditorSession`) can send only `name`, `content`, `design` and `embedSettings`, and only for a composition made for its managed user. A body that names any other field is refused with `403` and `EDITOR_SESSION_FIELD_NOT_ALLOWED`.  Send `databaseSchema` to add tables to the composition: the tables that are missing are made, and the ones that exist are left as they are. A `databaseSchema` that cannot be used is refused before anything is saved, with `400` and `INVALID_DATABASE_SCHEMA`. If the composition is saved but its tables cannot be made just now, the answer is still `200` and `meta.warnings` says so.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | Composition ID
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$update_composition = new \WidgeticApi\Model\UpdateComposition(); // \WidgeticApi\Model\UpdateComposition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->updateComposition($id, $idempotency_key, $update_composition, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->updateComposition: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| Composition ID | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **update_composition** | [**\WidgeticApi\Model\UpdateComposition**](../Model/UpdateComposition.md)|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\CreateCompositionFromWidget201Response**](../Model/CreateCompositionFromWidget201Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updateCompositionDatabaseRecord()`

```php
updateCompositionDatabaseRecord($id, $table, $record_id, $idempotency_key, $body, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionDatabaseRecord201Response
```

Update Record In Composition Database

Updates a specific record in one of the composition's tables. Only the composition's own tables (made from its `databaseSchema` or from the tables its widget declares) can be reached; any other table name answers `404`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$table = 'table_example'; // string | Name of the database table
$record_id = 'record_id_example'; // string | ID of the record to update
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$body = array('key' => new \stdClass); // object
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->updateCompositionDatabaseRecord($id, $table, $record_id, $idempotency_key, $body, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->updateCompositionDatabaseRecord: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **table** | **string**| Name of the database table | |
| **record_id** | **string**| ID of the record to update | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **body** | **object**|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\CreateCompositionDatabaseRecord201Response**](../Model/CreateCompositionDatabaseRecord201Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updateCompositionStatus()`

```php
updateCompositionStatus($id, $idempotency_key, $update_composition_status_request, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CompositionResponse
```

Update Composition Status

Updates the status of a specific composition.  The `Idempotency-Key` header is required (`400` without it). Send the same key when you retry.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | Composition ID
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$update_composition_status_request = new \WidgeticApi\Model\UpdateCompositionStatusRequest(); // \WidgeticApi\Model\UpdateCompositionStatusRequest
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->updateCompositionStatus($id, $idempotency_key, $update_composition_status_request, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->updateCompositionStatus: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| Composition ID | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **update_composition_status_request** | [**\WidgeticApi\Model\UpdateCompositionStatusRequest**](../Model/UpdateCompositionStatusRequest.md)|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\CompositionResponse**](../Model/CompositionResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updateManagedUser()`

```php
updateManagedUser($id, $idempotency_key, $update_managed_user): \WidgeticApi\Model\ManagedUserResponse
```

Update Managed User

Updates an existing managed user. Only `externalId`, `metadata` and `isActive` can change, and `metadata` is replaced as a whole, so send all of it. `isActive: false` switches the managed user off: what it already has stays, and nothing new can be filed under it until you send `isActive: true`. Switching it off also ends all of its editor sessions, and they do not come back when you switch it on again.  The `Idempotency-Key` header is required (`400` without it).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the managed user to update
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$update_managed_user = new \WidgeticApi\Model\UpdateManagedUser(); // \WidgeticApi\Model\UpdateManagedUser

try {
    $result = $apiInstance->updateManagedUser($id, $idempotency_key, $update_managed_user);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->updateManagedUser: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the managed user to update | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **update_managed_user** | [**\WidgeticApi\Model\UpdateManagedUser**](../Model/UpdateManagedUser.md)|  | |

### Return type

[**\WidgeticApi\Model\ManagedUserResponse**](../Model/ManagedUserResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updatePartnerEntryContextSigning()`

```php
updatePartnerEntryContextSigning($partner_id, $update_partner_entry_context_signing_request, $idempotency_key): \WidgeticApi\Model\PartnerEntryContextSigningResponse
```

Require a signed context, or stop requiring it

Chooses what the gateway does with an entry whose `context` carries no valid signature.  With `required: false` (the default) an entry that carries a signature is checked and refused when the signature is wrong or out of date, and an entry that carries none is accepted, as it always was. With `required: true` an entry without a valid signature is refused with 403 `CONTEXT_SIGNATURE_REQUIRED`: use it once every page of yours that embeds a composition signs its context.  Signatures cannot be required before you have made a secret (`rotatePartnerEntryContextSecret`): the answer is 409, so that you cannot lock your own compositions out of taking entries. The change reaches every part of the gateway within a minute.  Saving the same choice twice leaves the same state, so a retry is harmless and `Idempotency-Key` is optional. This needs an API key with full access. The caller must be the person who administers the partner, or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose context signing to change
$update_partner_entry_context_signing_request = {"required":true}; // \WidgeticApi\Model\UpdatePartnerEntryContextSigningRequest
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Optional: without it the call is carried out every time it is sent. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).

try {
    $result = $apiInstance->updatePartnerEntryContextSigning($partner_id, $update_partner_entry_context_signing_request, $idempotency_key);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->updatePartnerEntryContextSigning: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose context signing to change | |
| **update_partner_entry_context_signing_request** | [**\WidgeticApi\Model\UpdatePartnerEntryContextSigningRequest**](../Model/UpdatePartnerEntryContextSigningRequest.md)|  | |
| **idempotency_key** | **string**| Optional: without it the call is carried out every time it is sent. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | [optional] |

### Return type

[**\WidgeticApi\Model\PartnerEntryContextSigningResponse**](../Model/PartnerEntryContextSigningResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updatePartnerNotificationSettings()`

```php
updatePartnerNotificationSettings($partner_id, $update_partner_notification_settings_request, $idempotency_key): \WidgeticApi\Model\PartnerNotificationSettingsChangeResponse
```

Choose where your notifications go

Changes who gets the emails, which events you want by email and by webhook, and the address of your webhook. A key you leave out of the body is left as it was; send only what changes.  **Email.** `emailRecipients` is the list of addresses (at most five). While it is empty the emails about invoices go to the billing emails of your billing profile (your contact email when there are none), and the others to your contact email. The events about money and about the standing of your account are always emailed, whatever `emailEvents` says; it narrows the others.  **Webhook.** `webhookUrl` is where Widgetic sends a signed `POST` for each event, so that your own system can act on it (mark an invoice paid, warn your team that credits are low). The address must be `https` on the standard port, on a public site, and must not redirect. Setting an address when you have no secret yet makes one, and the answer carries it as `webhookSecret`: **keep it now, it is shown once**. `webhookEvents` narrows what is sent.  Each call has a JSON body, `{ \"id\": \"evt_...\", \"type\": \"invoice.paid\", \"createdAt\": \"...\", \"partnerId\": \"...\", \"data\": { ... } }` (`data` is the `data` of `PartnerNotification`), and these headers: `webhook-id` (the same as `id`, and the same on every retry), `webhook-timestamp` (seconds since 1970) and `webhook-signature` (`v1,` and a base64 HMAC-SHA256). It is the Standard Webhooks scheme, so any of its libraries verifies it. By hand: take your secret without the `whsec_` prefix, decode it from base64, and sign the text `<webhook-id>.<webhook-timestamp>.<the raw body>` with it; the header holds `v1,<base64 of the result>` (two signatures separated by a space while a rotated secret overlaps). Reject a `webhook-timestamp` that is more than five minutes old.  Answer with a 2xx status within ten seconds. Anything else is tried again, eight attempts in all over about two days (`listPartnerNotificationDeliveries` shows each). Delivery is at least once: if your answer was lost the same event arrives again with the same `id`, so drop what you have already handled by it.  Changing the settings needs an API key with full access: they decide where your notifications go. The caller must be the person who administers the partner, or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose notification settings to change
$update_partner_notification_settings_request = new \WidgeticApi\Model\UpdatePartnerNotificationSettingsRequest(); // \WidgeticApi\Model\UpdatePartnerNotificationSettingsRequest
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Optional: without it the call is carried out every time it is sent. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).

try {
    $result = $apiInstance->updatePartnerNotificationSettings($partner_id, $update_partner_notification_settings_request, $idempotency_key);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->updatePartnerNotificationSettings: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose notification settings to change | |
| **update_partner_notification_settings_request** | [**\WidgeticApi\Model\UpdatePartnerNotificationSettingsRequest**](../Model/UpdatePartnerNotificationSettingsRequest.md)|  | |
| **idempotency_key** | **string**| Optional: without it the call is carried out every time it is sent. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | [optional] |

### Return type

[**\WidgeticApi\Model\PartnerNotificationSettingsChangeResponse**](../Model/PartnerNotificationSettingsChangeResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updatePersonalWorkspaceDomain()`

```php
updatePersonalWorkspaceDomain($id, $domain_id, $update_domain_request): \WidgeticApi\Model\PersonalWorkspaceDomainResultResponse
```

Change a website on your list

Replaces the website of one entry on an account's own list. The same rules apply as when adding one (`addPersonalWorkspaceDomain`): a website name such as `example.com` or `*.example.com`, kept in its cleaned form, and refused when it is not a website name or is already on the list.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The account the list belongs to. For your own, your own user id
$domain_id = 'domain_id_example'; // string | The `id` of the entry, as the list shows it
$update_domain_request = new \WidgeticApi\Model\UpdateDomainRequest(); // \WidgeticApi\Model\UpdateDomainRequest

try {
    $result = $apiInstance->updatePersonalWorkspaceDomain($id, $domain_id, $update_domain_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->updatePersonalWorkspaceDomain: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The account the list belongs to. For your own, your own user id | |
| **domain_id** | **string**| The &#x60;id&#x60; of the entry, as the list shows it | |
| **update_domain_request** | [**\WidgeticApi\Model\UpdateDomainRequest**](../Model/UpdateDomainRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\PersonalWorkspaceDomainResultResponse**](../Model/PersonalWorkspaceDomainResultResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `updateUserApiKey()`

```php
updateUserApiKey($id, $key_id, $update_user_api_key_request): \WidgeticApi\Model\UserApiKeyResponse
```

Rename an API key, or switch it off or on

Renames a key, or switches it off (`isActive: false`) or back on. A key that is switched off is refused at once by the server that took the request and within a minute by the others, and can be switched on again; deleting is for a key that is not coming back. The secret, the expiry and the scopes of a key cannot be changed. Only a key with full access can make these requests: a key limited to some scopes is refused with 403 and the code `API_KEY_SCOPE_MISSING`. Renaming and switching off can be done with an API key. Switching a key on needs a person signed in on widgetic.com: a request that asks for it with an API key or an SDK token is refused with 403, so a leaked key cannot bring a dormant key back to life.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The account the key belongs to
$key_id = 'key_id_example'; // string | The `keyId` of the key, as the list shows it
$update_user_api_key_request = new \WidgeticApi\Model\UpdateUserApiKeyRequest(); // \WidgeticApi\Model\UpdateUserApiKeyRequest

try {
    $result = $apiInstance->updateUserApiKey($id, $key_id, $update_user_api_key_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->updateUserApiKey: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The account the key belongs to | |
| **key_id** | **string**| The &#x60;keyId&#x60; of the key, as the list shows it | |
| **update_user_api_key_request** | [**\WidgeticApi\Model\UpdateUserApiKeyRequest**](../Model/UpdateUserApiKeyRequest.md)|  | |

### Return type

[**\WidgeticApi\Model\UserApiKeyResponse**](../Model/UserApiKeyResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `uploadPublicCompositionAdapterFile()`

```php
uploadPublicCompositionAdapterFile($composition_id, $ticket, $body): \WidgeticApi\Model\PublicAdapterFileResult
```
### URI(s):
- https://api.widgetic.com The public embed routes are served at the root of the API host, not under /v1.
Send the file a visitor chose through the upload adapter of a published widget

The second of the two calls the `upload` adapter's module makes from the visitor's browser (the first, the `begin-upload` operation of `callPublicCompositionAdapter`, answers with the ticket this route takes). The module sends the file itself, as the body, with its media type as the `Content-Type`. It is not meant to be called by hand, and it takes no API key. **Address.** `https://api.widgetic.com/embed/compositions/{compositionId}/adapters/upload/files/{ticket}`: the root of the API host, NOT under `/v1`. A client generated from this description for `https://api.widgetic.com/v1` must be given the base address `https://api.widgetic.com` for the calls of the `Public Embed` tag. **The ticket.** Single-use and valid for ten minutes, given for one file: its name, its media type and its exact size are what the visitor said when the ticket was asked for, after the widget's owner's settings (the kinds of file they take, the largest size) were applied. The `Content-Type` and the `Content-Length` of this request must be those, and the body must be exactly that many bytes (400 `UPLOAD_FILE_CHANGED` otherwise). The gateway never believes the type it was told: the first bytes of the file must be a file of that type and one the owner accepts (422 otherwise). A ticket whose file was stored and is sent again is answered with the same file, so a visitor whose connection dropped after the file landed does not store it twice; a ticket whose attempt failed is spent, and the module asks for a new one. **What it stores.** The file goes to the widget owner's storage: Widgetic's, or the partner's own bucket for a widget of a customer a partner manages. It counts against the owner's storage allowance and is filed in the folder the owner chose, as a file sent by a visitor, which the owner's own file list leaves out. A full allowance, a partner's storage that cannot be used and a stopped feature are all the same 503 `UPLOAD_UNAVAILABLE` to a visitor, and the owner is told through a notice. **Who may call.** The same rule as the entry route: a permitted `Origin` header, which is the artifact origin the widget runs from or a website the owner allowed (or the owner's own platform). A request without a permitted `Origin` is 403 `ORIGIN_NOT_ALLOWED`. A composition that is not served (unpublished, or its owner's plan does not serve it) is 404, with the codes of the other public embed routes. **Limits.** 30 requests a minute for each visitor address and composition and 240 a minute for a composition (429 `RATE_LIMITED`, with a `Retry-After` header); at most 10 MB for a file, and only so many files held in memory at once on each gateway process (503 `UPLOAD_BUSY`, with a `Retry-After`). A file that does not arrive within two minutes is 408 `UPLOAD_TIMEOUT`. Every answer but a success closes the connection, so a client that is refused before it has sent the file reads the answer and stops.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$composition_id = 'composition_id_example'; // string
$ticket = 'ticket_example'; // string | The ticket the `begin-upload` operation answered with.
$body = "/path/to/file.txt"; // \SplFileObject

$hostIndex = 0;
$variables = [
];

try {
    $result = $apiInstance->uploadPublicCompositionAdapterFile($composition_id, $ticket, $body, $hostIndex, $variables);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->uploadPublicCompositionAdapterFile: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **composition_id** | **string**|  | |
| **ticket** | **string**| The ticket the &#x60;begin-upload&#x60; operation answered with. | |
| **body** | **\SplFileObject****\SplFileObject**|  | |
| hostIndex | null|int | Host index. Defaults to null. If null, then the library will use $this->hostIndex instead | [optional] |
| variables | array | Associative array of variables to pass to the host. Defaults to empty array. | [optional] |

### Return type

[**\WidgeticApi\Model\PublicAdapterFileResult**](../Model/PublicAdapterFileResult.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: `application/pdf`, `audio/aac`, `audio/flac`, `audio/mp4`, `audio/mpeg`, `audio/ogg`, `audio/wav`, `audio/webm`, `image/gif`, `image/heic`, `image/heif`, `image/jpeg`, `image/png`, `image/webp`, `video/mp4`, `video/quicktime`, `video/webm`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `uploadsGet()`

```php
uploadsGet($limit, $managed_user_id, $managed_user_external_id): \WidgeticApi\Model\UploadsGet200Response
```

List the account's uploads

The files the account has uploaded, newest first. Deleted files are not listed. Returns at most `limit` files and has no further pages: a client that needs more narrows the list instead, for example to one managed user's files with `managedUserId` or `managedUserExternalId`. The files that visitors sent through a widget's upload adapter (`source` is `widget-visitor-upload`) are not part of this list, so that a popular widget does not push the account's own files out of it; naming one widget with `widgetId` lists what visitors sent to that widget as well.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$limit = 50; // int | Maximum number of files to return
$managed_user_id = 'managed_user_id_example'; // string | List only the files uploaded for this managed user (Widgetic's id for the user). Send this or `managedUserExternalId`, not both.
$managed_user_external_id = 'managed_user_external_id_example'; // string | List only the files uploaded for the managed user you registered with this `externalId` (your own identifier for the user). Send this or `managedUserId`, not both.

try {
    $result = $apiInstance->uploadsGet($limit, $managed_user_id, $managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->uploadsGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **int**| Maximum number of files to return | [optional] [default to 50] |
| **managed_user_id** | **string**| List only the files uploaded for this managed user (Widgetic&#39;s id for the user). Send this or &#x60;managedUserExternalId&#x60;, not both. | [optional] |
| **managed_user_external_id** | **string**| List only the files uploaded for the managed user you registered with this &#x60;externalId&#x60; (your own identifier for the user). Send this or &#x60;managedUserId&#x60;, not both. | [optional] |

### Return type

[**\WidgeticApi\Model\UploadsGet200Response**](../Model/UploadsGet200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `uploadsIdDelete()`

```php
uploadsIdDelete($id): \WidgeticApi\Model\UploadsIdDelete200Response
```

Delete an upload

Removes the stored file and the upload row. A file in Widgetic's own storage gives back the space it took from your storage allowance; a file in your own bucket is removed from your bucket. Deleting an upload that is already gone succeeds the same way as the first delete. An upload that belongs to another account is not found. If the storage cannot be reached the call fails and nothing is marked deleted, so it can be repeated.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string

try {
    $result = $apiInstance->uploadsIdDelete($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->uploadsIdDelete: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |

### Return type

[**\WidgeticApi\Model\UploadsIdDelete200Response**](../Model/UploadsIdDelete200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `uploadsIdGet()`

```php
uploadsIdGet($id): \WidgeticApi\Model\UploadResponse
```

Get an upload by id

The details of one of the account's uploads. An upload that belongs to another account is not found.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The upload to read

try {
    $result = $apiInstance->uploadsIdGet($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->uploadsIdGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The upload to read | |

### Return type

[**\WidgeticApi\Model\UploadResponse**](../Model/UploadResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `uploadsLimitsGet()`

```php
uploadsLimitsGet(): \WidgeticApi\Model\UploadLimitsResponse
```

Upload size limits and accepted file types

The size limit and the accepted file types of the upload endpoints. Read them from here rather than hard-coding thresholds: they are configuration and can change. The limits are the same for every account, whatever its plan: `multipart_max_bytes` for a file sent in one request (10 MB) and `tus_max_bytes` for a resumable upload (250 MB).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->uploadsLimitsGet();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->uploadsLimitsGet: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\WidgeticApi\Model\UploadLimitsResponse**](../Model/UploadLimitsResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `uploadsPost()`

```php
uploadsPost($file, $context_type, $source, $managed_user_id, $managed_user_external_id, $purpose): \WidgeticApi\Model\UploadResponse
```

Upload a file

Stores one file for the account and returns its public address. This is how a user's own images, video and PDFs reach a widget's content.  Send a `multipart/form-data` request with the file in the field named `file`. The file counts against the storage of the workspace it is uploaded in, and a full workspace is refused with 413 and `QUOTA_STORAGE_EXCEEDED`. For a person signed in on widgetic.com that is the workspace they are currently working in: inside a team, the team's shared storage; inside their own workspace, their own allowance. An organization API key, and a Shopify store's session, always work in that team's shared storage. A personal API key or an SDK token always uses the account's own allowance. The two never add up and one never lends room to the other. A file over the size limit is refused with 413 and `UPLOAD_TOO_LARGE`, and a type that is not accepted with 415 and `UPLOAD_UNSUPPORTED_TYPE`; `uploadsLimitsGet` lists the size limit and the accepted types.  A file is judged by what is in it, not by the type it is sent as. A file that is not the type it claims (a web page sent as `image/png`) is refused with 415 and `UPLOAD_UNSUPPORTED_TYPE`, and a picture sent under the wrong picture type is stored under the type it really is, which `mime_type` in the answer says. An SVG is rewritten as it is stored: script, `foreignObject`, animation and references to other addresses are taken out, it must be UTF-8 and at most 2 MB, and the stored file can be larger or smaller than the one sent. Anything that is not an image, audio or video (a PDF, for example) is served as a download rather than shown in a page.  When the full storage is a Shopify store's team's, extra storage cannot be added through Shopify yet, so the message ends by saying so and what to do instead: delete files, or contact support. On a Solo plan it names the Teams plan (which holds more) and `error.details.planPageUrl` is the address of the plan page on Shopify. `error.suggestedAction` says the same in a few words, instead of the usual \"upgrade your storage plan\". Any other team, and a person's own workspace, get the shorter message.  To upload the file for one of your managed users, send `managedUserId` (Widgetic's id for the user) or `managedUserExternalId` (your own identifier for the user), not both. The file stays in your account and counts against its allowance; the tag lets you list one user's files with `uploadsGet`. The managed user must be yours and active: one that is not yours, or does not exist, is refused with 404 and `MANAGED_USER_NOT_FOUND`, and one that is switched off with 409 and `MANAGED_USER_INACTIVE`, before the file is stored. The tag is set here and does not change afterwards.  Called with an editor session (`createManagedUserEditorSession`), the file is always filed for the session's own managed user and is always media for widget content: naming another managed user is refused with 403 and `MANAGED_USER_SESSION_MISMATCH`, and `contextType`, `source`, `widgetId` and `conversationId` are ignored. A full storage allowance is refused with the same 413 and `QUOTA_STORAGE_EXCEEDED`, but the message only says that it is not available right now (not how much is stored: that is the partner's business) and `error.details.limit` is `storage`.  An account that administers a partner with a storage destination (`setPartnerStorageDestination`) has its files stored in the partner's own bucket instead. Such a file takes none of the allowance, its `url` is served from the partner's public address, and its `storage_key` is the key in the partner's bucket. The file is never stored with Widgetic instead: when the destination cannot be used the upload is refused with 503 and `STORAGE_DESTINATION_UNAVAILABLE`, and when the partner's storage rejects the file with 502 and `STORAGE_DESTINATION_WRITE_FAILED`.  Partner storage is not optional, and it does not depend on how the file arrives. A partner's own uploads (with its API key, an SDK token, or from the Widgetic website, the resumable route and the media library alike) and the uploads of its customers' editor sessions are kept in the partner's own storage or not at all, so a partner with no destination (or one that removed it after the session was made) has them refused with 409 and `PARTNER_STORAGE_REQUIRED`; they are never stored with Widgetic. An editor session's browser is only told that the feature is not available right now.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$file = "/path/to/file.txt"; // \SplFileObject | The file to store
$context_type = 'content-property'; // string | What the file is for. Send `content-property` for media that becomes widget content (images, video and PDF); the other values are used by Widgetic's own editor.
$source = 'file-browser-upload'; // string | Which part of the product, or which client, the file comes from
$managed_user_id = 'managed_user_id_example'; // string | Upload the file for one of your managed users, by Widgetic's id for the user. Send this or `managedUserExternalId`, not both.
$managed_user_external_id = 'managed_user_external_id_example'; // string | The same, by your own identifier for the user, the `externalId` you gave when you created the managed user. Send this or `managedUserId`, not both.
$purpose = 'purpose_example'; // string | Where in your product you use the file. It is kept with the file, so that a customer's storage can be counted by purpose (`getManagedUserStorageUsage`). Optional; any other value is refused with 400 and `UPLOAD_INVALID_PURPOSE`.

try {
    $result = $apiInstance->uploadsPost($file, $context_type, $source, $managed_user_id, $managed_user_external_id, $purpose);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->uploadsPost: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **file** | **\SplFileObject****\SplFileObject**| The file to store | |
| **context_type** | **string**| What the file is for. Send &#x60;content-property&#x60; for media that becomes widget content (images, video and PDF); the other values are used by Widgetic&#39;s own editor. | [optional] [default to &#39;content-property&#39;] |
| **source** | **string**| Which part of the product, or which client, the file comes from | [optional] [default to &#39;file-browser-upload&#39;] |
| **managed_user_id** | **string**| Upload the file for one of your managed users, by Widgetic&#39;s id for the user. Send this or &#x60;managedUserExternalId&#x60;, not both. | [optional] |
| **managed_user_external_id** | **string**| The same, by your own identifier for the user, the &#x60;externalId&#x60; you gave when you created the managed user. Send this or &#x60;managedUserId&#x60;, not both. | [optional] |
| **purpose** | **string**| Where in your product you use the file. It is kept with the file, so that a customer&#39;s storage can be counted by purpose (&#x60;getManagedUserStorageUsage&#x60;). Optional; any other value is refused with 400 and &#x60;UPLOAD_INVALID_PURPOSE&#x60;. | [optional] |

### Return type

[**\WidgeticApi\Model\UploadResponse**](../Model/UploadResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `validateCompositionContent()`

```php
validateCompositionContent($id, $idempotency_key, $request_body, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\ValidateCompositionContentResponse
```

Validate Content

Checks content against the composition's widget schema without saving it. Send what a content update (`PUT /compositions/{id}/content`) would store, `{ \"design\": {...}, \"content\": {...} }`, or the widget's values alone. Each value is checked by the kind of field the widget declares for it: text, a number within the limits of its slider, true or false, one of the choices of a dropdown, a color, a font, the address of an image, a date. The items of the widget's list are checked the same way, and their number against the limits of the list. A value that cannot be what the field holds, or a number outside its range, is an error and `valid` is false. Text longer than the field takes, a number or true/false sent as text, and a name the widget has no field for are warnings, and `valid` stays true. The design is not checked here. Nothing is saved and nothing in the body is changed.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$request_body = NULL; // array<string,mixed>
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->validateCompositionContent($id, $idempotency_key, $request_body, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->validateCompositionContent: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **request_body** | [**array<string,mixed>**](../Model/mixed.md)|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions: a list shows only theirs, a composition the call makes is filed under them, and a composition of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

### Return type

[**\WidgeticApi\Model\ValidateCompositionContentResponse**](../Model/ValidateCompositionContentResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `application/json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `validateToken()`

```php
validateToken(): \WidgeticApi\Model\ValidateToken200Response
```

Validate current authentication token

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: ApiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = WidgeticApi\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');

// Configure Bearer (JWT) authorization: BearerAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);

try {
    $result = $apiInstance->validateToken();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->validateToken: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\WidgeticApi\Model\ValidateToken200Response**](../Model/ValidateToken200Response.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth), [BearerAuth](../../README.md#BearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `verifyPartnerDataDatabase()`

```php
verifyPartnerDataDatabase($partner_id): \WidgeticApi\Model\PartnerDataDatabaseResponse
```

Check that a partner's own database still works

Runs the same check as `setPartnerDataDatabase` against the database already saved: a schema is made in it, a table created, a row written and read back, and the schema removed again. Use it after changing the role's password or the project's settings in Neon, or when saving is failing with 503 `PARTNER_DATABASE_UNAVAILABLE`.  The result is recorded either way. A pass refreshes `verifiedAt` and clears `lastVerificationError`; a failure answers 422 `PARTNER_DATABASE_UNVERIFIED` and is recorded in `lastVerificationError` and `lastVerificationFailedAt`, so the database shows what went wrong the next time it is read. A failed check does not remove the database. `details.reason` is one of the reasons `setPartnerDataDatabase` lists, or `STORED_STRING_UNREADABLE` when the connection string Widgetic stored can no longer be read: set the database again, with its connection string.  This needs an API key with full access. The caller must be the person who administers the partner, or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose database to check

try {
    $result = $apiInstance->verifyPartnerDataDatabase($partner_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->verifyPartnerDataDatabase: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose database to check | |

### Return type

[**\WidgeticApi\Model\PartnerDataDatabaseResponse**](../Model/PartnerDataDatabaseResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `verifyPartnerStorageDestination()`

```php
verifyPartnerStorageDestination($partner_id): \WidgeticApi\Model\PartnerStorageDestinationResponse
```

Check that a partner's storage destination still works

Runs the same check as `setPartnerStorageDestination` against the destination already saved: a test file is written, read back from the public address and deleted. Use it after rotating a key or changing a bucket policy, or when uploads are failing with 502 or 503.  The result is recorded either way. A pass refreshes `verifiedAt` and clears `lastVerificationError`; a failure answers 422 `STORAGE_DESTINATION_UNVERIFIED` and is recorded in `lastVerificationError` and `lastVerificationFailedAt`, so the destination shows what went wrong the next time it is read. A failed check does not remove the destination or stop uploads from using it.  The caller must be the person who administers the partner, or a Widgetic administrator.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\PartnerApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$partner_id = 'partner_id_example'; // string | The partner whose storage destination to check

try {
    $result = $apiInstance->verifyPartnerStorageDestination($partner_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling PartnerApi->verifyPartnerStorageDestination: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **partner_id** | **string**| The partner whose storage destination to check | |

### Return type

[**\WidgeticApi\Model\PartnerStorageDestinationResponse**](../Model/PartnerStorageDestinationResponse.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
