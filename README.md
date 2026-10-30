# OpenAPIClient-php

API documentation for the Widgetic API Gateway


## Installation & Usage

### Requirements

PHP 7.4 and later.
Should also work with PHP 8.0.

### Composer

To install the bindings via [Composer](https://getcomposer.org/), add the following to `composer.json`:

```json
{
  "repositories": [
    {
      "type": "vcs",
      "url": "https://github.com/widgetic/api-sdk-php.git"
    }
  ],
  "require": {
    "widgetic/api-sdk-php": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
<?php
require_once('/path/to/OpenAPIClient-php/vendor/autoload.php');
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');



// Configure Bearer (JWT) authorization: apiKeyAuth
$config = WidgeticApi\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new WidgeticApi\Api\BrandKitApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$asset_id = 'asset_id_example'; // string
$organization_id = 'organization_id_example'; // string

try {
    $result = $apiInstance->deleteBrandKitAsset_0($asset_id, $organization_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling BrandKitApi->deleteBrandKitAsset_0: ', $e->getMessage(), PHP_EOL;
}

```

## API Endpoints

All URIs are relative to *https://api.widgetic.com/v1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*BrandKitApi* | [**deleteBrandKitAsset_0**](docs/Api/BrandKitApi.md#deletebrandkitasset_0) | **DELETE** /brand-kit/assets/{assetId} | Remove a font or icon from the Brand Kit
*BrandKitApi* | [**deleteBrandKit_0**](docs/Api/BrandKitApi.md#deletebrandkit_0) | **DELETE** /brand-kit | Reset the Brand Kit to the default
*BrandKitApi* | [**getBrandKit_0**](docs/Api/BrandKitApi.md#getbrandkit_0) | **GET** /brand-kit | The Brand Kit of the current workspace
*BrandKitApi* | [**patchBrandKitAsset_0**](docs/Api/BrandKitApi.md#patchbrandkitasset_0) | **PATCH** /brand-kit/assets/{assetId} | Rename an icon or relabel a font variant
*BrandKitApi* | [**patchBrandKit_0**](docs/Api/BrandKitApi.md#patchbrandkit_0) | **PATCH** /brand-kit | Change part of the Brand Kit
*BrandKitApi* | [**postBrandKitFont_0**](docs/Api/BrandKitApi.md#postbrandkitfont_0) | **POST** /brand-kit/fonts | Upload a font file to the Brand Kit
*BrandKitApi* | [**postBrandKitIcon_0**](docs/Api/BrandKitApi.md#postbrandkiticon_0) | **POST** /brand-kit/icons | Add a named SVG icon to the Brand Kit
*BrandKitApi* | [**putBrandKit_0**](docs/Api/BrandKitApi.md#putbrandkit_0) | **PUT** /brand-kit | Save Brand Kit tokens
*CanvasesApi* | [**createCanvas_0**](docs/Api/CanvasesApi.md#createcanvas_0) | **POST** /canvases | Create Canvas
*CanvasesApi* | [**deleteCanvas_0**](docs/Api/CanvasesApi.md#deletecanvas_0) | **DELETE** /canvases/{id} | Delete Canvas
*CanvasesApi* | [**getAllCanvases_0**](docs/Api/CanvasesApi.md#getallcanvases_0) | **GET** /canvases | Get All Canvases
*CanvasesApi* | [**getCanvas_0**](docs/Api/CanvasesApi.md#getcanvas_0) | **GET** /canvases/{id} | Get Canvas
*CanvasesApi* | [**updateCanvas_0**](docs/Api/CanvasesApi.md#updatecanvas_0) | **PUT** /canvases/{id} | Update Canvas
*CompositionsApi* | [**addAiAnswersKnowledgeDocument_0**](docs/Api/CompositionsApi.md#addaianswersknowledgedocument_0) | **POST** /compositions/{id}/adapters/ai-answers/knowledge/documents | Add a document for a widget&#39;s AI to answer from
*CompositionsApi* | [**addAiAnswersKnowledgeFile_0**](docs/Api/CompositionsApi.md#addaianswersknowledgefile_0) | **POST** /compositions/{id}/adapters/ai-answers/knowledge/documents/file | Add a text file or a picture of a document (a PDF once PDFs are read) for a widget&#39;s AI to answer from
*CompositionsApi* | [**checkCompositionAccess_0**](docs/Api/CompositionsApi.md#checkcompositionaccess_0) | **GET** /compositions/{id}/access | Check Composition Access
*CompositionsApi* | [**createCompositionContentItem_0**](docs/Api/CompositionsApi.md#createcompositioncontentitem_0) | **POST** /compositions/{id}/content/{list}/items | Add a content list item
*CompositionsApi* | [**createCompositionDatabaseRecord_0**](docs/Api/CompositionsApi.md#createcompositiondatabaserecord_0) | **POST** /compositions/{id}/database/{table} | Create Record In Composition Database
*CompositionsApi* | [**createComposition_0**](docs/Api/CompositionsApi.md#createcomposition_0) | **POST** /compositions | Create Composition
*CompositionsApi* | [**deleteCompositionContentItem_0**](docs/Api/CompositionsApi.md#deletecompositioncontentitem_0) | **DELETE** /compositions/{id}/content/{list}/items/{itemId} | Delete a content list item
*CompositionsApi* | [**deleteCompositionDataSource_0**](docs/Api/CompositionsApi.md#deletecompositiondatasource_0) | **DELETE** /compositions/{id}/data-source | Remove the composition data source binding
*CompositionsApi* | [**deleteCompositionDatabaseRecord_0**](docs/Api/CompositionsApi.md#deletecompositiondatabaserecord_0) | **DELETE** /compositions/{id}/database/{table}/{recordId} | Delete Record From Composition Database
*CompositionsApi* | [**deleteComposition_0**](docs/Api/CompositionsApi.md#deletecomposition_0) | **DELETE** /compositions/{id} | Delete Composition
*CompositionsApi* | [**describeCompositionEntries_0**](docs/Api/CompositionsApi.md#describecompositionentries_0) | **GET** /compositions/{id}/entries | Describe What a Composition Keeps
*CompositionsApi* | [**duplicateComposition_0**](docs/Api/CompositionsApi.md#duplicatecomposition_0) | **POST** /compositions/{id}/duplicate | Duplicate Composition
*CompositionsApi* | [**getAiAnswersKnowledge_0**](docs/Api/CompositionsApi.md#getaianswersknowledge_0) | **GET** /compositions/{id}/adapters/ai-answers/knowledge | See the documents a widget&#39;s AI answers from
*CompositionsApi* | [**getAllCompositions_0**](docs/Api/CompositionsApi.md#getallcompositions_0) | **GET** /compositions | Get All Compositions
*CompositionsApi* | [**getCompositionById_0**](docs/Api/CompositionsApi.md#getcompositionbyid_0) | **GET** /compositions/{id} | Get Composition
*CompositionsApi* | [**getCompositionContentSchema_0**](docs/Api/CompositionsApi.md#getcompositioncontentschema_0) | **GET** /compositions/{id}/schema/content | Get Content Schema
*CompositionsApi* | [**getCompositionContent_0**](docs/Api/CompositionsApi.md#getcompositioncontent_0) | **GET** /compositions/{id}/content | Get Current Content
*CompositionsApi* | [**getCompositionDataSource_0**](docs/Api/CompositionsApi.md#getcompositiondatasource_0) | **GET** /compositions/{id}/data-source | Read the composition data source binding
*CompositionsApi* | [**getCompositionDatabaseRecord_0**](docs/Api/CompositionsApi.md#getcompositiondatabaserecord_0) | **GET** /compositions/{id}/database/{table}/{recordId} | Get Record From Composition Database
*CompositionsApi* | [**getCompositionDatabaseRecords_0**](docs/Api/CompositionsApi.md#getcompositiondatabaserecords_0) | **GET** /compositions/{id}/database/{table} | Get All Records From Composition Database Table
*CompositionsApi* | [**getCompositionDesignSchema_0**](docs/Api/CompositionsApi.md#getcompositiondesignschema_0) | **GET** /compositions/{id}/schema/design | Get Design Schema
*CompositionsApi* | [**getCompositionDesign_0**](docs/Api/CompositionsApi.md#getcompositiondesign_0) | **GET** /compositions/{id}/design | Get Composition Design
*CompositionsApi* | [**getCompositionEmbedSchema_0**](docs/Api/CompositionsApi.md#getcompositionembedschema_0) | **GET** /compositions/{id}/schema/embed | Get Embed Schema
*CompositionsApi* | [**getCompositionEmbedSettings_0**](docs/Api/CompositionsApi.md#getcompositionembedsettings_0) | **GET** /compositions/{id}/embed-settings | Get Composition Embed Settings
*CompositionsApi* | [**getCompositionPreview_0**](docs/Api/CompositionsApi.md#getcompositionpreview_0) | **GET** /compositions/{id}/preview | Get Composition Preview
*CompositionsApi* | [**getCompositionVersions_0**](docs/Api/CompositionsApi.md#getcompositionversions_0) | **GET** /compositions/{id}/versions | Get Composition Versions
*CompositionsApi* | [**getCompositionsBatch_0**](docs/Api/CompositionsApi.md#getcompositionsbatch_0) | **POST** /compositions/batch | Get Compositions Batch
*CompositionsApi* | [**patchCompositionContentItem_0**](docs/Api/CompositionsApi.md#patchcompositioncontentitem_0) | **PATCH** /compositions/{id}/content/{list}/items/{itemId} | Update a content list item
*CompositionsApi* | [**readCompositionEntries_0**](docs/Api/CompositionsApi.md#readcompositionentries_0) | **GET** /compositions/{id}/entries/{table} | Read the Entries of a Composition&#39;s Table
*CompositionsApi* | [**removeAiAnswersKnowledgeDocument_0**](docs/Api/CompositionsApi.md#removeaianswersknowledgedocument_0) | **DELETE** /compositions/{id}/adapters/ai-answers/knowledge/documents/{documentId} | Remove a document from a widget&#39;s knowledge base
*CompositionsApi* | [**setCompositionDataSource_0**](docs/Api/CompositionsApi.md#setcompositiondatasource_0) | **PUT** /compositions/{id}/data-source | Bind a public JSON data source for embed refresh
*CompositionsApi* | [**setDynamicContent_0**](docs/Api/CompositionsApi.md#setdynamiccontent_0) | **PUT** /compositions/{id}/content | Set Dynamic Content
*CompositionsApi* | [**updateCompositionDatabaseRecord_0**](docs/Api/CompositionsApi.md#updatecompositiondatabaserecord_0) | **PUT** /compositions/{id}/database/{table}/{recordId} | Update Record In Composition Database
*CompositionsApi* | [**updateCompositionStatus_0**](docs/Api/CompositionsApi.md#updatecompositionstatus_0) | **PUT** /compositions/{id}/status | Update Composition Status
*CompositionsApi* | [**updateComposition_0**](docs/Api/CompositionsApi.md#updatecomposition_0) | **PUT** /compositions/{id} | Update Composition
*CompositionsApi* | [**validateCompositionContent_0**](docs/Api/CompositionsApi.md#validatecompositioncontent_0) | **POST** /compositions/{id}/content/validate | Validate Content
*CreditsApi* | [**getUserCreditBalance_0**](docs/Api/CreditsApi.md#getusercreditbalance_0) | **GET** /credits/user/{userId}/balance | Get an account&#39;s credit balance
*CreditsApi* | [**getUserCreditTransactions_0**](docs/Api/CreditsApi.md#getusercredittransactions_0) | **GET** /credits/user/{userId}/transactions | List an account&#39;s credit ledger
*EntitlementsApi* | [**getManagedUserEntitlements_0**](docs/Api/EntitlementsApi.md#getmanageduserentitlements_0) | **GET** /entitlements/managed-users/{managedUserId} | Get managed user entitlements
*EntitlementsApi* | [**getPartnerEntitlements_0**](docs/Api/EntitlementsApi.md#getpartnerentitlements_0) | **GET** /entitlements/partners/{partnerId} | Get partner entitlements
*InvoicesApi* | [**getInvoicesByPartnerId_0**](docs/Api/InvoicesApi.md#getinvoicesbypartnerid_0) | **GET** /invoices/partner/{partnerId} | List a partner&#39;s invoices
*ManagedUsersApi* | [**copyPresetForManagedUser_0**](docs/Api/ManagedUsersApi.md#copypresetformanageduser_0) | **POST** /managed-users/{id}/presets/{key}/copy | Give a managed user a copy of one of your presets
*ManagedUsersApi* | [**createCompositionFromPreset_0**](docs/Api/ManagedUsersApi.md#createcompositionfrompreset_0) | **POST** /managed-users/{id}/presets/{key}/composition | Create a composition from one of your presets in one call
*ManagedUsersApi* | [**createManagedUserEditorSession_0**](docs/Api/ManagedUsersApi.md#createmanagedusereditorsession_0) | **POST** /managed-users/{id}/editor-sessions | Create an editor session for a managed user
*ManagedUsersApi* | [**createManagedUser_0**](docs/Api/ManagedUsersApi.md#createmanageduser_0) | **POST** /managed-users | Create Managed User
*ManagedUsersApi* | [**deleteManagedUser_0**](docs/Api/ManagedUsersApi.md#deletemanageduser_0) | **DELETE** /managed-users/{id} | Delete Managed User
*ManagedUsersApi* | [**getAllManagedUsers_0**](docs/Api/ManagedUsersApi.md#getallmanagedusers_0) | **GET** /managed-users | Get Managed Users
*ManagedUsersApi* | [**getManagedUserById_0**](docs/Api/ManagedUsersApi.md#getmanageduserbyid_0) | **GET** /managed-users/{id} | Get Managed User By ID
*ManagedUsersApi* | [**getManagedUserDesignDefaults_0**](docs/Api/ManagedUsersApi.md#getmanageduserdesigndefaults_0) | **GET** /managed-users/{id}/design-defaults | Read design defaults for one managed user
*ManagedUsersApi* | [**getManagedUserLimits_0**](docs/Api/ManagedUsersApi.md#getmanageduserlimits_0) | **GET** /managed-users/{id}/limits | Read monthly credit cap and usage for one managed user
*ManagedUsersApi* | [**getManagedUserStorageUsage_0**](docs/Api/ManagedUsersApi.md#getmanageduserstorageusage_0) | **GET** /managed-users/{id}/storage-usage | Storage used by one managed user&#39;s uploads
*ManagedUsersApi* | [**getManagedUserUsage_0**](docs/Api/ManagedUsersApi.md#getmanageduserusage_0) | **GET** /managed-users/{id}/usage | What a managed user&#39;s editor sessions spent
*ManagedUsersApi* | [**getManagedUsersByManagerId_0**](docs/Api/ManagedUsersApi.md#getmanagedusersbymanagerid_0) | **GET** /users/{managerId}/managed-users | Get Managed Users By Manager
*ManagedUsersApi* | [**revokeManagedUserEditorSession_0**](docs/Api/ManagedUsersApi.md#revokemanagedusereditorsession_0) | **DELETE** /managed-users/{id}/editor-sessions/{sessionId} | End one editor session of a managed user
*ManagedUsersApi* | [**revokeManagedUserEditorSessions_0**](docs/Api/ManagedUsersApi.md#revokemanagedusereditorsessions_0) | **DELETE** /managed-users/{id}/editor-sessions | End every editor session of a managed user
*ManagedUsersApi* | [**setManagedUserDesignDefaults_0**](docs/Api/ManagedUsersApi.md#setmanageduserdesigndefaults_0) | **PUT** /managed-users/{id}/design-defaults | Set or clear design defaults for one managed user
*ManagedUsersApi* | [**setManagedUserLimits_0**](docs/Api/ManagedUsersApi.md#setmanageduserlimits_0) | **PUT** /managed-users/{id}/limits | Set or clear the monthly credit cap for one managed user
*ManagedUsersApi* | [**updateManagedUser_0**](docs/Api/ManagedUsersApi.md#updatemanageduser_0) | **PUT** /managed-users/{id} | Update Managed User
*OperationsApi* | [**operationsIdGet_0**](docs/Api/OperationsApi.md#operationsidget_0) | **GET** /operations/{id} | Get operation status
*PartnerApi* | [**addAiAnswersKnowledgeDocument**](docs/Api/PartnerApi.md#addaianswersknowledgedocument) | **POST** /compositions/{id}/adapters/ai-answers/knowledge/documents | Add a document for a widget&#39;s AI to answer from
*PartnerApi* | [**addAiAnswersKnowledgeFile**](docs/Api/PartnerApi.md#addaianswersknowledgefile) | **POST** /compositions/{id}/adapters/ai-answers/knowledge/documents/file | Add a text file or a picture of a document (a PDF once PDFs are read) for a widget&#39;s AI to answer from
*PartnerApi* | [**addPersonalWorkspaceDomain**](docs/Api/PartnerApi.md#addpersonalworkspacedomain) | **POST** /users/{id}/workspace/domains | Allow a website to show your widgets
*PartnerApi* | [**archiveWorkspaceWorkflow**](docs/Api/PartnerApi.md#archiveworkspaceworkflow) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/archive | Archive a Workflow
*PartnerApi* | [**callPublicCompositionAdapter**](docs/Api/PartnerApi.md#callpubliccompositionadapter) | **POST** /embed/compositions/{compositionId}/adapters/{adapterId}/{operation} | Call a gateway operation of an adapter a published widget uses
*PartnerApi* | [**checkCompositionAccess**](docs/Api/PartnerApi.md#checkcompositionaccess) | **GET** /compositions/{id}/access | Check Composition Access
*PartnerApi* | [**confirmPartnerAdapterConnection**](docs/Api/PartnerApi.md#confirmpartneradapterconnection) | **POST** /partners/{partnerId}/adapter-connections/{adapterId}/{credentialKey}/confirm | Confirm a partner&#39;s adapter address with the code that was emailed to it
*PartnerApi* | [**confirmUserAdapterConnection**](docs/Api/PartnerApi.md#confirmuseradapterconnection) | **POST** /users/{userId}/adapter-connections/{adapterId}/{credentialKey}/confirm | Confirm an adapter address with the code that was emailed to it
*PartnerApi* | [**copyPresetForManagedUser**](docs/Api/PartnerApi.md#copypresetformanageduser) | **POST** /managed-users/{id}/presets/{key}/copy | Give a managed user a copy of one of your presets
*PartnerApi* | [**createCanvas**](docs/Api/PartnerApi.md#createcanvas) | **POST** /canvases | Create Canvas
*PartnerApi* | [**createComposition**](docs/Api/PartnerApi.md#createcomposition) | **POST** /compositions | Create Composition
*PartnerApi* | [**createCompositionContentItem**](docs/Api/PartnerApi.md#createcompositioncontentitem) | **POST** /compositions/{id}/content/{list}/items | Add a content list item
*PartnerApi* | [**createCompositionDatabaseRecord**](docs/Api/PartnerApi.md#createcompositiondatabaserecord) | **POST** /compositions/{id}/database/{table} | Create Record In Composition Database
*PartnerApi* | [**createCompositionFromPreset**](docs/Api/PartnerApi.md#createcompositionfrompreset) | **POST** /managed-users/{id}/presets/{key}/composition | Create a composition from one of your presets in one call
*PartnerApi* | [**createCompositionFromWidget**](docs/Api/PartnerApi.md#createcompositionfromwidget) | **POST** /widgets/{id}/composition | Create a composition for a widget in one call
*PartnerApi* | [**createManagedUser**](docs/Api/PartnerApi.md#createmanageduser) | **POST** /managed-users | Create Managed User
*PartnerApi* | [**createManagedUserEditorSession**](docs/Api/PartnerApi.md#createmanagedusereditorsession) | **POST** /managed-users/{id}/editor-sessions | Create an editor session for a managed user
*PartnerApi* | [**createPartnerExtraCreditsInvoice**](docs/Api/PartnerApi.md#createpartnerextracreditsinvoice) | **POST** /partners/{partnerId}/credits/extra-invoice | Buy extra credits for a partner
*PartnerApi* | [**createPublicCompositionEntry**](docs/Api/PartnerApi.md#createpubliccompositionentry) | **POST** /embed/compositions/{compositionId}/entries/{table} | Append a visitor entry through the gateway
*PartnerApi* | [**createUserApiKey**](docs/Api/PartnerApi.md#createuserapikey) | **POST** /users/{id}/keys | Create an API key
*PartnerApi* | [**createWidget**](docs/Api/PartnerApi.md#createwidget) | **POST** /widgets | Create Widget
*PartnerApi* | [**createWorkspaceWorkflow**](docs/Api/PartnerApi.md#createworkspaceworkflow) | **POST** /workspaces/{workspaceId}/workflows | Create a Workflow
*PartnerApi* | [**createWorkspaceWorkflowFromPreset**](docs/Api/PartnerApi.md#createworkspaceworkflowfrompreset) | **POST** /workspaces/{workspaceId}/workflows/from-preset | Start a Workflow from a starting point
*PartnerApi* | [**deleteBrandKit**](docs/Api/PartnerApi.md#deletebrandkit) | **DELETE** /brand-kit | Reset the Brand Kit to the default
*PartnerApi* | [**deleteBrandKitAsset**](docs/Api/PartnerApi.md#deletebrandkitasset) | **DELETE** /brand-kit/assets/{assetId} | Remove a font or icon from the Brand Kit
*PartnerApi* | [**deleteCanvas**](docs/Api/PartnerApi.md#deletecanvas) | **DELETE** /canvases/{id} | Delete Canvas
*PartnerApi* | [**deleteComposition**](docs/Api/PartnerApi.md#deletecomposition) | **DELETE** /compositions/{id} | Delete Composition
*PartnerApi* | [**deleteCompositionContentItem**](docs/Api/PartnerApi.md#deletecompositioncontentitem) | **DELETE** /compositions/{id}/content/{list}/items/{itemId} | Delete a content list item
*PartnerApi* | [**deleteCompositionDataSource**](docs/Api/PartnerApi.md#deletecompositiondatasource) | **DELETE** /compositions/{id}/data-source | Remove the composition data source binding
*PartnerApi* | [**deleteCompositionDatabaseRecord**](docs/Api/PartnerApi.md#deletecompositiondatabaserecord) | **DELETE** /compositions/{id}/database/{table}/{recordId} | Delete Record From Composition Database
*PartnerApi* | [**deleteCompositionEntryItems**](docs/Api/PartnerApi.md#deletecompositionentryitems) | **DELETE** /compositions/{id}/entries/{table}/items | Delete composition entry items by id or host context
*PartnerApi* | [**deleteManagedUser**](docs/Api/PartnerApi.md#deletemanageduser) | **DELETE** /managed-users/{id} | Delete Managed User
*PartnerApi* | [**deletePersonalWorkspaceDomain**](docs/Api/PartnerApi.md#deletepersonalworkspacedomain) | **DELETE** /users/{id}/workspace/domains/{domainId} | Stop allowing a website to show your widgets
*PartnerApi* | [**deleteUserApiKey**](docs/Api/PartnerApi.md#deleteuserapikey) | **DELETE** /users/{id}/keys/{keyId} | Delete an API key
*PartnerApi* | [**deleteWorkspaceWorkflow**](docs/Api/PartnerApi.md#deleteworkspaceworkflow) | **DELETE** /workspaces/{workspaceId}/workflows/{workflowId} | Delete a Workflow
*PartnerApi* | [**describeCompositionEntries**](docs/Api/PartnerApi.md#describecompositionentries) | **GET** /compositions/{id}/entries | Describe What a Composition Keeps
*PartnerApi* | [**discardWorkspaceWorkflowChanges**](docs/Api/PartnerApi.md#discardworkspaceworkflowchanges) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/discard | Discard the Unpublished Changes of a Workflow
*PartnerApi* | [**duplicateComposition**](docs/Api/PartnerApi.md#duplicatecomposition) | **POST** /compositions/{id}/duplicate | Duplicate Composition
*PartnerApi* | [**duplicateWorkspaceWorkflow**](docs/Api/PartnerApi.md#duplicateworkspaceworkflow) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/duplicate | Duplicate a Workflow
*PartnerApi* | [**exportCompositionEntryItems**](docs/Api/PartnerApi.md#exportcompositionentryitems) | **GET** /compositions/{id}/entries/{table}/export | Export composition entry items
*PartnerApi* | [**getAiAnswersKnowledge**](docs/Api/PartnerApi.md#getaianswersknowledge) | **GET** /compositions/{id}/adapters/ai-answers/knowledge | See the documents a widget&#39;s AI answers from
*PartnerApi* | [**getAllCanvases**](docs/Api/PartnerApi.md#getallcanvases) | **GET** /canvases | Get All Canvases
*PartnerApi* | [**getAllCompositions**](docs/Api/PartnerApi.md#getallcompositions) | **GET** /compositions | Get All Compositions
*PartnerApi* | [**getAllManagedUsers**](docs/Api/PartnerApi.md#getallmanagedusers) | **GET** /managed-users | Get Managed Users
*PartnerApi* | [**getBrandKit**](docs/Api/PartnerApi.md#getbrandkit) | **GET** /brand-kit | The Brand Kit of the current workspace
*PartnerApi* | [**getCanvas**](docs/Api/PartnerApi.md#getcanvas) | **GET** /canvases/{id} | Get Canvas
*PartnerApi* | [**getCompositionById**](docs/Api/PartnerApi.md#getcompositionbyid) | **GET** /compositions/{id} | Get Composition
*PartnerApi* | [**getCompositionContent**](docs/Api/PartnerApi.md#getcompositioncontent) | **GET** /compositions/{id}/content | Get Current Content
*PartnerApi* | [**getCompositionContentSchema**](docs/Api/PartnerApi.md#getcompositioncontentschema) | **GET** /compositions/{id}/schema/content | Get Content Schema
*PartnerApi* | [**getCompositionDataSource**](docs/Api/PartnerApi.md#getcompositiondatasource) | **GET** /compositions/{id}/data-source | Read the composition data source binding
*PartnerApi* | [**getCompositionDatabaseRecord**](docs/Api/PartnerApi.md#getcompositiondatabaserecord) | **GET** /compositions/{id}/database/{table}/{recordId} | Get Record From Composition Database
*PartnerApi* | [**getCompositionDatabaseRecords**](docs/Api/PartnerApi.md#getcompositiondatabaserecords) | **GET** /compositions/{id}/database/{table} | Get All Records From Composition Database Table
*PartnerApi* | [**getCompositionDesign**](docs/Api/PartnerApi.md#getcompositiondesign) | **GET** /compositions/{id}/design | Get Composition Design
*PartnerApi* | [**getCompositionDesignSchema**](docs/Api/PartnerApi.md#getcompositiondesignschema) | **GET** /compositions/{id}/schema/design | Get Design Schema
*PartnerApi* | [**getCompositionEmbedSchema**](docs/Api/PartnerApi.md#getcompositionembedschema) | **GET** /compositions/{id}/schema/embed | Get Embed Schema
*PartnerApi* | [**getCompositionEmbedSettings**](docs/Api/PartnerApi.md#getcompositionembedsettings) | **GET** /compositions/{id}/embed-settings | Get Composition Embed Settings
*PartnerApi* | [**getCompositionPreview**](docs/Api/PartnerApi.md#getcompositionpreview) | **GET** /compositions/{id}/preview | Get Composition Preview
*PartnerApi* | [**getCompositionVersions**](docs/Api/PartnerApi.md#getcompositionversions) | **GET** /compositions/{id}/versions | Get Composition Versions
*PartnerApi* | [**getCompositionsBatch**](docs/Api/PartnerApi.md#getcompositionsbatch) | **POST** /compositions/batch | Get Compositions Batch
*PartnerApi* | [**getInvoicesByPartnerId**](docs/Api/PartnerApi.md#getinvoicesbypartnerid) | **GET** /invoices/partner/{partnerId} | List a partner&#39;s invoices
*PartnerApi* | [**getManagedUserById**](docs/Api/PartnerApi.md#getmanageduserbyid) | **GET** /managed-users/{id} | Get Managed User By ID
*PartnerApi* | [**getManagedUserDesignDefaults**](docs/Api/PartnerApi.md#getmanageduserdesigndefaults) | **GET** /managed-users/{id}/design-defaults | Read design defaults for one managed user
*PartnerApi* | [**getManagedUserEntitlements**](docs/Api/PartnerApi.md#getmanageduserentitlements) | **GET** /entitlements/managed-users/{managedUserId} | Get managed user entitlements
*PartnerApi* | [**getManagedUserLimits**](docs/Api/PartnerApi.md#getmanageduserlimits) | **GET** /managed-users/{id}/limits | Read monthly credit cap and usage for one managed user
*PartnerApi* | [**getManagedUserStorageUsage**](docs/Api/PartnerApi.md#getmanageduserstorageusage) | **GET** /managed-users/{id}/storage-usage | Storage used by one managed user&#39;s uploads
*PartnerApi* | [**getManagedUserUsage**](docs/Api/PartnerApi.md#getmanageduserusage) | **GET** /managed-users/{id}/usage | What a managed user&#39;s editor sessions spent
*PartnerApi* | [**getManagedUsersByManagerId**](docs/Api/PartnerApi.md#getmanagedusersbymanagerid) | **GET** /users/{managerId}/managed-users | Get Managed Users By Manager
*PartnerApi* | [**getMyPartners**](docs/Api/PartnerApi.md#getmypartners) | **GET** /partners/mine | Find the partner you administer
*PartnerApi* | [**getPartnerAdapterConnections**](docs/Api/PartnerApi.md#getpartneradapterconnections) | **GET** /partners/{partnerId}/adapter-connections | See which adapter keys a partner has connected
*PartnerApi* | [**getPartnerAnalyticsByManagedUser**](docs/Api/PartnerApi.md#getpartneranalyticsbymanageduser) | **GET** /partners/{partnerId}/analytics/managed-users | What each managed user&#39;s widgets did
*PartnerApi* | [**getPartnerAnalyticsSummary**](docs/Api/PartnerApi.md#getpartneranalyticssummary) | **GET** /partners/{partnerId}/analytics/summary | What was done with a partner&#39;s published widgets
*PartnerApi* | [**getPartnerAnalyticsTimeline**](docs/Api/PartnerApi.md#getpartneranalyticstimeline) | **GET** /partners/{partnerId}/analytics/timeline | What was done with a partner&#39;s widgets, day by day
*PartnerApi* | [**getPartnerAnalyticsTopWidgets**](docs/Api/PartnerApi.md#getpartneranalyticstopwidgets) | **GET** /partners/{partnerId}/analytics/top-widgets | Which widgets were viewed the most
*PartnerApi* | [**getPartnerBillingOverview**](docs/Api/PartnerApi.md#getpartnerbillingoverview) | **GET** /partners/{partnerId}/billing-overview | Get comprehensive partner billing overview
*PartnerApi* | [**getPartnerContract**](docs/Api/PartnerApi.md#getpartnercontract) | **GET** /partners/{partnerId}/contract | Get a partner&#39;s contract
*PartnerApi* | [**getPartnerCreditBalance**](docs/Api/PartnerApi.md#getpartnercreditbalance) | **GET** /partners/{partnerId}/credits/balance | Get partner credit balance
*PartnerApi* | [**getPartnerCreditTransactions**](docs/Api/PartnerApi.md#getpartnercredittransactions) | **GET** /partners/{partnerId}/credits/transactions | Get partner credit transaction history
*PartnerApi* | [**getPartnerDataDatabase**](docs/Api/PartnerApi.md#getpartnerdatadatabase) | **GET** /partners/{partnerId}/data-database | See the Neon database a partner keeps the data of its compositions in
*PartnerApi* | [**getPartnerDesignDefaults**](docs/Api/PartnerApi.md#getpartnerdesigndefaults) | **GET** /partners/{partnerId}/design-defaults | Read partner-wide design defaults
*PartnerApi* | [**getPartnerEntitlements**](docs/Api/PartnerApi.md#getpartnerentitlements) | **GET** /entitlements/partners/{partnerId} | Get partner entitlements
*PartnerApi* | [**getPartnerEntryContextSigning**](docs/Api/PartnerApi.md#getpartnerentrycontextsigning) | **GET** /partners/{partnerId}/entry-context-signing | See how the context of your embeds is signed
*PartnerApi* | [**getPartnerNotificationSettings**](docs/Api/PartnerApi.md#getpartnernotificationsettings) | **GET** /partners/{partnerId}/notifications/settings | Where your notifications go
*PartnerApi* | [**getPartnerStorageDestination**](docs/Api/PartnerApi.md#getpartnerstoragedestination) | **GET** /partners/{partnerId}/storage | Get where a partner&#39;s uploaded files are stored
*PartnerApi* | [**getPartnerStorageUsage**](docs/Api/PartnerApi.md#getpartnerstorageusage) | **GET** /partners/{partnerId}/storage/usage | What a partner&#39;s customers store
*PartnerApi* | [**getPersonalWorkspaceDomains**](docs/Api/PartnerApi.md#getpersonalworkspacedomains) | **GET** /users/{id}/workspace/domains | List the websites allowed to show your widgets
*PartnerApi* | [**getPublicCompositionEmbed**](docs/Api/PartnerApi.md#getpubliccompositionembed) | **GET** /embed/compositions/{compositionId} | Resolve a composition UUID to a published widget URL
*PartnerApi* | [**getPublicCompositionIframe**](docs/Api/PartnerApi.md#getpubliccompositioniframe) | **GET** /embed/compositions/{compositionId}/frame | Embed a published composition with its saved values
*PartnerApi* | [**getPublicWorkflow**](docs/Api/PartnerApi.md#getpublicworkflow) | **GET** /embed/workflows/{workflowId} | Read the published Workflow of an embed
*PartnerApi* | [**getPublicWorkflowFrame**](docs/Api/PartnerApi.md#getpublicworkflowframe) | **GET** /embed/workflows/{workflowId}/frame | Show a published Workflow in a page of its own
*PartnerApi* | [**getPublicWorkflowVersion**](docs/Api/PartnerApi.md#getpublicworkflowversion) | **GET** /embed/workflows/{workflowId}/versions/{versionId} | Read one published version of a Workflow
*PartnerApi* | [**getUserAdapterConnections**](docs/Api/PartnerApi.md#getuseradapterconnections) | **GET** /users/{userId}/adapter-connections | See which adapter keys an account has connected
*PartnerApi* | [**getUserApiKeyUsageLogs**](docs/Api/PartnerApi.md#getuserapikeyusagelogs) | **GET** /users/{id}/api-keys/{keyId}/logs | Read what an API key was used for
*PartnerApi* | [**getUserApiKeys**](docs/Api/PartnerApi.md#getuserapikeys) | **GET** /users/{id}/keys | List the API keys of an account
*PartnerApi* | [**getUserCreditBalance**](docs/Api/PartnerApi.md#getusercreditbalance) | **GET** /credits/user/{userId}/balance | Get an account&#39;s credit balance
*PartnerApi* | [**getUserCreditTransactions**](docs/Api/PartnerApi.md#getusercredittransactions) | **GET** /credits/user/{userId}/transactions | List an account&#39;s credit ledger
*PartnerApi* | [**getWidgets**](docs/Api/PartnerApi.md#getwidgets) | **GET** /widgets | List Widgets
*PartnerApi* | [**getWidgetsBatch**](docs/Api/PartnerApi.md#getwidgetsbatch) | **POST** /widgets/batch | Get Widgets Batch
*PartnerApi* | [**getWorkspaceWorkflow**](docs/Api/PartnerApi.md#getworkspaceworkflow) | **GET** /workspaces/{workspaceId}/workflows/{workflowId} | Get a Workflow
*PartnerApi* | [**getWorkspaceWorkflowStats**](docs/Api/PartnerApi.md#getworkspaceworkflowstats) | **GET** /workspaces/{workspaceId}/workflows/{workflowId}/stats | Get what Visitors Did in a Workflow
*PartnerApi* | [**getWorkspaceWorkflowVersion**](docs/Api/PartnerApi.md#getworkspaceworkflowversion) | **GET** /workspaces/{workspaceId}/workflows/{workflowId}/versions/{versionId} | Get a Published Version of a Workflow
*PartnerApi* | [**listCompositionEntryItems**](docs/Api/PartnerApi.md#listcompositionentryitems) | **GET** /compositions/{id}/entries/{table}/items | List composition entry items with paging and filters
*PartnerApi* | [**listManagedUserEntries**](docs/Api/PartnerApi.md#listmanageduserentries) | **GET** /managed-users/{id}/entries | List entries across a managed user&#39;s compositions
*PartnerApi* | [**listPartnerNotificationDeliveries**](docs/Api/PartnerApi.md#listpartnernotificationdeliveries) | **GET** /partners/{partnerId}/notifications/deliveries | How your notifications reached you
*PartnerApi* | [**listPartnerNotifications**](docs/Api/PartnerApi.md#listpartnernotifications) | **GET** /partners/{partnerId}/notifications | What your partner account was told
*PartnerApi* | [**listPartnerPresets**](docs/Api/PartnerApi.md#listpartnerpresets) | **GET** /partners/{partnerId}/presets | List the widgets a partner offers as presets
*PartnerApi* | [**listPartnerWorkflowPresets**](docs/Api/PartnerApi.md#listpartnerworkflowpresets) | **GET** /partners/{partnerId}/workflow-presets | List the workflows a partner offers as places to start
*PartnerApi* | [**listWorkspaceWorkflowCompositionOptions**](docs/Api/PartnerApi.md#listworkspaceworkflowcompositionoptions) | **GET** /workspaces/{workspaceId}/workflows/composition-options | List the compositions a workflow can show, and what each can do
*PartnerApi* | [**listWorkspaceWorkflowPresets**](docs/Api/PartnerApi.md#listworkspaceworkflowpresets) | **GET** /workspaces/{workspaceId}/workflows/presets | List the starting points for a new Workflow
*PartnerApi* | [**listWorkspaceWorkflowVersions**](docs/Api/PartnerApi.md#listworkspaceworkflowversions) | **GET** /workspaces/{workspaceId}/workflows/{workflowId}/versions | List the Published Versions of a Workflow
*PartnerApi* | [**listWorkspaceWorkflows**](docs/Api/PartnerApi.md#listworkspaceworkflows) | **GET** /workspaces/{workspaceId}/workflows | List the Workflows of a Workspace
*PartnerApi* | [**operationsIdGet**](docs/Api/PartnerApi.md#operationsidget) | **GET** /operations/{id} | Get operation status
*PartnerApi* | [**patchBrandKit**](docs/Api/PartnerApi.md#patchbrandkit) | **PATCH** /brand-kit | Change part of the Brand Kit
*PartnerApi* | [**patchBrandKitAsset**](docs/Api/PartnerApi.md#patchbrandkitasset) | **PATCH** /brand-kit/assets/{assetId} | Rename an icon or relabel a font variant
*PartnerApi* | [**patchCompositionContentItem**](docs/Api/PartnerApi.md#patchcompositioncontentitem) | **PATCH** /compositions/{id}/content/{list}/items/{itemId} | Update a content list item
*PartnerApi* | [**pauseWorkspaceWorkflow**](docs/Api/PartnerApi.md#pauseworkspaceworkflow) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/pause | Pause a Workflow
*PartnerApi* | [**postBrandKitFont**](docs/Api/PartnerApi.md#postbrandkitfont) | **POST** /brand-kit/fonts | Upload a font file to the Brand Kit
*PartnerApi* | [**postBrandKitIcon**](docs/Api/PartnerApi.md#postbrandkiticon) | **POST** /brand-kit/icons | Add a named SVG icon to the Brand Kit
*PartnerApi* | [**postPublicCompositionEmbedStatus**](docs/Api/PartnerApi.md#postpubliccompositionembedstatus) | **POST** /embed/compositions/status | Batch-check whether compositions are currently served for embed
*PartnerApi* | [**publishWorkspaceWorkflow**](docs/Api/PartnerApi.md#publishworkspaceworkflow) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/publish | Publish the Draft of a Workflow
*PartnerApi* | [**putBrandKit**](docs/Api/PartnerApi.md#putbrandkit) | **PUT** /brand-kit | Save Brand Kit tokens
*PartnerApi* | [**readCompositionEntries**](docs/Api/PartnerApi.md#readcompositionentries) | **GET** /compositions/{id}/entries/{table} | Read the Entries of a Composition&#39;s Table
*PartnerApi* | [**removeAiAnswersKnowledgeDocument**](docs/Api/PartnerApi.md#removeaianswersknowledgedocument) | **DELETE** /compositions/{id}/adapters/ai-answers/knowledge/documents/{documentId} | Remove a document from a widget&#39;s knowledge base
*PartnerApi* | [**removePartnerAdapterConnection**](docs/Api/PartnerApi.md#removepartneradapterconnection) | **DELETE** /partners/{partnerId}/adapter-connections/{adapterId}/{credentialKey} | Remove an adapter key from a partner
*PartnerApi* | [**removePartnerDataDatabase**](docs/Api/PartnerApi.md#removepartnerdatadatabase) | **DELETE** /partners/{partnerId}/data-database | Stop keeping the data of a partner&#39;s compositions in its own database
*PartnerApi* | [**removePartnerPreset**](docs/Api/PartnerApi.md#removepartnerpreset) | **DELETE** /partners/{partnerId}/presets/{key} | Take a widget off the partner&#39;s presets
*PartnerApi* | [**removePartnerStorageDestination**](docs/Api/PartnerApi.md#removepartnerstoragedestination) | **DELETE** /partners/{partnerId}/storage | Stop storing a partner&#39;s uploaded files in its own bucket
*PartnerApi* | [**removePartnerWorkflowPreset**](docs/Api/PartnerApi.md#removepartnerworkflowpreset) | **DELETE** /partners/{partnerId}/workflow-presets/{key} | Stop offering a workflow as a place to start
*PartnerApi* | [**removeUserAdapterConnection**](docs/Api/PartnerApi.md#removeuseradapterconnection) | **DELETE** /users/{userId}/adapter-connections/{adapterId}/{credentialKey} | Remove an adapter key from an account
*PartnerApi* | [**replayPartnerNotificationDelivery**](docs/Api/PartnerApi.md#replaypartnernotificationdelivery) | **POST** /partners/{partnerId}/notifications/deliveries/{deliveryId}/replay | Send a webhook delivery again
*PartnerApi* | [**reportPublicWorkflowEvents**](docs/Api/PartnerApi.md#reportpublicworkflowevents) | **POST** /embed/workflows/{workflowId}/events | Report what visitors did in a Workflow, as counts
*PartnerApi* | [**restoreWorkspaceWorkflowVersion**](docs/Api/PartnerApi.md#restoreworkspaceworkflowversion) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/versions/{versionId}/restore | Restore a Version of a Workflow into the Draft
*PartnerApi* | [**resumeWorkspaceWorkflow**](docs/Api/PartnerApi.md#resumeworkspaceworkflow) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/resume | Resume a Paused Workflow
*PartnerApi* | [**revokeManagedUserEditorSession**](docs/Api/PartnerApi.md#revokemanagedusereditorsession) | **DELETE** /managed-users/{id}/editor-sessions/{sessionId} | End one editor session of a managed user
*PartnerApi* | [**revokeManagedUserEditorSessions**](docs/Api/PartnerApi.md#revokemanagedusereditorsessions) | **DELETE** /managed-users/{id}/editor-sessions | End every editor session of a managed user
*PartnerApi* | [**rotatePartnerEntryContextSecret**](docs/Api/PartnerApi.md#rotatepartnerentrycontextsecret) | **POST** /partners/{partnerId}/entry-context-signing/secret | Make a secret to sign the context of your embeds
*PartnerApi* | [**rotatePartnerWebhookSecret**](docs/Api/PartnerApi.md#rotatepartnerwebhooksecret) | **POST** /partners/{partnerId}/notifications/webhook-secret | Make a new secret for your webhook
*PartnerApi* | [**saveWorkspaceWorkflow**](docs/Api/PartnerApi.md#saveworkspaceworkflow) | **PUT** /workspaces/{workspaceId}/workflows/{workflowId} | Save the Draft of a Workflow
*PartnerApi* | [**sendPartnerNotificationTestEvent**](docs/Api/PartnerApi.md#sendpartnernotificationtestevent) | **POST** /partners/{partnerId}/notifications/test-event | Send a test event to your webhook
*PartnerApi* | [**setCompositionDataSource**](docs/Api/PartnerApi.md#setcompositiondatasource) | **PUT** /compositions/{id}/data-source | Bind a public JSON data source for embed refresh
*PartnerApi* | [**setDynamicContent**](docs/Api/PartnerApi.md#setdynamiccontent) | **PUT** /compositions/{id}/content | Set Dynamic Content
*PartnerApi* | [**setManagedUserDesignDefaults**](docs/Api/PartnerApi.md#setmanageduserdesigndefaults) | **PUT** /managed-users/{id}/design-defaults | Set or clear design defaults for one managed user
*PartnerApi* | [**setManagedUserLimits**](docs/Api/PartnerApi.md#setmanageduserlimits) | **PUT** /managed-users/{id}/limits | Set or clear the monthly credit cap for one managed user
*PartnerApi* | [**setPartnerAdapterConnection**](docs/Api/PartnerApi.md#setpartneradapterconnection) | **PUT** /partners/{partnerId}/adapter-connections/{adapterId}/{credentialKey} | Connect an adapter key to a partner
*PartnerApi* | [**setPartnerDataDatabase**](docs/Api/PartnerApi.md#setpartnerdatadatabase) | **PUT** /partners/{partnerId}/data-database | Keep the data of a partner&#39;s compositions in a Neon database of its own
*PartnerApi* | [**setPartnerDesignDefaults**](docs/Api/PartnerApi.md#setpartnerdesigndefaults) | **PUT** /partners/{partnerId}/design-defaults | Set or clear partner-wide design defaults
*PartnerApi* | [**setPartnerPreset**](docs/Api/PartnerApi.md#setpartnerpreset) | **PUT** /partners/{partnerId}/presets/{key} | Make a widget a preset, or replace a preset
*PartnerApi* | [**setPartnerStorageDestination**](docs/Api/PartnerApi.md#setpartnerstoragedestination) | **PUT** /partners/{partnerId}/storage | Set where a partner&#39;s uploaded files are stored
*PartnerApi* | [**setPartnerWorkflowPreset**](docs/Api/PartnerApi.md#setpartnerworkflowpreset) | **PUT** /partners/{partnerId}/workflow-presets/{key} | Offer a workflow as a place to start, or replace what a key offers
*PartnerApi* | [**setUserAdapterConnection**](docs/Api/PartnerApi.md#setuseradapterconnection) | **PUT** /users/{userId}/adapter-connections/{adapterId}/{credentialKey} | Connect an adapter key to an account
*PartnerApi* | [**unarchiveWorkspaceWorkflow**](docs/Api/PartnerApi.md#unarchiveworkspaceworkflow) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/unarchive | Unarchive a Workflow
*PartnerApi* | [**updateCanvas**](docs/Api/PartnerApi.md#updatecanvas) | **PUT** /canvases/{id} | Update Canvas
*PartnerApi* | [**updateComposition**](docs/Api/PartnerApi.md#updatecomposition) | **PUT** /compositions/{id} | Update Composition
*PartnerApi* | [**updateCompositionDatabaseRecord**](docs/Api/PartnerApi.md#updatecompositiondatabaserecord) | **PUT** /compositions/{id}/database/{table}/{recordId} | Update Record In Composition Database
*PartnerApi* | [**updateCompositionStatus**](docs/Api/PartnerApi.md#updatecompositionstatus) | **PUT** /compositions/{id}/status | Update Composition Status
*PartnerApi* | [**updateManagedUser**](docs/Api/PartnerApi.md#updatemanageduser) | **PUT** /managed-users/{id} | Update Managed User
*PartnerApi* | [**updatePartnerEntryContextSigning**](docs/Api/PartnerApi.md#updatepartnerentrycontextsigning) | **PUT** /partners/{partnerId}/entry-context-signing | Require a signed context, or stop requiring it
*PartnerApi* | [**updatePartnerNotificationSettings**](docs/Api/PartnerApi.md#updatepartnernotificationsettings) | **PUT** /partners/{partnerId}/notifications/settings | Choose where your notifications go
*PartnerApi* | [**updatePersonalWorkspaceDomain**](docs/Api/PartnerApi.md#updatepersonalworkspacedomain) | **PUT** /users/{id}/workspace/domains/{domainId} | Change a website on your list
*PartnerApi* | [**updateUserApiKey**](docs/Api/PartnerApi.md#updateuserapikey) | **PUT** /users/{id}/keys/{keyId} | Rename an API key, or switch it off or on
*PartnerApi* | [**uploadPublicCompositionAdapterFile**](docs/Api/PartnerApi.md#uploadpubliccompositionadapterfile) | **PUT** /embed/compositions/{compositionId}/adapters/upload/files/{ticket} | Send the file a visitor chose through the upload adapter of a published widget
*PartnerApi* | [**uploadsGet**](docs/Api/PartnerApi.md#uploadsget) | **GET** /uploads | List the account&#39;s uploads
*PartnerApi* | [**uploadsIdDelete**](docs/Api/PartnerApi.md#uploadsiddelete) | **DELETE** /uploads/{id} | Delete an upload
*PartnerApi* | [**uploadsIdGet**](docs/Api/PartnerApi.md#uploadsidget) | **GET** /uploads/{id} | Get an upload by id
*PartnerApi* | [**uploadsLimitsGet**](docs/Api/PartnerApi.md#uploadslimitsget) | **GET** /uploads/limits | Upload size limits and accepted file types
*PartnerApi* | [**uploadsPost**](docs/Api/PartnerApi.md#uploadspost) | **POST** /uploads | Upload a file
*PartnerApi* | [**validateCompositionContent**](docs/Api/PartnerApi.md#validatecompositioncontent) | **POST** /compositions/{id}/content/validate | Validate Content
*PartnerApi* | [**validateToken**](docs/Api/PartnerApi.md#validatetoken) | **GET** /tokens/validate | Validate current authentication token
*PartnerApi* | [**verifyPartnerDataDatabase**](docs/Api/PartnerApi.md#verifypartnerdatadatabase) | **POST** /partners/{partnerId}/data-database/verify | Check that a partner&#39;s own database still works
*PartnerApi* | [**verifyPartnerStorageDestination**](docs/Api/PartnerApi.md#verifypartnerstoragedestination) | **POST** /partners/{partnerId}/storage/verify | Check that a partner&#39;s storage destination still works
*PartnersApi* | [**confirmPartnerAdapterConnection_0**](docs/Api/PartnersApi.md#confirmpartneradapterconnection_0) | **POST** /partners/{partnerId}/adapter-connections/{adapterId}/{credentialKey}/confirm | Confirm a partner&#39;s adapter address with the code that was emailed to it
*PartnersApi* | [**createPartnerExtraCreditsInvoice_0**](docs/Api/PartnersApi.md#createpartnerextracreditsinvoice_0) | **POST** /partners/{partnerId}/credits/extra-invoice | Buy extra credits for a partner
*PartnersApi* | [**getMyPartners_0**](docs/Api/PartnersApi.md#getmypartners_0) | **GET** /partners/mine | Find the partner you administer
*PartnersApi* | [**getPartnerAdapterConnections_0**](docs/Api/PartnersApi.md#getpartneradapterconnections_0) | **GET** /partners/{partnerId}/adapter-connections | See which adapter keys a partner has connected
*PartnersApi* | [**getPartnerAnalyticsByManagedUser_0**](docs/Api/PartnersApi.md#getpartneranalyticsbymanageduser_0) | **GET** /partners/{partnerId}/analytics/managed-users | What each managed user&#39;s widgets did
*PartnersApi* | [**getPartnerAnalyticsSummary_0**](docs/Api/PartnersApi.md#getpartneranalyticssummary_0) | **GET** /partners/{partnerId}/analytics/summary | What was done with a partner&#39;s published widgets
*PartnersApi* | [**getPartnerAnalyticsTimeline_0**](docs/Api/PartnersApi.md#getpartneranalyticstimeline_0) | **GET** /partners/{partnerId}/analytics/timeline | What was done with a partner&#39;s widgets, day by day
*PartnersApi* | [**getPartnerAnalyticsTopWidgets_0**](docs/Api/PartnersApi.md#getpartneranalyticstopwidgets_0) | **GET** /partners/{partnerId}/analytics/top-widgets | Which widgets were viewed the most
*PartnersApi* | [**getPartnerBillingOverview_0**](docs/Api/PartnersApi.md#getpartnerbillingoverview_0) | **GET** /partners/{partnerId}/billing-overview | Get comprehensive partner billing overview
*PartnersApi* | [**getPartnerContract_0**](docs/Api/PartnersApi.md#getpartnercontract_0) | **GET** /partners/{partnerId}/contract | Get a partner&#39;s contract
*PartnersApi* | [**getPartnerCreditBalance_0**](docs/Api/PartnersApi.md#getpartnercreditbalance_0) | **GET** /partners/{partnerId}/credits/balance | Get partner credit balance
*PartnersApi* | [**getPartnerCreditTransactions_0**](docs/Api/PartnersApi.md#getpartnercredittransactions_0) | **GET** /partners/{partnerId}/credits/transactions | Get partner credit transaction history
*PartnersApi* | [**getPartnerDataDatabase_0**](docs/Api/PartnersApi.md#getpartnerdatadatabase_0) | **GET** /partners/{partnerId}/data-database | See the Neon database a partner keeps the data of its compositions in
*PartnersApi* | [**getPartnerDesignDefaults_0**](docs/Api/PartnersApi.md#getpartnerdesigndefaults_0) | **GET** /partners/{partnerId}/design-defaults | Read partner-wide design defaults
*PartnersApi* | [**getPartnerEntryContextSigning_0**](docs/Api/PartnersApi.md#getpartnerentrycontextsigning_0) | **GET** /partners/{partnerId}/entry-context-signing | See how the context of your embeds is signed
*PartnersApi* | [**getPartnerNotificationSettings_0**](docs/Api/PartnersApi.md#getpartnernotificationsettings_0) | **GET** /partners/{partnerId}/notifications/settings | Where your notifications go
*PartnersApi* | [**getPartnerStorageDestination_0**](docs/Api/PartnersApi.md#getpartnerstoragedestination_0) | **GET** /partners/{partnerId}/storage | Get where a partner&#39;s uploaded files are stored
*PartnersApi* | [**getPartnerStorageUsage_0**](docs/Api/PartnersApi.md#getpartnerstorageusage_0) | **GET** /partners/{partnerId}/storage/usage | What a partner&#39;s customers store
*PartnersApi* | [**listPartnerNotificationDeliveries_0**](docs/Api/PartnersApi.md#listpartnernotificationdeliveries_0) | **GET** /partners/{partnerId}/notifications/deliveries | How your notifications reached you
*PartnersApi* | [**listPartnerNotifications_0**](docs/Api/PartnersApi.md#listpartnernotifications_0) | **GET** /partners/{partnerId}/notifications | What your partner account was told
*PartnersApi* | [**listPartnerPresets_0**](docs/Api/PartnersApi.md#listpartnerpresets_0) | **GET** /partners/{partnerId}/presets | List the widgets a partner offers as presets
*PartnersApi* | [**listPartnerWorkflowPresets_0**](docs/Api/PartnersApi.md#listpartnerworkflowpresets_0) | **GET** /partners/{partnerId}/workflow-presets | List the workflows a partner offers as places to start
*PartnersApi* | [**removePartnerAdapterConnection_0**](docs/Api/PartnersApi.md#removepartneradapterconnection_0) | **DELETE** /partners/{partnerId}/adapter-connections/{adapterId}/{credentialKey} | Remove an adapter key from a partner
*PartnersApi* | [**removePartnerDataDatabase_0**](docs/Api/PartnersApi.md#removepartnerdatadatabase_0) | **DELETE** /partners/{partnerId}/data-database | Stop keeping the data of a partner&#39;s compositions in its own database
*PartnersApi* | [**removePartnerPreset_0**](docs/Api/PartnersApi.md#removepartnerpreset_0) | **DELETE** /partners/{partnerId}/presets/{key} | Take a widget off the partner&#39;s presets
*PartnersApi* | [**removePartnerStorageDestination_0**](docs/Api/PartnersApi.md#removepartnerstoragedestination_0) | **DELETE** /partners/{partnerId}/storage | Stop storing a partner&#39;s uploaded files in its own bucket
*PartnersApi* | [**removePartnerWorkflowPreset_0**](docs/Api/PartnersApi.md#removepartnerworkflowpreset_0) | **DELETE** /partners/{partnerId}/workflow-presets/{key} | Stop offering a workflow as a place to start
*PartnersApi* | [**replayPartnerNotificationDelivery_0**](docs/Api/PartnersApi.md#replaypartnernotificationdelivery_0) | **POST** /partners/{partnerId}/notifications/deliveries/{deliveryId}/replay | Send a webhook delivery again
*PartnersApi* | [**rotatePartnerEntryContextSecret_0**](docs/Api/PartnersApi.md#rotatepartnerentrycontextsecret_0) | **POST** /partners/{partnerId}/entry-context-signing/secret | Make a secret to sign the context of your embeds
*PartnersApi* | [**rotatePartnerWebhookSecret_0**](docs/Api/PartnersApi.md#rotatepartnerwebhooksecret_0) | **POST** /partners/{partnerId}/notifications/webhook-secret | Make a new secret for your webhook
*PartnersApi* | [**sendPartnerNotificationTestEvent_0**](docs/Api/PartnersApi.md#sendpartnernotificationtestevent_0) | **POST** /partners/{partnerId}/notifications/test-event | Send a test event to your webhook
*PartnersApi* | [**setPartnerAdapterConnection_0**](docs/Api/PartnersApi.md#setpartneradapterconnection_0) | **PUT** /partners/{partnerId}/adapter-connections/{adapterId}/{credentialKey} | Connect an adapter key to a partner
*PartnersApi* | [**setPartnerDataDatabase_0**](docs/Api/PartnersApi.md#setpartnerdatadatabase_0) | **PUT** /partners/{partnerId}/data-database | Keep the data of a partner&#39;s compositions in a Neon database of its own
*PartnersApi* | [**setPartnerDesignDefaults_0**](docs/Api/PartnersApi.md#setpartnerdesigndefaults_0) | **PUT** /partners/{partnerId}/design-defaults | Set or clear partner-wide design defaults
*PartnersApi* | [**setPartnerPreset_0**](docs/Api/PartnersApi.md#setpartnerpreset_0) | **PUT** /partners/{partnerId}/presets/{key} | Make a widget a preset, or replace a preset
*PartnersApi* | [**setPartnerStorageDestination_0**](docs/Api/PartnersApi.md#setpartnerstoragedestination_0) | **PUT** /partners/{partnerId}/storage | Set where a partner&#39;s uploaded files are stored
*PartnersApi* | [**setPartnerWorkflowPreset_0**](docs/Api/PartnersApi.md#setpartnerworkflowpreset_0) | **PUT** /partners/{partnerId}/workflow-presets/{key} | Offer a workflow as a place to start, or replace what a key offers
*PartnersApi* | [**updatePartnerEntryContextSigning_0**](docs/Api/PartnersApi.md#updatepartnerentrycontextsigning_0) | **PUT** /partners/{partnerId}/entry-context-signing | Require a signed context, or stop requiring it
*PartnersApi* | [**updatePartnerNotificationSettings_0**](docs/Api/PartnersApi.md#updatepartnernotificationsettings_0) | **PUT** /partners/{partnerId}/notifications/settings | Choose where your notifications go
*PartnersApi* | [**verifyPartnerDataDatabase_0**](docs/Api/PartnersApi.md#verifypartnerdatadatabase_0) | **POST** /partners/{partnerId}/data-database/verify | Check that a partner&#39;s own database still works
*PartnersApi* | [**verifyPartnerStorageDestination_0**](docs/Api/PartnersApi.md#verifypartnerstoragedestination_0) | **POST** /partners/{partnerId}/storage/verify | Check that a partner&#39;s storage destination still works
*PublicEmbedApi* | [**callPublicCompositionAdapter_0**](docs/Api/PublicEmbedApi.md#callpubliccompositionadapter_0) | **POST** /embed/compositions/{compositionId}/adapters/{adapterId}/{operation} | Call a gateway operation of an adapter a published widget uses
*PublicEmbedApi* | [**createPublicCompositionEntry_0**](docs/Api/PublicEmbedApi.md#createpubliccompositionentry_0) | **POST** /embed/compositions/{compositionId}/entries/{table} | Append a visitor entry through the gateway
*PublicEmbedApi* | [**getPublicCompositionEmbed_0**](docs/Api/PublicEmbedApi.md#getpubliccompositionembed_0) | **GET** /embed/compositions/{compositionId} | Resolve a composition UUID to a published widget URL
*PublicEmbedApi* | [**getPublicCompositionIframe_0**](docs/Api/PublicEmbedApi.md#getpubliccompositioniframe_0) | **GET** /embed/compositions/{compositionId}/frame | Embed a published composition with its saved values
*PublicEmbedApi* | [**getPublicWorkflowFrame_0**](docs/Api/PublicEmbedApi.md#getpublicworkflowframe_0) | **GET** /embed/workflows/{workflowId}/frame | Show a published Workflow in a page of its own
*PublicEmbedApi* | [**getPublicWorkflowVersion_0**](docs/Api/PublicEmbedApi.md#getpublicworkflowversion_0) | **GET** /embed/workflows/{workflowId}/versions/{versionId} | Read one published version of a Workflow
*PublicEmbedApi* | [**getPublicWorkflow_0**](docs/Api/PublicEmbedApi.md#getpublicworkflow_0) | **GET** /embed/workflows/{workflowId} | Read the published Workflow of an embed
*PublicEmbedApi* | [**postPublicCompositionEmbedStatus_0**](docs/Api/PublicEmbedApi.md#postpubliccompositionembedstatus_0) | **POST** /embed/compositions/status | Batch-check whether compositions are currently served for embed
*PublicEmbedApi* | [**reportPublicWorkflowEvents_0**](docs/Api/PublicEmbedApi.md#reportpublicworkflowevents_0) | **POST** /embed/workflows/{workflowId}/events | Report what visitors did in a Workflow, as counts
*PublicEmbedApi* | [**uploadPublicCompositionAdapterFile_0**](docs/Api/PublicEmbedApi.md#uploadpubliccompositionadapterfile_0) | **PUT** /embed/compositions/{compositionId}/adapters/upload/files/{ticket} | Send the file a visitor chose through the upload adapter of a published widget
*TokensApi* | [**validateToken_0**](docs/Api/TokensApi.md#validatetoken_0) | **GET** /tokens/validate | Validate current authentication token
*UploadsApi* | [**uploadsGet_0**](docs/Api/UploadsApi.md#uploadsget_0) | **GET** /uploads | List the account&#39;s uploads
*UploadsApi* | [**uploadsIdDelete_0**](docs/Api/UploadsApi.md#uploadsiddelete_0) | **DELETE** /uploads/{id} | Delete an upload
*UploadsApi* | [**uploadsIdGet_0**](docs/Api/UploadsApi.md#uploadsidget_0) | **GET** /uploads/{id} | Get an upload by id
*UploadsApi* | [**uploadsLimitsGet_0**](docs/Api/UploadsApi.md#uploadslimitsget_0) | **GET** /uploads/limits | Upload size limits and accepted file types
*UploadsApi* | [**uploadsPost_0**](docs/Api/UploadsApi.md#uploadspost_0) | **POST** /uploads | Upload a file
*UsersApi* | [**addPersonalWorkspaceDomain_0**](docs/Api/UsersApi.md#addpersonalworkspacedomain_0) | **POST** /users/{id}/workspace/domains | Allow a website to show your widgets
*UsersApi* | [**confirmUserAdapterConnection_0**](docs/Api/UsersApi.md#confirmuseradapterconnection_0) | **POST** /users/{userId}/adapter-connections/{adapterId}/{credentialKey}/confirm | Confirm an adapter address with the code that was emailed to it
*UsersApi* | [**createUserApiKey_0**](docs/Api/UsersApi.md#createuserapikey_0) | **POST** /users/{id}/keys | Create an API key
*UsersApi* | [**deletePersonalWorkspaceDomain_0**](docs/Api/UsersApi.md#deletepersonalworkspacedomain_0) | **DELETE** /users/{id}/workspace/domains/{domainId} | Stop allowing a website to show your widgets
*UsersApi* | [**deleteUserApiKey_0**](docs/Api/UsersApi.md#deleteuserapikey_0) | **DELETE** /users/{id}/keys/{keyId} | Delete an API key
*UsersApi* | [**getPersonalWorkspaceDomains_0**](docs/Api/UsersApi.md#getpersonalworkspacedomains_0) | **GET** /users/{id}/workspace/domains | List the websites allowed to show your widgets
*UsersApi* | [**getUserAdapterConnections_0**](docs/Api/UsersApi.md#getuseradapterconnections_0) | **GET** /users/{userId}/adapter-connections | See which adapter keys an account has connected
*UsersApi* | [**getUserApiKeyUsageLogs_0**](docs/Api/UsersApi.md#getuserapikeyusagelogs_0) | **GET** /users/{id}/api-keys/{keyId}/logs | Read what an API key was used for
*UsersApi* | [**getUserApiKeys_0**](docs/Api/UsersApi.md#getuserapikeys_0) | **GET** /users/{id}/keys | List the API keys of an account
*UsersApi* | [**removeUserAdapterConnection_0**](docs/Api/UsersApi.md#removeuseradapterconnection_0) | **DELETE** /users/{userId}/adapter-connections/{adapterId}/{credentialKey} | Remove an adapter key from an account
*UsersApi* | [**setUserAdapterConnection_0**](docs/Api/UsersApi.md#setuseradapterconnection_0) | **PUT** /users/{userId}/adapter-connections/{adapterId}/{credentialKey} | Connect an adapter key to an account
*UsersApi* | [**updatePersonalWorkspaceDomain_0**](docs/Api/UsersApi.md#updatepersonalworkspacedomain_0) | **PUT** /users/{id}/workspace/domains/{domainId} | Change a website on your list
*UsersApi* | [**updateUserApiKey_0**](docs/Api/UsersApi.md#updateuserapikey_0) | **PUT** /users/{id}/keys/{keyId} | Rename an API key, or switch it off or on
*WidgetsApi* | [**createCompositionFromWidget_0**](docs/Api/WidgetsApi.md#createcompositionfromwidget_0) | **POST** /widgets/{id}/composition | Create a composition for a widget in one call
*WidgetsApi* | [**createWidget_0**](docs/Api/WidgetsApi.md#createwidget_0) | **POST** /widgets | Create Widget
*WidgetsApi* | [**getWidgetsBatch_0**](docs/Api/WidgetsApi.md#getwidgetsbatch_0) | **POST** /widgets/batch | Get Widgets Batch
*WidgetsApi* | [**getWidgets_0**](docs/Api/WidgetsApi.md#getwidgets_0) | **GET** /widgets | List Widgets
*WorkflowsApi* | [**archiveWorkspaceWorkflow_0**](docs/Api/WorkflowsApi.md#archiveworkspaceworkflow_0) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/archive | Archive a Workflow
*WorkflowsApi* | [**createWorkspaceWorkflowFromPreset_0**](docs/Api/WorkflowsApi.md#createworkspaceworkflowfrompreset_0) | **POST** /workspaces/{workspaceId}/workflows/from-preset | Start a Workflow from a starting point
*WorkflowsApi* | [**createWorkspaceWorkflow_0**](docs/Api/WorkflowsApi.md#createworkspaceworkflow_0) | **POST** /workspaces/{workspaceId}/workflows | Create a Workflow
*WorkflowsApi* | [**deleteWorkspaceWorkflow_0**](docs/Api/WorkflowsApi.md#deleteworkspaceworkflow_0) | **DELETE** /workspaces/{workspaceId}/workflows/{workflowId} | Delete a Workflow
*WorkflowsApi* | [**discardWorkspaceWorkflowChanges_0**](docs/Api/WorkflowsApi.md#discardworkspaceworkflowchanges_0) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/discard | Discard the Unpublished Changes of a Workflow
*WorkflowsApi* | [**duplicateWorkspaceWorkflow_0**](docs/Api/WorkflowsApi.md#duplicateworkspaceworkflow_0) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/duplicate | Duplicate a Workflow
*WorkflowsApi* | [**getWorkspaceWorkflowStats_0**](docs/Api/WorkflowsApi.md#getworkspaceworkflowstats_0) | **GET** /workspaces/{workspaceId}/workflows/{workflowId}/stats | Get what Visitors Did in a Workflow
*WorkflowsApi* | [**getWorkspaceWorkflowVersion_0**](docs/Api/WorkflowsApi.md#getworkspaceworkflowversion_0) | **GET** /workspaces/{workspaceId}/workflows/{workflowId}/versions/{versionId} | Get a Published Version of a Workflow
*WorkflowsApi* | [**getWorkspaceWorkflow_0**](docs/Api/WorkflowsApi.md#getworkspaceworkflow_0) | **GET** /workspaces/{workspaceId}/workflows/{workflowId} | Get a Workflow
*WorkflowsApi* | [**listPartnerWorkflowPresets_1**](docs/Api/WorkflowsApi.md#listpartnerworkflowpresets_1) | **GET** /partners/{partnerId}/workflow-presets | List the workflows a partner offers as places to start
*WorkflowsApi* | [**listWorkspaceWorkflowCompositionOptions_0**](docs/Api/WorkflowsApi.md#listworkspaceworkflowcompositionoptions_0) | **GET** /workspaces/{workspaceId}/workflows/composition-options | List the compositions a workflow can show, and what each can do
*WorkflowsApi* | [**listWorkspaceWorkflowPresets_0**](docs/Api/WorkflowsApi.md#listworkspaceworkflowpresets_0) | **GET** /workspaces/{workspaceId}/workflows/presets | List the starting points for a new Workflow
*WorkflowsApi* | [**listWorkspaceWorkflowVersions_0**](docs/Api/WorkflowsApi.md#listworkspaceworkflowversions_0) | **GET** /workspaces/{workspaceId}/workflows/{workflowId}/versions | List the Published Versions of a Workflow
*WorkflowsApi* | [**listWorkspaceWorkflows_0**](docs/Api/WorkflowsApi.md#listworkspaceworkflows_0) | **GET** /workspaces/{workspaceId}/workflows | List the Workflows of a Workspace
*WorkflowsApi* | [**pauseWorkspaceWorkflow_0**](docs/Api/WorkflowsApi.md#pauseworkspaceworkflow_0) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/pause | Pause a Workflow
*WorkflowsApi* | [**publishWorkspaceWorkflow_0**](docs/Api/WorkflowsApi.md#publishworkspaceworkflow_0) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/publish | Publish the Draft of a Workflow
*WorkflowsApi* | [**removePartnerWorkflowPreset_1**](docs/Api/WorkflowsApi.md#removepartnerworkflowpreset_1) | **DELETE** /partners/{partnerId}/workflow-presets/{key} | Stop offering a workflow as a place to start
*WorkflowsApi* | [**restoreWorkspaceWorkflowVersion_0**](docs/Api/WorkflowsApi.md#restoreworkspaceworkflowversion_0) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/versions/{versionId}/restore | Restore a Version of a Workflow into the Draft
*WorkflowsApi* | [**resumeWorkspaceWorkflow_0**](docs/Api/WorkflowsApi.md#resumeworkspaceworkflow_0) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/resume | Resume a Paused Workflow
*WorkflowsApi* | [**saveWorkspaceWorkflow_0**](docs/Api/WorkflowsApi.md#saveworkspaceworkflow_0) | **PUT** /workspaces/{workspaceId}/workflows/{workflowId} | Save the Draft of a Workflow
*WorkflowsApi* | [**setPartnerWorkflowPreset_1**](docs/Api/WorkflowsApi.md#setpartnerworkflowpreset_1) | **PUT** /partners/{partnerId}/workflow-presets/{key} | Offer a workflow as a place to start, or replace what a key offers
*WorkflowsApi* | [**unarchiveWorkspaceWorkflow_0**](docs/Api/WorkflowsApi.md#unarchiveworkspaceworkflow_0) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/unarchive | Unarchive a Workflow
*WorkspacesApi* | [**archiveWorkspaceWorkflow_1**](docs/Api/WorkspacesApi.md#archiveworkspaceworkflow_1) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/archive | Archive a Workflow
*WorkspacesApi* | [**createWorkspaceWorkflowFromPreset_1**](docs/Api/WorkspacesApi.md#createworkspaceworkflowfrompreset_1) | **POST** /workspaces/{workspaceId}/workflows/from-preset | Start a Workflow from a starting point
*WorkspacesApi* | [**createWorkspaceWorkflow_1**](docs/Api/WorkspacesApi.md#createworkspaceworkflow_1) | **POST** /workspaces/{workspaceId}/workflows | Create a Workflow
*WorkspacesApi* | [**deleteWorkspaceWorkflow_1**](docs/Api/WorkspacesApi.md#deleteworkspaceworkflow_1) | **DELETE** /workspaces/{workspaceId}/workflows/{workflowId} | Delete a Workflow
*WorkspacesApi* | [**discardWorkspaceWorkflowChanges_1**](docs/Api/WorkspacesApi.md#discardworkspaceworkflowchanges_1) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/discard | Discard the Unpublished Changes of a Workflow
*WorkspacesApi* | [**duplicateWorkspaceWorkflow_1**](docs/Api/WorkspacesApi.md#duplicateworkspaceworkflow_1) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/duplicate | Duplicate a Workflow
*WorkspacesApi* | [**getWorkspaceWorkflowStats_1**](docs/Api/WorkspacesApi.md#getworkspaceworkflowstats_1) | **GET** /workspaces/{workspaceId}/workflows/{workflowId}/stats | Get what Visitors Did in a Workflow
*WorkspacesApi* | [**getWorkspaceWorkflowVersion_1**](docs/Api/WorkspacesApi.md#getworkspaceworkflowversion_1) | **GET** /workspaces/{workspaceId}/workflows/{workflowId}/versions/{versionId} | Get a Published Version of a Workflow
*WorkspacesApi* | [**getWorkspaceWorkflow_1**](docs/Api/WorkspacesApi.md#getworkspaceworkflow_1) | **GET** /workspaces/{workspaceId}/workflows/{workflowId} | Get a Workflow
*WorkspacesApi* | [**listWorkspaceWorkflowCompositionOptions_1**](docs/Api/WorkspacesApi.md#listworkspaceworkflowcompositionoptions_1) | **GET** /workspaces/{workspaceId}/workflows/composition-options | List the compositions a workflow can show, and what each can do
*WorkspacesApi* | [**listWorkspaceWorkflowPresets_1**](docs/Api/WorkspacesApi.md#listworkspaceworkflowpresets_1) | **GET** /workspaces/{workspaceId}/workflows/presets | List the starting points for a new Workflow
*WorkspacesApi* | [**listWorkspaceWorkflowVersions_1**](docs/Api/WorkspacesApi.md#listworkspaceworkflowversions_1) | **GET** /workspaces/{workspaceId}/workflows/{workflowId}/versions | List the Published Versions of a Workflow
*WorkspacesApi* | [**listWorkspaceWorkflows_1**](docs/Api/WorkspacesApi.md#listworkspaceworkflows_1) | **GET** /workspaces/{workspaceId}/workflows | List the Workflows of a Workspace
*WorkspacesApi* | [**pauseWorkspaceWorkflow_1**](docs/Api/WorkspacesApi.md#pauseworkspaceworkflow_1) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/pause | Pause a Workflow
*WorkspacesApi* | [**publishWorkspaceWorkflow_1**](docs/Api/WorkspacesApi.md#publishworkspaceworkflow_1) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/publish | Publish the Draft of a Workflow
*WorkspacesApi* | [**restoreWorkspaceWorkflowVersion_1**](docs/Api/WorkspacesApi.md#restoreworkspaceworkflowversion_1) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/versions/{versionId}/restore | Restore a Version of a Workflow into the Draft
*WorkspacesApi* | [**resumeWorkspaceWorkflow_1**](docs/Api/WorkspacesApi.md#resumeworkspaceworkflow_1) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/resume | Resume a Paused Workflow
*WorkspacesApi* | [**saveWorkspaceWorkflow_1**](docs/Api/WorkspacesApi.md#saveworkspaceworkflow_1) | **PUT** /workspaces/{workspaceId}/workflows/{workflowId} | Save the Draft of a Workflow
*WorkspacesApi* | [**unarchiveWorkspaceWorkflow_1**](docs/Api/WorkspacesApi.md#unarchiveworkspaceworkflow_1) | **POST** /workspaces/{workspaceId}/workflows/{workflowId}/unarchive | Unarchive a Workflow

## Models

- [AccountCreditBalance](docs/Model/AccountCreditBalance.md)
- [AccountCreditBalanceResponse](docs/Model/AccountCreditBalanceResponse.md)
- [AccountCreditTransaction](docs/Model/AccountCreditTransaction.md)
- [AdapterConnection](docs/Model/AdapterConnection.md)
- [AdapterConnectionRemoval](docs/Model/AdapterConnectionRemoval.md)
- [AddAiAnswersKnowledgeDocument201Response](docs/Model/AddAiAnswersKnowledgeDocument201Response.md)
- [AddAiAnswersKnowledgeDocumentRequest](docs/Model/AddAiAnswersKnowledgeDocumentRequest.md)
- [AddDomainRequest](docs/Model/AddDomainRequest.md)
- [AiAnswersKnowledge](docs/Model/AiAnswersKnowledge.md)
- [AiAnswersKnowledgeDocument](docs/Model/AiAnswersKnowledgeDocument.md)
- [AiAnswersKnowledgeRemoval](docs/Model/AiAnswersKnowledgeRemoval.md)
- [AiAnswersKnowledgeTotals](docs/Model/AiAnswersKnowledgeTotals.md)
- [ApiKeyScope](docs/Model/ApiKeyScope.md)
- [BrandColor](docs/Model/BrandColor.md)
- [BrandFont](docs/Model/BrandFont.md)
- [BrandKitAssetView](docs/Model/BrandKitAssetView.md)
- [BrandKitFigmaSource](docs/Model/BrandKitFigmaSource.md)
- [BrandKitTokens](docs/Model/BrandKitTokens.md)
- [BrandKitTokensFonts](docs/Model/BrandKitTokensFonts.md)
- [BrandKitView](docs/Model/BrandKitView.md)
- [BrandKitViewOwner](docs/Model/BrandKitViewOwner.md)
- [BrandKitViewResponse](docs/Model/BrandKitViewResponse.md)
- [BrandSpacing](docs/Model/BrandSpacing.md)
- [Canvas](docs/Model/Canvas.md)
- [CanvasResponse](docs/Model/CanvasResponse.md)
- [CheckCompositionAccessResponse](docs/Model/CheckCompositionAccessResponse.md)
- [CheckCompositionAccessResponseData](docs/Model/CheckCompositionAccessResponseData.md)
- [Composition](docs/Model/Composition.md)
- [CompositionDataSource](docs/Model/CompositionDataSource.md)
- [CompositionDataSourceResponse](docs/Model/CompositionDataSourceResponse.md)
- [CompositionEntriesDescription](docs/Model/CompositionEntriesDescription.md)
- [CompositionEntriesDescriptionResponse](docs/Model/CompositionEntriesDescriptionResponse.md)
- [CompositionEntriesReading](docs/Model/CompositionEntriesReading.md)
- [CompositionEntriesReadingResponse](docs/Model/CompositionEntriesReadingResponse.md)
- [CompositionEntryAggregateTally](docs/Model/CompositionEntryAggregateTally.md)
- [CompositionEntryAggregatesBlock](docs/Model/CompositionEntryAggregatesBlock.md)
- [CompositionEntryColumn](docs/Model/CompositionEntryColumn.md)
- [CompositionEntryDeleteSuccess](docs/Model/CompositionEntryDeleteSuccess.md)
- [CompositionEntryDeleteSuccessData](docs/Model/CompositionEntryDeleteSuccessData.md)
- [CompositionEntryItem](docs/Model/CompositionEntryItem.md)
- [CompositionEntryItemsMeta](docs/Model/CompositionEntryItemsMeta.md)
- [CompositionEntryItemsPageSuccess](docs/Model/CompositionEntryItemsPageSuccess.md)
- [CompositionEntryTable](docs/Model/CompositionEntryTable.md)
- [CompositionEntryTally](docs/Model/CompositionEntryTally.md)
- [CompositionLastEditedBy](docs/Model/CompositionLastEditedBy.md)
- [CompositionResponse](docs/Model/CompositionResponse.md)
- [CompositionVersion](docs/Model/CompositionVersion.md)
- [ConfirmAdapterConnectionRequest](docs/Model/ConfirmAdapterConnectionRequest.md)
- [ContentCheckFinding](docs/Model/ContentCheckFinding.md)
- [ContentItemWriteResult](docs/Model/ContentItemWriteResult.md)
- [ContentItemWriteResultValidationResult](docs/Model/ContentItemWriteResultValidationResult.md)
- [CopyPartnerPresetRequest](docs/Model/CopyPartnerPresetRequest.md)
- [CreateCanvasRequest](docs/Model/CreateCanvasRequest.md)
- [CreateCompositionContentItem201Response](docs/Model/CreateCompositionContentItem201Response.md)
- [CreateCompositionContentItemRequest](docs/Model/CreateCompositionContentItemRequest.md)
- [CreateCompositionDatabaseRecord201Response](docs/Model/CreateCompositionDatabaseRecord201Response.md)
- [CreateCompositionFromPresetRequest](docs/Model/CreateCompositionFromPresetRequest.md)
- [CreateCompositionFromWidget201Response](docs/Model/CreateCompositionFromWidget201Response.md)
- [CreateCompositionFromWidgetRequest](docs/Model/CreateCompositionFromWidgetRequest.md)
- [CreateUserApiKeyRequest](docs/Model/CreateUserApiKeyRequest.md)
- [CreateWidget201Response](docs/Model/CreateWidget201Response.md)
- [CreateWidget201ResponseData](docs/Model/CreateWidget201ResponseData.md)
- [CreateWorkspaceWorkflowFromPreset201Response](docs/Model/CreateWorkspaceWorkflowFromPreset201Response.md)
- [CreateWorkspaceWorkflowFromPresetRequest](docs/Model/CreateWorkspaceWorkflowFromPresetRequest.md)
- [CreateWorkspaceWorkflowRequest](docs/Model/CreateWorkspaceWorkflowRequest.md)
- [CreatedUserApiKey](docs/Model/CreatedUserApiKey.md)
- [CreatedUserApiKeyResponse](docs/Model/CreatedUserApiKeyResponse.md)
- [DeleteCompositionContentItemResponse](docs/Model/DeleteCompositionContentItemResponse.md)
- [DeleteCompositionContentItemResponseData](docs/Model/DeleteCompositionContentItemResponseData.md)
- [DeleteCompositionDataSourceResponse](docs/Model/DeleteCompositionDataSourceResponse.md)
- [DeleteCompositionDataSourceResponseData](docs/Model/DeleteCompositionDataSourceResponseData.md)
- [DeleteManagedUser200Response](docs/Model/DeleteManagedUser200Response.md)
- [DeletePersonalWorkspaceDomainResponse](docs/Model/DeletePersonalWorkspaceDomainResponse.md)
- [DeletePersonalWorkspaceDomainResponseData](docs/Model/DeletePersonalWorkspaceDomainResponseData.md)
- [DeleteUserApiKeyResponse](docs/Model/DeleteUserApiKeyResponse.md)
- [DeleteUserApiKeyResponseData](docs/Model/DeleteUserApiKeyResponseData.md)
- [DeleteWorkspaceWorkflow200Response](docs/Model/DeleteWorkspaceWorkflow200Response.md)
- [DesignDefaults](docs/Model/DesignDefaults.md)
- [DuplicateComposition202Response](docs/Model/DuplicateComposition202Response.md)
- [DuplicateComposition202ResponseData](docs/Model/DuplicateComposition202ResponseData.md)
- [DuplicateCompositionRequest](docs/Model/DuplicateCompositionRequest.md)
- [EditorSession](docs/Model/EditorSession.md)
- [EditorSessionResponse](docs/Model/EditorSessionResponse.md)
- [Entitlement](docs/Model/Entitlement.md)
- [ErrorDetail](docs/Model/ErrorDetail.md)
- [ErrorResponse](docs/Model/ErrorResponse.md)
- [ExportCompositionEntryItems200Response](docs/Model/ExportCompositionEntryItems200Response.md)
- [ExportCompositionEntryItems200ResponseMeta](docs/Model/ExportCompositionEntryItems200ResponseMeta.md)
- [GetAiAnswersKnowledge200Response](docs/Model/GetAiAnswersKnowledge200Response.md)
- [GetAllCanvasesResponse](docs/Model/GetAllCanvasesResponse.md)
- [GetAllCanvasesResponseData](docs/Model/GetAllCanvasesResponseData.md)
- [GetAllCompositions200Response](docs/Model/GetAllCompositions200Response.md)
- [GetAllManagedUsers200Response](docs/Model/GetAllManagedUsers200Response.md)
- [GetCompositionContentResponse](docs/Model/GetCompositionContentResponse.md)
- [GetCompositionContentSchemaResponse](docs/Model/GetCompositionContentSchemaResponse.md)
- [GetCompositionContentSchemaResponseData](docs/Model/GetCompositionContentSchemaResponseData.md)
- [GetCompositionDataSourceResponse](docs/Model/GetCompositionDataSourceResponse.md)
- [GetCompositionDatabaseRecords200Response](docs/Model/GetCompositionDatabaseRecords200Response.md)
- [GetCompositionDesignResponse](docs/Model/GetCompositionDesignResponse.md)
- [GetCompositionDesignSchemaResponse](docs/Model/GetCompositionDesignSchemaResponse.md)
- [GetCompositionDesignSchemaResponseData](docs/Model/GetCompositionDesignSchemaResponseData.md)
- [GetCompositionEmbedSchemaResponse](docs/Model/GetCompositionEmbedSchemaResponse.md)
- [GetCompositionEmbedSchemaResponseData](docs/Model/GetCompositionEmbedSchemaResponseData.md)
- [GetCompositionEmbedSettingsResponse](docs/Model/GetCompositionEmbedSettingsResponse.md)
- [GetCompositionPreviewResponse](docs/Model/GetCompositionPreviewResponse.md)
- [GetCompositionPreviewResponseData](docs/Model/GetCompositionPreviewResponseData.md)
- [GetCompositionVersions200Response](docs/Model/GetCompositionVersions200Response.md)
- [GetCompositionsBatchRequest](docs/Model/GetCompositionsBatchRequest.md)
- [GetCompositionsBatchResponse](docs/Model/GetCompositionsBatchResponse.md)
- [GetCompositionsBatchResponseData](docs/Model/GetCompositionsBatchResponseData.md)
- [GetInvoicesByPartnerId200Response](docs/Model/GetInvoicesByPartnerId200Response.md)
- [GetManagedUserEntitlementsResponse](docs/Model/GetManagedUserEntitlementsResponse.md)
- [GetManagedUserEntitlementsResponseData](docs/Model/GetManagedUserEntitlementsResponseData.md)
- [GetManagedUserLimits200Response](docs/Model/GetManagedUserLimits200Response.md)
- [GetManagedUserStorageUsage200Response](docs/Model/GetManagedUserStorageUsage200Response.md)
- [GetManagedUserStorageUsage200ResponseData](docs/Model/GetManagedUserStorageUsage200ResponseData.md)
- [GetManagedUserStorageUsage200ResponseDataByPurpose](docs/Model/GetManagedUserStorageUsage200ResponseDataByPurpose.md)
- [GetManagedUsersByManagerIdResponse](docs/Model/GetManagedUsersByManagerIdResponse.md)
- [GetManagedUsersByManagerIdResponseData](docs/Model/GetManagedUsersByManagerIdResponseData.md)
- [GetPartnerBillingOverview200Response](docs/Model/GetPartnerBillingOverview200Response.md)
- [GetPartnerCreditTransactions200Response](docs/Model/GetPartnerCreditTransactions200Response.md)
- [GetPartnerDesignDefaults200Response](docs/Model/GetPartnerDesignDefaults200Response.md)
- [GetPartnerEntitlementsResponse](docs/Model/GetPartnerEntitlementsResponse.md)
- [GetPartnerEntitlementsResponseData](docs/Model/GetPartnerEntitlementsResponseData.md)
- [GetPersonalWorkspaceDomains200Response](docs/Model/GetPersonalWorkspaceDomains200Response.md)
- [GetPublicCompositionEmbed200Response](docs/Model/GetPublicCompositionEmbed200Response.md)
- [GetPublicCompositionEmbed200ResponseAdapters](docs/Model/GetPublicCompositionEmbed200ResponseAdapters.md)
- [GetPublicCompositionEmbed200ResponseAdaptersCaptcha](docs/Model/GetPublicCompositionEmbed200ResponseAdaptersCaptcha.md)
- [GetPublicCompositionEmbed200ResponseDataSource](docs/Model/GetPublicCompositionEmbed200ResponseDataSource.md)
- [GetPublicCompositionEmbed200ResponseDirect](docs/Model/GetPublicCompositionEmbed200ResponseDirect.md)
- [GetPublicCompositionEmbed200ResponseEntries](docs/Model/GetPublicCompositionEmbed200ResponseEntries.md)
- [GetPublicCompositionEmbed200ResponseMedia](docs/Model/GetPublicCompositionEmbed200ResponseMedia.md)
- [GetPublicWorkflow200Response](docs/Model/GetPublicWorkflow200Response.md)
- [GetUserAdapterConnections200Response](docs/Model/GetUserAdapterConnections200Response.md)
- [GetUserApiKeyUsageLogsResponse](docs/Model/GetUserApiKeyUsageLogsResponse.md)
- [GetUserApiKeyUsageLogsResponseData](docs/Model/GetUserApiKeyUsageLogsResponseData.md)
- [GetUserApiKeys200Response](docs/Model/GetUserApiKeys200Response.md)
- [GetWidgets200Response](docs/Model/GetWidgets200Response.md)
- [GetWidgetsBatchRequest](docs/Model/GetWidgetsBatchRequest.md)
- [GetWidgetsBatchResponse](docs/Model/GetWidgetsBatchResponse.md)
- [GetWidgetsBatchResponseData](docs/Model/GetWidgetsBatchResponseData.md)
- [GetWidgetsBatchResponseDataErrorsInner](docs/Model/GetWidgetsBatchResponseDataErrorsInner.md)
- [GetWorkspaceWorkflowStats200Response](docs/Model/GetWorkspaceWorkflowStats200Response.md)
- [GetWorkspaceWorkflowVersion200Response](docs/Model/GetWorkspaceWorkflowVersion200Response.md)
- [ListPartnerPresets200Response](docs/Model/ListPartnerPresets200Response.md)
- [ListPartnerWorkflowPresets200Response](docs/Model/ListPartnerWorkflowPresets200Response.md)
- [ListWorkspaceWorkflowCompositionOptions200Response](docs/Model/ListWorkspaceWorkflowCompositionOptions200Response.md)
- [ListWorkspaceWorkflowPresets200Response](docs/Model/ListWorkspaceWorkflowPresets200Response.md)
- [ListWorkspaceWorkflowVersions200Response](docs/Model/ListWorkspaceWorkflowVersions200Response.md)
- [ListWorkspaceWorkflows200Response](docs/Model/ListWorkspaceWorkflows200Response.md)
- [ManagedUser](docs/Model/ManagedUser.md)
- [ManagedUserEntriesMeta](docs/Model/ManagedUserEntriesMeta.md)
- [ManagedUserEntriesPageSuccess](docs/Model/ManagedUserEntriesPageSuccess.md)
- [ManagedUserEntryItem](docs/Model/ManagedUserEntryItem.md)
- [ManagedUserLimits](docs/Model/ManagedUserLimits.md)
- [ManagedUserOperationUsage](docs/Model/ManagedUserOperationUsage.md)
- [ManagedUserRemoval](docs/Model/ManagedUserRemoval.md)
- [ManagedUserResponse](docs/Model/ManagedUserResponse.md)
- [ManagedUserUsage](docs/Model/ManagedUserUsage.md)
- [ManagedUserUsageResponse](docs/Model/ManagedUserUsageResponse.md)
- [ManagedUserUsageTotals](docs/Model/ManagedUserUsageTotals.md)
- [MyPartner](docs/Model/MyPartner.md)
- [MyPartners](docs/Model/MyPartners.md)
- [MyPartnersResponse](docs/Model/MyPartnersResponse.md)
- [NewComposition](docs/Model/NewComposition.md)
- [NewEditorSession](docs/Model/NewEditorSession.md)
- [NewManagedUser](docs/Model/NewManagedUser.md)
- [NewWidget](docs/Model/NewWidget.md)
- [OfferWorkflowPresetRequest](docs/Model/OfferWorkflowPresetRequest.md)
- [OfferedWorkflowPreset](docs/Model/OfferedWorkflowPreset.md)
- [OfferedWorkflowPresetList](docs/Model/OfferedWorkflowPresetList.md)
- [OfferedWorkflowPresetWidget](docs/Model/OfferedWorkflowPresetWidget.md)
- [OperationsIdGetResponse](docs/Model/OperationsIdGetResponse.md)
- [OperationsIdGetResponseData](docs/Model/OperationsIdGetResponseData.md)
- [PartnerAnalyticsByManagedUser](docs/Model/PartnerAnalyticsByManagedUser.md)
- [PartnerAnalyticsByManagedUserResponse](docs/Model/PartnerAnalyticsByManagedUserResponse.md)
- [PartnerAnalyticsOfDay](docs/Model/PartnerAnalyticsOfDay.md)
- [PartnerAnalyticsOfManagedUser](docs/Model/PartnerAnalyticsOfManagedUser.md)
- [PartnerAnalyticsOfWidget](docs/Model/PartnerAnalyticsOfWidget.md)
- [PartnerAnalyticsSummary](docs/Model/PartnerAnalyticsSummary.md)
- [PartnerAnalyticsSummaryResponse](docs/Model/PartnerAnalyticsSummaryResponse.md)
- [PartnerAnalyticsTimeline](docs/Model/PartnerAnalyticsTimeline.md)
- [PartnerAnalyticsTimelineResponse](docs/Model/PartnerAnalyticsTimelineResponse.md)
- [PartnerAnalyticsTopWidgets](docs/Model/PartnerAnalyticsTopWidgets.md)
- [PartnerAnalyticsTopWidgetsResponse](docs/Model/PartnerAnalyticsTopWidgetsResponse.md)
- [PartnerBillingOverview](docs/Model/PartnerBillingOverview.md)
- [PartnerBillingOverviewBillingIntegration](docs/Model/PartnerBillingOverviewBillingIntegration.md)
- [PartnerBillingOverviewOperationalCredits](docs/Model/PartnerBillingOverviewOperationalCredits.md)
- [PartnerBillingOverviewPartner](docs/Model/PartnerBillingOverviewPartner.md)
- [PartnerContract](docs/Model/PartnerContract.md)
- [PartnerContractResponse](docs/Model/PartnerContractResponse.md)
- [PartnerCustomization](docs/Model/PartnerCustomization.md)
- [PartnerDataDatabase](docs/Model/PartnerDataDatabase.md)
- [PartnerDataDatabaseRemoval](docs/Model/PartnerDataDatabaseRemoval.md)
- [PartnerDataDatabaseRemovalResponse](docs/Model/PartnerDataDatabaseRemovalResponse.md)
- [PartnerDataDatabaseResponse](docs/Model/PartnerDataDatabaseResponse.md)
- [PartnerEntryContextSecret](docs/Model/PartnerEntryContextSecret.md)
- [PartnerEntryContextSecretResponse](docs/Model/PartnerEntryContextSecretResponse.md)
- [PartnerEntryContextSigning](docs/Model/PartnerEntryContextSigning.md)
- [PartnerEntryContextSigningResponse](docs/Model/PartnerEntryContextSigningResponse.md)
- [PartnerExtraCreditsInvoice](docs/Model/PartnerExtraCreditsInvoice.md)
- [PartnerExtraCreditsInvoiceResponse](docs/Model/PartnerExtraCreditsInvoiceResponse.md)
- [PartnerInvoice](docs/Model/PartnerInvoice.md)
- [PartnerNotification](docs/Model/PartnerNotification.md)
- [PartnerNotificationDefaultRecipients](docs/Model/PartnerNotificationDefaultRecipients.md)
- [PartnerNotificationDelivery](docs/Model/PartnerNotificationDelivery.md)
- [PartnerNotificationDeliveryLog](docs/Model/PartnerNotificationDeliveryLog.md)
- [PartnerNotificationDeliveryLogResponse](docs/Model/PartnerNotificationDeliveryLogResponse.md)
- [PartnerNotificationDeliveryResponse](docs/Model/PartnerNotificationDeliveryResponse.md)
- [PartnerNotificationEvent](docs/Model/PartnerNotificationEvent.md)
- [PartnerNotificationEventType](docs/Model/PartnerNotificationEventType.md)
- [PartnerNotificationPage](docs/Model/PartnerNotificationPage.md)
- [PartnerNotificationPageResponse](docs/Model/PartnerNotificationPageResponse.md)
- [PartnerNotificationSettings](docs/Model/PartnerNotificationSettings.md)
- [PartnerNotificationSettingsChange](docs/Model/PartnerNotificationSettingsChange.md)
- [PartnerNotificationSettingsChangeResponse](docs/Model/PartnerNotificationSettingsChangeResponse.md)
- [PartnerNotificationSettingsResponse](docs/Model/PartnerNotificationSettingsResponse.md)
- [PartnerNotificationTestEventRequest](docs/Model/PartnerNotificationTestEventRequest.md)
- [PartnerNotificationTestEventResult](docs/Model/PartnerNotificationTestEventResult.md)
- [PartnerNotificationTestEventResultResponse](docs/Model/PartnerNotificationTestEventResultResponse.md)
- [PartnerPreset](docs/Model/PartnerPreset.md)
- [PartnerPresetCopy](docs/Model/PartnerPresetCopy.md)
- [PartnerPresetCopyResponse](docs/Model/PartnerPresetCopyResponse.md)
- [PartnerPresetRemoval](docs/Model/PartnerPresetRemoval.md)
- [PartnerPresetRemovalResponse](docs/Model/PartnerPresetRemovalResponse.md)
- [PartnerPresetResponse](docs/Model/PartnerPresetResponse.md)
- [PartnerReportPage](docs/Model/PartnerReportPage.md)
- [PartnerReportPeriod](docs/Model/PartnerReportPeriod.md)
- [PartnerStorageDestination](docs/Model/PartnerStorageDestination.md)
- [PartnerStorageDestinationResponse](docs/Model/PartnerStorageDestinationResponse.md)
- [PartnerStorageRemoval](docs/Model/PartnerStorageRemoval.md)
- [PartnerStorageRemovalResponse](docs/Model/PartnerStorageRemovalResponse.md)
- [PartnerStorageUsage](docs/Model/PartnerStorageUsage.md)
- [PartnerStorageUsageOfManagedUser](docs/Model/PartnerStorageUsageOfManagedUser.md)
- [PartnerStorageUsageResponse](docs/Model/PartnerStorageUsageResponse.md)
- [PartnerStorageUsageTotals](docs/Model/PartnerStorageUsageTotals.md)
- [PatchBrandKitAssetRequest](docs/Model/PatchBrandKitAssetRequest.md)
- [PatchBrandKitRequest](docs/Model/PatchBrandKitRequest.md)
- [PatchBrandKitRequestFonts](docs/Model/PatchBrandKitRequestFonts.md)
- [PatchBrandKitRequestSpacing](docs/Model/PatchBrandKitRequestSpacing.md)
- [PersonalWorkspaceDomain](docs/Model/PersonalWorkspaceDomain.md)
- [PersonalWorkspaceDomainResult](docs/Model/PersonalWorkspaceDomainResult.md)
- [PersonalWorkspaceDomainResultResponse](docs/Model/PersonalWorkspaceDomainResultResponse.md)
- [PostBrandKitIconRequest](docs/Model/PostBrandKitIconRequest.md)
- [PostPublicCompositionEmbedStatus200Response](docs/Model/PostPublicCompositionEmbedStatus200Response.md)
- [PostPublicCompositionEmbedStatus200ResponseData](docs/Model/PostPublicCompositionEmbedStatus200ResponseData.md)
- [PostPublicCompositionEmbedStatusRequest](docs/Model/PostPublicCompositionEmbedStatusRequest.md)
- [PublicAdapterCallError](docs/Model/PublicAdapterCallError.md)
- [PublicAdapterCallRequest](docs/Model/PublicAdapterCallRequest.md)
- [PublicAdapterCallResult](docs/Model/PublicAdapterCallResult.md)
- [PublicAdapterCallResultData](docs/Model/PublicAdapterCallResultData.md)
- [PublicAdapterFileResult](docs/Model/PublicAdapterFileResult.md)
- [PublicAdapterFileResultData](docs/Model/PublicAdapterFileResultData.md)
- [PublicAdapterFileResultDataFile](docs/Model/PublicAdapterFileResultDataFile.md)
- [PublicCompositionEntryCreated](docs/Model/PublicCompositionEntryCreated.md)
- [PublicCompositionEntryCreatedData](docs/Model/PublicCompositionEntryCreatedData.md)
- [PublicCompositionEntryRequest](docs/Model/PublicCompositionEntryRequest.md)
- [PublicEmbedFailure](docs/Model/PublicEmbedFailure.md)
- [PublicEmbedFailureDetails](docs/Model/PublicEmbedFailureDetails.md)
- [PublicEmbedFailureError](docs/Model/PublicEmbedFailureError.md)
- [PublicWorkflow](docs/Model/PublicWorkflow.md)
- [PublicWorkflowEventsAccepted](docs/Model/PublicWorkflowEventsAccepted.md)
- [PublicWorkflowEventsRequest](docs/Model/PublicWorkflowEventsRequest.md)
- [PublicWorkflowEventsRequestEventsInner](docs/Model/PublicWorkflowEventsRequestEventsInner.md)
- [PublicWorkflowEventsRequestHeightsInner](docs/Model/PublicWorkflowEventsRequestHeightsInner.md)
- [PublicWorkflowTranslation](docs/Model/PublicWorkflowTranslation.md)
- [PublishWorkspaceWorkflow200Response](docs/Model/PublishWorkspaceWorkflow200Response.md)
- [PublishWorkspaceWorkflowRequest](docs/Model/PublishWorkspaceWorkflowRequest.md)
- [PurposeStorageBucket](docs/Model/PurposeStorageBucket.md)
- [PutBrandKitRequest](docs/Model/PutBrandKitRequest.md)
- [RemoveAiAnswersKnowledgeDocument200Response](docs/Model/RemoveAiAnswersKnowledgeDocument200Response.md)
- [RemovePartnerWorkflowPreset200Response](docs/Model/RemovePartnerWorkflowPreset200Response.md)
- [RemoveUserAdapterConnection200Response](docs/Model/RemoveUserAdapterConnection200Response.md)
- [ReportPublicWorkflowEvents200Response](docs/Model/ReportPublicWorkflowEvents200Response.md)
- [RequestExtraCredits](docs/Model/RequestExtraCredits.md)
- [ResponseMeta](docs/Model/ResponseMeta.md)
- [RevokeManagedUserEditorSessionsResponse](docs/Model/RevokeManagedUserEditorSessionsResponse.md)
- [RevokeManagedUserEditorSessionsResponseData](docs/Model/RevokeManagedUserEditorSessionsResponseData.md)
- [SaveWorkspaceWorkflow200Response](docs/Model/SaveWorkspaceWorkflow200Response.md)
- [SaveWorkspaceWorkflowRequest](docs/Model/SaveWorkspaceWorkflowRequest.md)
- [SetAdapterConnectionRequest](docs/Model/SetAdapterConnectionRequest.md)
- [SetCompositionDataSourceRequest](docs/Model/SetCompositionDataSourceRequest.md)
- [SetDynamicContentRequest](docs/Model/SetDynamicContentRequest.md)
- [SetDynamicContentResponse](docs/Model/SetDynamicContentResponse.md)
- [SetDynamicContentResponseData](docs/Model/SetDynamicContentResponseData.md)
- [SetDynamicContentResponseDataValidationResult](docs/Model/SetDynamicContentResponseDataValidationResult.md)
- [SetManagedUserLimitsRequest](docs/Model/SetManagedUserLimitsRequest.md)
- [SetPartnerDataDatabaseRequest](docs/Model/SetPartnerDataDatabaseRequest.md)
- [SetPartnerDesignDefaultsRequest](docs/Model/SetPartnerDesignDefaultsRequest.md)
- [SetPartnerPresetRequest](docs/Model/SetPartnerPresetRequest.md)
- [SetPartnerStorageDestinationRequest](docs/Model/SetPartnerStorageDestinationRequest.md)
- [SetPartnerWorkflowPreset200Response](docs/Model/SetPartnerWorkflowPreset200Response.md)
- [SetUserAdapterConnection200Response](docs/Model/SetUserAdapterConnection200Response.md)
- [SuccessResponse](docs/Model/SuccessResponse.md)
- [UpdateCanvasRequest](docs/Model/UpdateCanvasRequest.md)
- [UpdateComposition](docs/Model/UpdateComposition.md)
- [UpdateCompositionStatusRequest](docs/Model/UpdateCompositionStatusRequest.md)
- [UpdateDomainRequest](docs/Model/UpdateDomainRequest.md)
- [UpdateManagedUser](docs/Model/UpdateManagedUser.md)
- [UpdatePartnerEntryContextSigningRequest](docs/Model/UpdatePartnerEntryContextSigningRequest.md)
- [UpdatePartnerNotificationSettingsRequest](docs/Model/UpdatePartnerNotificationSettingsRequest.md)
- [UpdateUserApiKeyRequest](docs/Model/UpdateUserApiKeyRequest.md)
- [Upload](docs/Model/Upload.md)
- [UploadLimits](docs/Model/UploadLimits.md)
- [UploadLimitsResponse](docs/Model/UploadLimitsResponse.md)
- [UploadResponse](docs/Model/UploadResponse.md)
- [UploadsGet200Response](docs/Model/UploadsGet200Response.md)
- [UploadsIdDelete200Response](docs/Model/UploadsIdDelete200Response.md)
- [UploadsIdDelete200ResponseData](docs/Model/UploadsIdDelete200ResponseData.md)
- [UserApiKey](docs/Model/UserApiKey.md)
- [UserApiKeyResponse](docs/Model/UserApiKeyResponse.md)
- [UserApiKeyUsageLog](docs/Model/UserApiKeyUsageLog.md)
- [ValidateCompositionContentResponse](docs/Model/ValidateCompositionContentResponse.md)
- [ValidateCompositionContentResponseData](docs/Model/ValidateCompositionContentResponseData.md)
- [ValidateToken200Response](docs/Model/ValidateToken200Response.md)
- [ValidateToken200ResponseData](docs/Model/ValidateToken200ResponseData.md)
- [Widget](docs/Model/Widget.md)
- [Workflow](docs/Model/Workflow.md)
- [WorkflowCompositionAction](docs/Model/WorkflowCompositionAction.md)
- [WorkflowCompositionField](docs/Model/WorkflowCompositionField.md)
- [WorkflowCompositionOption](docs/Model/WorkflowCompositionOption.md)
- [WorkflowCompositionOptionActions](docs/Model/WorkflowCompositionOptionActions.md)
- [WorkflowCompositionOptionInputs](docs/Model/WorkflowCompositionOptionInputs.md)
- [WorkflowCompositionOptions](docs/Model/WorkflowCompositionOptions.md)
- [WorkflowConditionCase](docs/Model/WorkflowConditionCase.md)
- [WorkflowConditionTest](docs/Model/WorkflowConditionTest.md)
- [WorkflowCounter](docs/Model/WorkflowCounter.md)
- [WorkflowDetail](docs/Model/WorkflowDetail.md)
- [WorkflowDetailAllOfLastEditedBy](docs/Model/WorkflowDetailAllOfLastEditedBy.md)
- [WorkflowEdge](docs/Model/WorkflowEdge.md)
- [WorkflowFieldReference](docs/Model/WorkflowFieldReference.md)
- [WorkflowGraph](docs/Model/WorkflowGraph.md)
- [WorkflowIssue](docs/Model/WorkflowIssue.md)
- [WorkflowList](docs/Model/WorkflowList.md)
- [WorkflowNode](docs/Model/WorkflowNode.md)
- [WorkflowNodePosition](docs/Model/WorkflowNodePosition.md)
- [WorkflowPresetChoice](docs/Model/WorkflowPresetChoice.md)
- [WorkflowPresetChoices](docs/Model/WorkflowPresetChoices.md)
- [WorkflowPresetRemoval](docs/Model/WorkflowPresetRemoval.md)
- [WorkflowPresetWidget](docs/Model/WorkflowPresetWidget.md)
- [WorkflowPublishResult](docs/Model/WorkflowPublishResult.md)
- [WorkflowRemoved](docs/Model/WorkflowRemoved.md)
- [WorkflowSchedule](docs/Model/WorkflowSchedule.md)
- [WorkflowStats](docs/Model/WorkflowStats.md)
- [WorkflowStatus](docs/Model/WorkflowStatus.md)
- [WorkflowTrigger](docs/Model/WorkflowTrigger.md)
- [WorkflowTriggerValuesInner](docs/Model/WorkflowTriggerValuesInner.md)
- [WorkflowVersion](docs/Model/WorkflowVersion.md)
- [WorkflowVersionDetail](docs/Model/WorkflowVersionDetail.md)
- [WorkflowVersionList](docs/Model/WorkflowVersionList.md)
- [WorkflowVersionPublishedBy](docs/Model/WorkflowVersionPublishedBy.md)

## Authorization

Authentication schemes defined for the API:
### apiKeyAuth

- **Type**: Bearer authentication (JWT)

### bearerAuth

- **Type**: Bearer authentication (JWT)

### BearerAuth

- **Type**: Bearer authentication (JWT)

### ApiKeyAuth

- **Type**: API key
- **API key parameter name**: Authorization
- **Location**: HTTP header


### webhookSignature

- **Type**: API key
- **API key parameter name**: X-Webhook-Signature
- **Location**: HTTP header


## Tests

To run the tests, use:

```bash
composer install
vendor/bin/phpunit
```

## Author



## About this package

This PHP package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: `1.0.0`
    - Package version: `1.11.111`
    - Generator version: `7.9.0`
- Build package: `org.openapitools.codegen.languages.PhpClientCodegen`
