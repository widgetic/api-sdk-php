# WidgeticApi\CompositionsApi

All URIs are relative to https://api.widgetic.com/v1, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**addAiAnswersKnowledgeDocument_0()**](CompositionsApi.md#addAiAnswersKnowledgeDocument_0) | **POST** /compositions/{id}/adapters/ai-answers/knowledge/documents | Add a document for a widget&#39;s AI to answer from |
| [**addAiAnswersKnowledgeFile_0()**](CompositionsApi.md#addAiAnswersKnowledgeFile_0) | **POST** /compositions/{id}/adapters/ai-answers/knowledge/documents/file | Add a text file or a picture of a document (a PDF once PDFs are read) for a widget&#39;s AI to answer from |
| [**checkCompositionAccess_0()**](CompositionsApi.md#checkCompositionAccess_0) | **GET** /compositions/{id}/access | Check Composition Access |
| [**createCompositionContentItem_0()**](CompositionsApi.md#createCompositionContentItem_0) | **POST** /compositions/{id}/content/{list}/items | Add a content list item |
| [**createCompositionDatabaseRecord_0()**](CompositionsApi.md#createCompositionDatabaseRecord_0) | **POST** /compositions/{id}/database/{table} | Create Record In Composition Database |
| [**createComposition_0()**](CompositionsApi.md#createComposition_0) | **POST** /compositions | Create Composition |
| [**deleteCompositionContentItem_0()**](CompositionsApi.md#deleteCompositionContentItem_0) | **DELETE** /compositions/{id}/content/{list}/items/{itemId} | Delete a content list item |
| [**deleteCompositionDataSource_0()**](CompositionsApi.md#deleteCompositionDataSource_0) | **DELETE** /compositions/{id}/data-source | Remove the composition data source binding |
| [**deleteCompositionDatabaseRecord_0()**](CompositionsApi.md#deleteCompositionDatabaseRecord_0) | **DELETE** /compositions/{id}/database/{table}/{recordId} | Delete Record From Composition Database |
| [**deleteComposition_0()**](CompositionsApi.md#deleteComposition_0) | **DELETE** /compositions/{id} | Delete Composition |
| [**describeCompositionEntries_0()**](CompositionsApi.md#describeCompositionEntries_0) | **GET** /compositions/{id}/entries | Describe What a Composition Keeps |
| [**duplicateComposition_0()**](CompositionsApi.md#duplicateComposition_0) | **POST** /compositions/{id}/duplicate | Duplicate Composition |
| [**getAiAnswersKnowledge_0()**](CompositionsApi.md#getAiAnswersKnowledge_0) | **GET** /compositions/{id}/adapters/ai-answers/knowledge | See the documents a widget&#39;s AI answers from |
| [**getAllCompositions_0()**](CompositionsApi.md#getAllCompositions_0) | **GET** /compositions | Get All Compositions |
| [**getCompositionById_0()**](CompositionsApi.md#getCompositionById_0) | **GET** /compositions/{id} | Get Composition |
| [**getCompositionContentSchema_0()**](CompositionsApi.md#getCompositionContentSchema_0) | **GET** /compositions/{id}/schema/content | Get Content Schema |
| [**getCompositionContent_0()**](CompositionsApi.md#getCompositionContent_0) | **GET** /compositions/{id}/content | Get Current Content |
| [**getCompositionDataSource_0()**](CompositionsApi.md#getCompositionDataSource_0) | **GET** /compositions/{id}/data-source | Read the composition data source binding |
| [**getCompositionDatabaseRecord_0()**](CompositionsApi.md#getCompositionDatabaseRecord_0) | **GET** /compositions/{id}/database/{table}/{recordId} | Get Record From Composition Database |
| [**getCompositionDatabaseRecords_0()**](CompositionsApi.md#getCompositionDatabaseRecords_0) | **GET** /compositions/{id}/database/{table} | Get All Records From Composition Database Table |
| [**getCompositionDesignSchema_0()**](CompositionsApi.md#getCompositionDesignSchema_0) | **GET** /compositions/{id}/schema/design | Get Design Schema |
| [**getCompositionDesign_0()**](CompositionsApi.md#getCompositionDesign_0) | **GET** /compositions/{id}/design | Get Composition Design |
| [**getCompositionEmbedSchema_0()**](CompositionsApi.md#getCompositionEmbedSchema_0) | **GET** /compositions/{id}/schema/embed | Get Embed Schema |
| [**getCompositionEmbedSettings_0()**](CompositionsApi.md#getCompositionEmbedSettings_0) | **GET** /compositions/{id}/embed-settings | Get Composition Embed Settings |
| [**getCompositionPreview_0()**](CompositionsApi.md#getCompositionPreview_0) | **GET** /compositions/{id}/preview | Get Composition Preview |
| [**getCompositionVersions_0()**](CompositionsApi.md#getCompositionVersions_0) | **GET** /compositions/{id}/versions | Get Composition Versions |
| [**getCompositionsBatch_0()**](CompositionsApi.md#getCompositionsBatch_0) | **POST** /compositions/batch | Get Compositions Batch |
| [**patchCompositionContentItem_0()**](CompositionsApi.md#patchCompositionContentItem_0) | **PATCH** /compositions/{id}/content/{list}/items/{itemId} | Update a content list item |
| [**readCompositionEntries_0()**](CompositionsApi.md#readCompositionEntries_0) | **GET** /compositions/{id}/entries/{table} | Read the Entries of a Composition&#39;s Table |
| [**removeAiAnswersKnowledgeDocument_0()**](CompositionsApi.md#removeAiAnswersKnowledgeDocument_0) | **DELETE** /compositions/{id}/adapters/ai-answers/knowledge/documents/{documentId} | Remove a document from a widget&#39;s knowledge base |
| [**setCompositionDataSource_0()**](CompositionsApi.md#setCompositionDataSource_0) | **PUT** /compositions/{id}/data-source | Bind a public JSON data source for embed refresh |
| [**setDynamicContent_0()**](CompositionsApi.md#setDynamicContent_0) | **PUT** /compositions/{id}/content | Set Dynamic Content |
| [**updateCompositionDatabaseRecord_0()**](CompositionsApi.md#updateCompositionDatabaseRecord_0) | **PUT** /compositions/{id}/database/{table}/{recordId} | Update Record In Composition Database |
| [**updateCompositionStatus_0()**](CompositionsApi.md#updateCompositionStatus_0) | **PUT** /compositions/{id}/status | Update Composition Status |
| [**updateComposition_0()**](CompositionsApi.md#updateComposition_0) | **PUT** /compositions/{id} | Update Composition |
| [**validateCompositionContent_0()**](CompositionsApi.md#validateCompositionContent_0) | **POST** /compositions/{id}/content/validate | Validate Content |


## `addAiAnswersKnowledgeDocument_0()`

```php
addAiAnswersKnowledgeDocument_0($id, $add_ai_answers_knowledge_document_request, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\AddAiAnswersKnowledgeDocument201Response
```

Add a document for a widget's AI to answer from

Gives the widget's AI a document to answer visitors' questions from. Send the title and the plain text. The call returns once the document is ready to be used, which takes a few seconds, longer for a long text.  **How it is used.** The text is cleaned, cut into short passages and each passage is turned into numbers (an embedding) so the widget can find the passages nearest to a question. When a visitor asks, the nearest passages and the question are shown to an AI model, which writes the answer from them and from nothing else; if the documents say nothing about the question the visitor is told so, and the owner is not charged for that question. The titles of the documents an answer used are shown to the visitor as its sources.  **What leaves Widgetic.** The text of a document is sent to OpenAI to be embedded when it is added, and the passages used for a question are sent to the AI model that writes the answer. Say so in your privacy policy.  **Treat every document as public.** An answer can quote or paraphrase anything a document says, to any visitor of the widget. Do not add passwords, keys, personal data or anything that must stay private.  **Limits.** A widget holds up to 20 documents, each up to 100000 characters, and up to 400000 characters in all (`getAiAnswersKnowledge` reports the current numbers). This call takes text. To add a text file or a picture of a document (a PDF too, once PDFs are read) without turning it into text yourself, use `addAiAnswersKnowledgeFile`. Adding a document costs no credits. The same text cannot be added twice to one widget (409).  The caller must be allowed to change the widget. An API key needs the `content:write` scope. Adds are limited to ten in ten minutes per person. A partner's customer in an editor session is one person of its own: its adds are not counted with the partner's other customers'.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The widget (composition) to add the document to
$add_ai_answers_knowledge_document_request = new \WidgeticApi\Model\AddAiAnswersKnowledgeDocumentRequest(); // \WidgeticApi\Model\AddAiAnswersKnowledgeDocumentRequest
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->addAiAnswersKnowledgeDocument_0($id, $add_ai_answers_knowledge_document_request, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->addAiAnswersKnowledgeDocument_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The widget (composition) to add the document to | |
| **add_ai_answers_knowledge_document_request** | [**\WidgeticApi\Model\AddAiAnswersKnowledgeDocumentRequest**](../Model/AddAiAnswersKnowledgeDocumentRequest.md)|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `addAiAnswersKnowledgeFile_0()`

```php
addAiAnswersKnowledgeFile_0($id, $file, $x_managed_user_id, $x_managed_user_external_id, $title): \WidgeticApi\Model\AddAiAnswersKnowledgeDocument201Response
```

Add a text file or a picture of a document (a PDF once PDFs are read) for a widget's AI to answer from

Gives the widget's AI a document made from a file. Send a `multipart/form-data` request with the file in the field named `file` and, if you like, a `title`. The file is turned into text and then added exactly as `addAiAnswersKnowledgeDocument` adds text: the same cleaning, the same limits, the same refusal of a copy of a document the widget already has. The call returns once the document is ready to be used, which takes a few seconds (a PDF is read first, so it takes longer).  **PDFs are not read yet.** For now a PDF is refused with 415, in a sentence that says what to do instead: paste the text, upload it as a text file, or upload its pages as pictures. What this description says about a PDF is what will hold from the day PDFs are read.  **Which files.** - A **PDF** (not read yet, see above), up to 10 MB and 300 pages. Its text is read and its paragraphs are put back   together. A PDF that is only pictures of pages (a scan) has no text to read: upload the pages as pictures instead.   A PDF locked with a password is refused. - A **text file**: `.txt`, `.text`, `.md`, `.markdown` or `.csv`, in UTF-8, UTF-16 or Windows-1252. - A **picture of a document**: PNG, JPEG or WebP, up to 4 MB. The text in it is read with the same text recognition   as the `ocr` adapter. - Word and other office files are not read yet: save the file as a PDF and upload that.  What a file is comes from what is in it, not from its name or the type it is sent as. A file that is none of these is refused with 415.  **The title.** Left out, the name of the file (without its extension) is the title. Visitors see the title as the source of an answer, so send one that means something to them.  **The file is not kept.** Only its text, cut into passages, is kept, and `getAiAnswersKnowledge` never returns it.  **What leaves Widgetic.** As for text, the words of the document are sent to OpenAI to be embedded when it is added, and the passages used for a question are sent to the AI model that writes the answer. A picture is also sent to the text recognition service. A PDF is read on Widgetic's own servers and is not sent anywhere to be read. Say so in your privacy policy.  **Treat every document as public.** An answer can quote or paraphrase anything a document says, to any visitor of the widget. Do not add passwords, keys, personal data or anything that must stay private.  **Limits.** The widget's limits are those of `addAiAnswersKnowledgeDocument` (up to 20 documents, each up to 100000 characters of text, and up to 400000 characters in all; `getAiAnswersKnowledge` reports the current numbers), and the file is at most 10 MB. Adding a document costs no credits. The same text cannot be added twice to one widget (409).  The caller must be allowed to change the widget. An API key needs the `content:write` scope. Adds, from text or from a file, share one limit of ten in ten minutes per person. A partner's customer in an editor session is one person of its own: its adds are not counted with the partner's other customers'.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The widget (composition) to add the document to
$file = "/path/to/file.txt"; // \SplFileObject | The file, which is a text file or a picture of a document (a PDF is not read yet). One file only
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$title = 'title_example'; // string | What the document is called, on one line. Visitors see it as the source of an answer. Left out, the name of the file stands in for it

try {
    $result = $apiInstance->addAiAnswersKnowledgeFile_0($id, $file, $x_managed_user_id, $x_managed_user_external_id, $title);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->addAiAnswersKnowledgeFile_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The widget (composition) to add the document to | |
| **file** | **\SplFileObject****\SplFileObject**| The file, which is a text file or a picture of a document (a PDF is not read yet). One file only | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **title** | **string**| What the document is called, on one line. Visitors see it as the source of an answer. Left out, the name of the file stands in for it | [optional] |

### Return type

[**\WidgeticApi\Model\AddAiAnswersKnowledgeDocument201Response**](../Model/AddAiAnswersKnowledgeDocument201Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `checkCompositionAccess_0()`

```php
checkCompositionAccess_0($id): \WidgeticApi\Model\CheckCompositionAccessResponse
```

Check Composition Access

Checks if the authenticated user can access a specific composition based on workspace context and permissions.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | Composition ID

try {
    $result = $apiInstance->checkCompositionAccess_0($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->checkCompositionAccess_0: ', $e->getMessage(), PHP_EOL;
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

## `createCompositionContentItem_0()`

```php
createCompositionContentItem_0($id, $list, $idempotency_key, $create_composition_content_item_request, $if_match, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionContentItem201Response
```

Add a content list item

Creates one item in a widget content list without replacing the whole list. Item field keys are widget data (camelCase or snake_case are kept as sent). Partners use this to keep galleries in sync.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
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
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->createCompositionContentItem_0($id, $list, $idempotency_key, $create_composition_content_item_request, $if_match, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->createCompositionContentItem_0: ', $e->getMessage(), PHP_EOL;
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
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `createCompositionDatabaseRecord_0()`

```php
createCompositionDatabaseRecord_0($id, $table, $idempotency_key, $body, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionDatabaseRecord201Response
```

Create Record In Composition Database

Creates a new record in one of the composition's tables. Only the composition's own tables (made from its `databaseSchema` or from the tables its widget declares) can be reached; any other table name answers `404`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$table = 'table_example'; // string | Name of the database table
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$body = array('key' => new \stdClass); // object
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->createCompositionDatabaseRecord_0($id, $table, $idempotency_key, $body, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->createCompositionDatabaseRecord_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **table** | **string**| Name of the database table | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **body** | **object**|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `createComposition_0()`

```php
createComposition_0($idempotency_key, $new_composition, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionFromWidget201Response
```

Create Composition

Creates a new composition.  To make the composition for one of your managed users, send `managedUserId` or `managedUserExternalId`. The composition stays in your account and is yours to edit; the tag lets you list one user's compositions with `getAllCompositions`. The managed user must be yours and active: one that is not yours, or does not exist, is answered with 404 and `MANAGED_USER_NOT_FOUND`, and one that is switched off with 409 and `MANAGED_USER_INACTIVE`. The tag is set here and does not change afterwards. A copy made with `duplicateComposition` keeps the tag of the original.  An editor session with the `creator` surface may call this to start a composition of a widget it built: it sends only `name`, `widgetId` (a widget made for the session's managed user) and `content`, and the composition is always made for that managed user.  Send `databaseSchema` to give the composition tables of its own for what visitors send it (the shape, the allowed types and the limits are described on the field). A `databaseSchema` that cannot be used is refused before anything is created, with `400` and `INVALID_DATABASE_SCHEMA`. If the composition is created but its tables cannot be made just now, the answer is still `201` and `meta.warnings` says so.  Leave `databaseSchema` out and the composition gets the tables its widget declares in its own source (`src/lib/meta/database.json`), if it declares any: they are made the same way, in a schema of the composition's own. A widget that keeps nothing leaves the composition without tables. If the widget's file cannot be used, or its tables cannot be made just now, the answer is still `201` and `meta.warnings` says so. The widget is read as it was when it was last published (as it is now, when it never was).  The `Idempotency-Key` header is required (`400` without it). Send the same key when you retry, so one composition is created, not two.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$new_composition = new \WidgeticApi\Model\NewComposition(); // \WidgeticApi\Model\NewComposition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->createComposition_0($idempotency_key, $new_composition, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->createComposition_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **new_composition** | [**\WidgeticApi\Model\NewComposition**](../Model/NewComposition.md)|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `deleteCompositionContentItem_0()`

```php
deleteCompositionContentItem_0($id, $list, $item_id, $idempotency_key, $if_match, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\DeleteCompositionContentItemResponse
```

Delete a content list item

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
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
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->deleteCompositionContentItem_0($id, $list, $item_id, $idempotency_key, $if_match, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->deleteCompositionContentItem_0: ', $e->getMessage(), PHP_EOL;
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
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `deleteCompositionDataSource_0()`

```php
deleteCompositionDataSource_0($id, $idempotency_key, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\DeleteCompositionDataSourceResponse
```

Remove the composition data source binding

Removes the binding. Asking again, or asking for a composition that had none, is not an error: the composition has no data source afterwards, and that is all `removed: true` says.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->deleteCompositionDataSource_0($id, $idempotency_key, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->deleteCompositionDataSource_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `deleteCompositionDatabaseRecord_0()`

```php
deleteCompositionDatabaseRecord_0($id, $table, $record_id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionDatabaseRecord201Response
```

Delete Record From Composition Database

Deletes a specific record from one of the composition's tables. Only the composition's own tables (made from its `databaseSchema` or from the tables its widget declares) can be reached; any other table name answers `404`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$table = 'table_example'; // string | Name of the database table
$record_id = 'record_id_example'; // string | ID of the record to delete
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->deleteCompositionDatabaseRecord_0($id, $table, $record_id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->deleteCompositionDatabaseRecord_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **table** | **string**| Name of the database table | |
| **record_id** | **string**| ID of the record to delete | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `deleteComposition_0()`

```php
deleteComposition_0($id, $x_managed_user_id, $x_managed_user_external_id)
```

Delete Composition

Deletes a specific composition, and the data it keeps (the tables it declared and what visitors left in them).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The ID of the composition to delete
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $apiInstance->deleteComposition_0($id, $x_managed_user_id, $x_managed_user_external_id);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->deleteComposition_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The ID of the composition to delete | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `describeCompositionEntries_0()`

```php
describeCompositionEntries_0($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CompositionEntriesDescriptionResponse
```

Describe What a Composition Keeps

Names the tables a composition's widget keeps entries in (the votes, ratings, answers or sign-ups its visitors left), their columns, and how many entries each holds. Call it first to learn the table and column names that `readCompositionEntries` takes.  A widget that only shows content keeps nothing of its own: the answer is `hasData: false` with no tables, and that is not an error. A table that could not be counted has `rows: null`, which is not zero.  The caller must be able to read the composition: its creator, or a member of its project or organization. An editor session cannot call this route.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->describeCompositionEntries_0($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->describeCompositionEntries_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `duplicateComposition_0()`

```php
duplicateComposition_0($id, $idempotency_key, $x_managed_user_id, $x_managed_user_external_id, $duplicate_composition_request): \WidgeticApi\Model\DuplicateComposition202Response
```

Duplicate Composition

Creates a duplicate of an existing composition for the authenticated user.  The duplicate is made after the answer: the call returns `202` with an `operationId`. Ask `GET /operations/{id}` for that operation until its `status` is `completed`; the new composition is named in `metadata.newCompositionId`. A problem with the duplicate's database (for example, tables that could not be made just now) is listed in `metadata.warnings`, which is absent when there is none.  The `Idempotency-Key` header is required (`400` without it). Send the same key when you retry, so one duplicate is made, not two.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition to duplicate
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$duplicate_composition_request = new \WidgeticApi\Model\DuplicateCompositionRequest(); // \WidgeticApi\Model\DuplicateCompositionRequest

try {
    $result = $apiInstance->duplicateComposition_0($id, $idempotency_key, $x_managed_user_id, $x_managed_user_external_id, $duplicate_composition_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->duplicateComposition_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition to duplicate | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
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

## `getAiAnswersKnowledge_0()`

```php
getAiAnswersKnowledge_0($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetAiAnswersKnowledge200Response
```

See the documents a widget's AI answers from

The `ai-answers` adapter lets a widget answer a visitor's question with text an AI model writes from documents the widget's owner provides. This lists those documents, and how much room is left for more: `totals` carries the widget's limits next to what it uses.  The list never contains what a document says, only which documents there are: their title, size and state. A `processing` document is not used to answer questions yet (or an add of it was interrupted: remove it and add it again).  Add a document with `addAiAnswersKnowledgeDocument`; remove one with `removeAiAnswersKnowledgeDocument`.  The caller must be allowed to see the widget: its owner, a partner for a customer it manages, or a Widgetic administrator. An API key needs the `content:read` scope.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The widget (composition) whose documents to list
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getAiAnswersKnowledge_0($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->getAiAnswersKnowledge_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The widget (composition) whose documents to list | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `getAllCompositions_0()`

```php
getAllCompositions_0($page, $size, $sort, $widget_id, $workspace, $project_folder, $status, $managed_user_id, $managed_user_external_id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetAllCompositions200Response
```

Get All Compositions

Retrieves all compositions with pagination support.  Pass `managedUserId` (Widgetic's id for one of your managed users) or `managedUserExternalId` (your own identifier for the user) to list only the compositions made for that managed user. The compositions of your other managed users, and your own, are left out. It combines with the other filters and with paging. A managed user that is not yours, or does not exist, is answered with 404 and `MANAGED_USER_NOT_FOUND`.  An editor session with the `creator` surface may call this to list the compositions of ONE widget it built: it must send `widgetId`, and the answer holds only the compositions made for the session's managed user.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
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
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getAllCompositions_0($page, $size, $sort, $widget_id, $workspace, $project_folder, $status, $managed_user_id, $managed_user_external_id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->getAllCompositions_0: ', $e->getMessage(), PHP_EOL;
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
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `getCompositionById_0()`

```php
getCompositionById_0($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionFromWidget201Response
```

Get Composition

Retrieves a specific composition by its ID.  The answer carries `direct`, which says whether the widget the composition is made from is drawn straight into your page (`true`) or inside a frame (`false`), or `null` while the widget has no published version. Read it before you go live: a widget drawn without a frame writes its entries from your own page, so the public entry route looks at the website that page is on. While the composition's allowed list is empty (you have not restricted the allowed websites), every website may write; once you list websites, only those may, besides Widgetic's own sites, the visitor's own machine and your own platform. A widget in a frame writes from Widgetic's own frame and is accepted whatever the list says. The public JSON of the composition stays open to every website.  For a composition a team shares (one filed under a project of an organization, or made in a Shopify store's workspace) the answer also carries `lastEditedBy` and `lastEditedAt`: who made the latest change and when, so that a teammate who opens it can be told \"Anna changed this at 14:32\". A composition in a personal project leaves both out, and so does an answer given to an editor session or to a call made for one managed user: only a person is told who a teammate is.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | Composition ID
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionById_0($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->getCompositionById_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| Composition ID | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `getCompositionContentSchema_0()`

```php
getCompositionContentSchema_0($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionContentSchemaResponse
```

Get Content Schema

Retrieves the content schema for a composition based on its widget type

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionContentSchema_0($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->getCompositionContentSchema_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `getCompositionContent_0()`

```php
getCompositionContent_0($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionContentResponse
```

Get Current Content

Retrieves the current content of a composition

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionContent_0($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->getCompositionContent_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `getCompositionDataSource_0()`

```php
getCompositionDataSource_0($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionDataSourceResponse
```

Read the composition data source binding

The data source that is bound to the composition: `url` and `refreshSeconds`. The answer's `data` is `null` when none is bound, and also when what is stored does not pass the rule for a public https address (a binding written by another path, such as the general embed-settings update, is never shown to a page unless it passes the same checks as this route).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionDataSource_0($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->getCompositionDataSource_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `getCompositionDatabaseRecord_0()`

```php
getCompositionDatabaseRecord_0($id, $table, $record_id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionDatabaseRecord201Response
```

Get Record From Composition Database

Retrieves a specific record from one of the composition's tables. Only the composition's own tables (made from its `databaseSchema` or from the tables its widget declares) can be reached; any other table name answers `404`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$table = 'table_example'; // string | Name of the database table
$record_id = 'record_id_example'; // string | ID of the record to retrieve
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionDatabaseRecord_0($id, $table, $record_id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->getCompositionDatabaseRecord_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **table** | **string**| Name of the database table | |
| **record_id** | **string**| ID of the record to retrieve | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `getCompositionDatabaseRecords_0()`

```php
getCompositionDatabaseRecords_0($id, $table, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionDatabaseRecords200Response
```

Get All Records From Composition Database Table

Retrieves all records from one of the composition's tables. Only the composition's own tables (made from its `databaseSchema` or from the tables its widget declares) can be reached; any other table name answers `404`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$table = 'table_example'; // string | Name of the database table
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionDatabaseRecords_0($id, $table, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->getCompositionDatabaseRecords_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **table** | **string**| Name of the database table | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `getCompositionDesignSchema_0()`

```php
getCompositionDesignSchema_0($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionDesignSchemaResponse
```

Get Design Schema

Retrieves the design schema for a composition based on its widget type

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionDesignSchema_0($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->getCompositionDesignSchema_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `getCompositionDesign_0()`

```php
getCompositionDesign_0($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionDesignResponse
```

Get Composition Design

Retrieves only the design field from a composition.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionDesign_0($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->getCompositionDesign_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `getCompositionEmbedSchema_0()`

```php
getCompositionEmbedSchema_0($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionEmbedSchemaResponse
```

Get Embed Schema

Retrieves the definition of the composition's Embed tab: which settings exist, what each one holds, what it defaults to, and when its control is shown. It is the third tab beside `schema/content` and `schema/design`, in the same format (`componentGroups` → `components` → `propertyGroups` → `properties`, each property with a `type`, a `defaultValue` and an `inputController`), so a client that draws those two tabs draws this one with the same code.  The schema is the same for every composition (it is the one Widgetic's own Embed Editor draws). The composition id decides who may ask: the caller must be able to read the composition.  Reading and saving the values: - `GET /compositions/{id}/embed-settings` returns what the composition saved. A composition whose Embed tab   was never saved has nothing to return; seed the form from `defaults`, which holds the `defaultValue` of   every setting that declares one. - `PUT /compositions/{id}` with `embedSettings` saves them. The gateway stores `embedSettings` as given and   does not check it against this schema; the schema is how a client knows what to put there.  A property's `visibilityCondition` says when its control is shown: `condition` is a comparison of the current values of the properties named in `dependsOn` (`useIframe === false`, `embedTarget === 'mixed' && keepDimensions === false`). While it is false the Embed Editor does not show the control.  A colour picker with `showOpacityControls` saves its opacity next to the colour, under the key `<name>_opacity` as a number from 0 to 1 (`overlayBackgroundColor` → `overlayBackgroundColor_opacity`). Its `defaultTransparency` is a percentage and the saved value a fraction (50 → 0.5).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionEmbedSchema_0($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->getCompositionEmbedSchema_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `getCompositionEmbedSettings_0()`

```php
getCompositionEmbedSettings_0($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionEmbedSettingsResponse
```

Get Composition Embed Settings

Retrieves only the embedSettings field from a composition.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionEmbedSettings_0($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->getCompositionEmbedSettings_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `getCompositionPreview_0()`

```php
getCompositionPreview_0($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionPreviewResponse
```

Get Composition Preview

Returns the address of the page an editor shows the composition in: the page of the widget's published version on the CDN, with the widget and version it is. Load it in a frame, then send the frame what to show (the content, design and embed settings you read from the composition, and every change the user makes) with `postMessage`: `{ type: 'widgetic:update', design }`, `{ type: 'widgetic:update', content }` or `{ type: 'widgetic:update', contentItems }`.  The version is the one embeds show, so the editor previews what a visitor gets. The address does not carry the composition id: an embed uses the id to fetch the saved composition itself, while an editor sends the current state (unsaved changes included).  A widget that has never been published has no page to show: the answer is 409 `WIDGET_NOT_PUBLISHED`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionPreview_0($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->getCompositionPreview_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `getCompositionVersions_0()`

```php
getCompositionVersions_0($id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\GetCompositionVersions200Response
```

Get Composition Versions

Retrieves version history for a specific composition.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | Composition ID
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->getCompositionVersions_0($id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->getCompositionVersions_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| Composition ID | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `getCompositionsBatch_0()`

```php
getCompositionsBatch_0($get_compositions_batch_request): \WidgeticApi\Model\GetCompositionsBatchResponse
```

Get Compositions Batch

Retrieves multiple compositions by their IDs in a single request. This endpoint includes domain validation for embed contexts and is used by the embed SDK.  Each composition is checked on its own. If its owner listed the websites it may appear on (the workspace's domain list, or the `allowedDomains` of a partner the owner administers) and the request comes from another website (the `Origin` header, or the host of `Referer` when there is no `Origin`), that composition is left out of `compositions` and reported in `errors` as `Domain access denied: <reason>`; the others are still returned. A request that names no website, and an owner who listed nothing, are not restricted, and a page on the visitor's own machine (`localhost`, `127.0.0.1` or `[::1]`, on any port) is always allowed. So is the website where a partner integrates Widgetic, with every subdomain of it (`platformDomain` in the answer of `GET /partners/mine`), for the compositions of that partner: a partner's list never has to name it.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$get_compositions_batch_request = new \WidgeticApi\Model\GetCompositionsBatchRequest(); // \WidgeticApi\Model\GetCompositionsBatchRequest

try {
    $result = $apiInstance->getCompositionsBatch_0($get_compositions_batch_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->getCompositionsBatch_0: ', $e->getMessage(), PHP_EOL;
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

## `patchCompositionContentItem_0()`

```php
patchCompositionContentItem_0($id, $list, $item_id, $idempotency_key, $request_body, $if_match, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionContentItem201Response
```

Update a content list item

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
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
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->patchCompositionContentItem_0($id, $list, $item_id, $idempotency_key, $request_body, $if_match, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->patchCompositionContentItem_0: ', $e->getMessage(), PHP_EOL;
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
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `readCompositionEntries_0()`

```php
readCompositionEntries_0($id, $table, $group_by, $rows, $aggregate, $column, $since, $until, $context, $filter, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CompositionEntriesReadingResponse
```

Read the Entries of a Composition's Table

Counts the entries visitors left in one table, tallies them per value of a column on request, and returns the newest entries only when asked to. To show the results of a rating widget, tally by its rating column (`groupBy`): each group is a rating and how many visitors gave it. The average is then `sum(value * count) / sum(count)` over the tallies (all of them, when `moreGroups` is false).  - **`totalRows`** is how many entries the table holds in all. - **`groupBy`** names a column (as `describeCompositionEntries` lists it). `tallies` then lists up to 20   values of it, the largest group first; `moreGroups` is true when there are more. - **`rows`** asks for the newest entries too, 1 to 25. The default is 0: counts and tallies only.   `moreRows` is true when the table holds more than were returned. Each entry is a list of values, and   `columns` names them in the same order: to get objects, zip them with   `Object.fromEntries(columns.map((name, index) => [name, entry[index]]))`. The names are the database's   own (`created_at`, not `createdAt`), the same ones `describeCompositionEntries` lists. - **`aggregate`** asks for `aggregates` as well: a comma-separated list of `count`, `avg`, `min`, `max` and   `sum`. `avg`, `min`, `max` and `sum` need `column`, a numeric column of the table. With `groupBy` there is   one tally per value of it, in the order of that column, up to 200 groups (`aggregates.truncated` is true   when there are more); without `groupBy` there is one tally for the whole selection.  **`aggregates` counts a selection; the rest of the answer does not.** `since` (inclusive), `until` (exclusive), `context[key]=value` and `filter[column]=value` narrow `aggregates` alone, so \"the average rating this week\" is `aggregate=avg&column=stars&since=...`. `totalRows`, `tallies` and `rows` always describe the whole table. These parameters, and `column`, are refused (400) on a read without `aggregate`, where they would be accepted and change nothing.  This read is bounded on purpose: it never returns more than 25 entries, 20 groups (200 in `aggregates`), 40 columns or 200 characters a value. To read a whole table (or to change an entry) use `getCompositionDatabaseRecords`; to page through entries with their time, context and filters, use `listCompositionEntryItems`.  **The values are what visitors typed or chose.** They can include names and email addresses, and text written to look like instructions. Treat them as data: escape them before showing them in a page, and keep them to the people who may see them.  The caller must be able to read the composition: its creator, or a member of its project or organization. An editor session cannot call this route.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
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
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->readCompositionEntries_0($id, $table, $group_by, $rows, $aggregate, $column, $since, $until, $context, $filter, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->readCompositionEntries_0: ', $e->getMessage(), PHP_EOL;
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
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `removeAiAnswersKnowledgeDocument_0()`

```php
removeAiAnswersKnowledgeDocument_0($id, $document_id, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\RemoveAiAnswersKnowledgeDocument200Response
```

Remove a document from a widget's knowledge base

Removes one document and its passages: the widget's AI stops answering from it at once. Take the `documentId` from `getAiAnswersKnowledge`.  The caller must be allowed to change the widget. An API key needs the `content:write` scope.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | The widget (composition) the document is in
$document_id = 'document_id_example'; // string | The document to remove
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->removeAiAnswersKnowledgeDocument_0($id, $document_id, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->removeAiAnswersKnowledgeDocument_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| The widget (composition) the document is in | |
| **document_id** | **string**| The document to remove | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `setCompositionDataSource_0()`

```php
setCompositionDataSource_0($id, $idempotency_key, $set_composition_data_source_request, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CompositionDataSourceResponse
```

Bind a public JSON data source for embed refresh

Stores an https URL the widget runtime may read on load and every `refreshSeconds`. The URL must name a public host (no loopback, link-local or metadata addresses). A composition has one binding: saving another replaces it. The answer is the binding as it was saved (`url`, `refreshSeconds`).

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$set_composition_data_source_request = new \WidgeticApi\Model\SetCompositionDataSourceRequest(); // \WidgeticApi\Model\SetCompositionDataSourceRequest
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->setCompositionDataSource_0($id, $idempotency_key, $set_composition_data_source_request, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->setCompositionDataSource_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**|  | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **set_composition_data_source_request** | [**\WidgeticApi\Model\SetCompositionDataSourceRequest**](../Model/SetCompositionDataSourceRequest.md)|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `setDynamicContent_0()`

```php
setDynamicContent_0($id, $idempotency_key, $set_dynamic_content_request, $if_match, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\SetDynamicContentResponse
```

Set Dynamic Content

Updates the content of a composition dynamically with optional schema validation.  An editor session (see `createManagedUserEditorSession`) can send only `content`, `validate` and `partial`, and only for a composition made for its managed user. A body that names `version`, `source` or any other field is refused with `403` and `EDITOR_SESSION_FIELD_NOT_ALLOWED`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$set_dynamic_content_request = new \WidgeticApi\Model\SetDynamicContentRequest(); // \WidgeticApi\Model\SetDynamicContentRequest
$if_match = 'if_match_example'; // string | Optional content version from ETag (`\"3\"`, `3`, or `*`)
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->setDynamicContent_0($id, $idempotency_key, $set_dynamic_content_request, $if_match, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->setDynamicContent_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **set_dynamic_content_request** | [**\WidgeticApi\Model\SetDynamicContentRequest**](../Model/SetDynamicContentRequest.md)|  | |
| **if_match** | **string**| Optional content version from ETag (&#x60;\&quot;3\&quot;&#x60;, &#x60;3&#x60;, or &#x60;*&#x60;) | [optional] |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `updateCompositionDatabaseRecord_0()`

```php
updateCompositionDatabaseRecord_0($id, $table, $record_id, $idempotency_key, $body, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionDatabaseRecord201Response
```

Update Record In Composition Database

Updates a specific record in one of the composition's tables. Only the composition's own tables (made from its `databaseSchema` or from the tables its widget declares) can be reached; any other table name answers `404`.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
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
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->updateCompositionDatabaseRecord_0($id, $table, $record_id, $idempotency_key, $body, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->updateCompositionDatabaseRecord_0: ', $e->getMessage(), PHP_EOL;
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
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `updateCompositionStatus_0()`

```php
updateCompositionStatus_0($id, $idempotency_key, $update_composition_status_request, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CompositionResponse
```

Update Composition Status

Updates the status of a specific composition.  The `Idempotency-Key` header is required (`400` without it). Send the same key when you retry.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | Composition ID
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$update_composition_status_request = new \WidgeticApi\Model\UpdateCompositionStatusRequest(); // \WidgeticApi\Model\UpdateCompositionStatusRequest
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->updateCompositionStatus_0($id, $idempotency_key, $update_composition_status_request, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->updateCompositionStatus_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| Composition ID | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **update_composition_status_request** | [**\WidgeticApi\Model\UpdateCompositionStatusRequest**](../Model/UpdateCompositionStatusRequest.md)|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `updateComposition_0()`

```php
updateComposition_0($id, $idempotency_key, $update_composition, $if_match, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\CreateCompositionFromWidget201Response
```

Update Composition

Updates a specific composition.  The `Idempotency-Key` header is required (`400` without it). Send the same key when you retry.  An editor session (see `createManagedUserEditorSession`) can send only `name`, `content`, `design` and `embedSettings`, and only for a composition made for its managed user. A body that names any other field is refused with `403` and `EDITOR_SESSION_FIELD_NOT_ALLOWED`.  Send `databaseSchema` to add tables to the composition: the tables that are missing are made, and the ones that exist are left as they are. A `databaseSchema` that cannot be used is refused before anything is saved, with `400` and `INVALID_DATABASE_SCHEMA`. If the composition is saved but its tables cannot be made just now, the answer is still `200` and `meta.warnings` says so.  **When several people edit the same composition.** A save that carries `content` can name the content version it started from in the `If-Match` header (the `contentVersion` of the composition you read, or the `ETag` of an earlier answer). If somebody saved the content since, nothing is overwritten: the save is refused with `412` and `CONTENT_VERSION_MISMATCH`, and `error.details.currentVersion` is the version to start again from. For a composition a team shares, `error.details` also says who got there first: `lastEditedBy` (`{ id, name }`, or `null` when nobody can be named) and `lastEditedAt`. An editor session, or a call made for one managed user, is told the version only. A save without `If-Match` still goes through, and the other person's change is replaced, as it always was.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | Composition ID
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$update_composition = new \WidgeticApi\Model\UpdateComposition(); // \WidgeticApi\Model\UpdateComposition
$if_match = 'if_match_example'; // string | Optional content version from `contentVersion` or an `ETag` (`\"3\"`, `3`, or `*`). Read only when the body has `content`.
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->updateComposition_0($id, $idempotency_key, $update_composition, $if_match, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->updateComposition_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| Composition ID | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **update_composition** | [**\WidgeticApi\Model\UpdateComposition**](../Model/UpdateComposition.md)|  | |
| **if_match** | **string**| Optional content version from &#x60;contentVersion&#x60; or an &#x60;ETag&#x60; (&#x60;\&quot;3\&quot;&#x60;, &#x60;3&#x60;, or &#x60;*&#x60;). Read only when the body has &#x60;content&#x60;. | [optional] |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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

## `validateCompositionContent_0()`

```php
validateCompositionContent_0($id, $idempotency_key, $request_body, $x_managed_user_id, $x_managed_user_external_id): \WidgeticApi\Model\ValidateCompositionContentResponse
```

Validate Content

Checks content against the composition's widget schema without saving it. Send what a content update (`PUT /compositions/{id}/content`) would store, `{ \"design\": {...}, \"content\": {...} }`, or the widget's values alone. Each value is checked by the kind of field the widget declares for it: text, a number within the limits of its slider, true or false, one of the choices of a dropdown, a color, a font, the address of an image, a date. The items of the widget's list are checked the same way, and their number against the limits of the list. A value that cannot be what the field holds, or a number outside its range, is an error and `valid` is false. Text longer than the field takes, a number or true/false sent as text, and a name the widget has no field for are warnings, and `valid` stays true. The design is not checked here. Nothing is saved and nothing in the body is changed.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\CompositionsApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the composition
$idempotency_key = 9b2d6f0a-3c41-4e5a-8d77-1f2e3a4b5c6d; // string | Required: a call without it is refused with `400`. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, `-` and `_`. Send the same key again when you retry (after a timeout, a dropped connection or a `5xx`) and the call is carried out once: the retry gets the first answer back, marked `X-Idempotency-Cached: true`. The same key with a different body is refused with `422`, and a retry that arrives while the first call is still running with `409` (see `Retry-After`).
$request_body = NULL; // array<string,mixed>
$x_managed_user_id = 3f2b8c1e-7a4d-4e0b-9c55-2d1a6b7e8f90; // string | The id Widgetic gave the managed user (`POST /managed-users`). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.
$x_managed_user_external_id = customer-1042; // string | Your own id for the managed user (its `externalId`), when you do not keep Widgetic's. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer's work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user's compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers `404` (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers `404` with `MANAGED_USER_NOT_FOUND`. An empty, repeated or malformed header is `400` with `MANAGED_USER_SCOPE_INVALID`; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with `403` and `MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE`: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer's browser holds, use an editor session. An `Idempotency-Key` is kept apart for each managed user.

try {
    $result = $apiInstance->validateCompositionContent_0($id, $idempotency_key, $request_body, $x_managed_user_id, $x_managed_user_external_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CompositionsApi->validateCompositionContent_0: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the composition | |
| **idempotency_key** | **string**| Required: a call without it is refused with &#x60;400&#x60;. A key of your own that names this one request; a UUID is ideal. It is 8 to 50 characters of letters, digits, &#x60;-&#x60; and &#x60;_&#x60;. Send the same key again when you retry (after a timeout, a dropped connection or a &#x60;5xx&#x60;) and the call is carried out once: the retry gets the first answer back, marked &#x60;X-Idempotency-Cached: true&#x60;. The same key with a different body is refused with &#x60;422&#x60;, and a retry that arrives while the first call is still running with &#x60;409&#x60; (see &#x60;Retry-After&#x60;). | |
| **request_body** | [**array<string,mixed>**](../Model/mixed.md)|  | |
| **x_managed_user_id** | **string**| The id Widgetic gave the managed user (&#x60;POST /managed-users&#x60;). Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |
| **x_managed_user_external_id** | **string**| Your own id for the managed user (its &#x60;externalId&#x60;), when you do not keep Widgetic&#39;s. Makes this call for one of your managed users, so that a mistake in your own code cannot reach another customer&#39;s work. Send this header, or the other one, never both. Left out, the call works on your whole account, as it always has. With it, the call reaches only that user&#39;s compositions and workflows: a list shows only theirs, a composition or a workflow the call makes is filed under them, and one of another user, or one that does not exist, answers &#x60;404&#x60; (the same answer, so the call cannot be used to find out what another customer has). A managed user that is not yours answers &#x60;404&#x60; with &#x60;MANAGED_USER_NOT_FOUND&#x60;. An empty, repeated or malformed header is &#x60;400&#x60; with &#x60;MANAGED_USER_SCOPE_INVALID&#x60;; an empty header is never read as no header. A call that is about the whole account, such as the list of your managed users, is refused with &#x60;403&#x60; and &#x60;MANAGED_USER_SCOPE_ROUTE_NOT_AVAILABLE&#x60;: send it without the header. Only your API key can send it. The header is a limit the call asks for: whoever holds the key can leave it out, so for a credential that a customer&#39;s browser holds, use an editor session. An &#x60;Idempotency-Key&#x60; is kept apart for each managed user. | [optional] |

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
