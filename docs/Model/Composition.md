# # Composition

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique identifier for the composition |
**creator_id** | **string** | ID of the user who created the composition |
**widget_id** | **string** | ID of the widget this composition is based on |
**name** | **string** | Name of the composition |
**content** | **object** | Content data for the composition |
**content_version** | **int** | Monotonic content version when the content_version migration is applied | [optional]
**status** | **string** | Current status of the composition |
**created_at** | **\DateTime** | When the composition was created |
**updated_at** | **\DateTime** | When the composition was last updated |
**embed_settings** | **object** | Settings for embedding the composition | [optional]
**design** | **object** | Design settings for the composition | [optional]
**database_id** | **string** | Legacy. The id of a Neon database that an earlier version made for this composition. A composition now keeps its tables in a schema of its own (named &#x60;comp_&#x60; followed by its id) in a database shared with other compositions, so new compositions have none. | [optional]
**project_id** | **string** | ID of the project this composition belongs to | [optional]
**managed_user_id** | **string** | The managed user the composition was made for, or null when it is your own. List one managed user&#39;s compositions with the &#x60;managedUserId&#x60; or &#x60;managedUserExternalId&#x60; query parameter of &#x60;getAllCompositions&#x60;. | [optional]
**direct** | **bool** | Whether the widget the composition is made from is drawn straight into the page, without a frame (&#x60;true&#x60;), or inside a frame (&#x60;false&#x60;). &#x60;null&#x60; when the widget has no published version yet. It is a fact about the widget&#39;s published version, so every composition of one widget answers the same, and it changes when you publish another version. It cannot be set. Only &#x60;getCompositionById&#x60; returns it: the other calls that return a composition leave it out, and so does that one on the rare occasion the answer could not be worked out just then (ask again). | [optional]
**last_edited_by** | [**\WidgeticApi\Model\CompositionLastEditedBy**](CompositionLastEditedBy.md) |  | [optional]
**last_edited_at** | **\DateTime** | When that latest change was made. Present whenever &#x60;lastEditedBy&#x60; is. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
