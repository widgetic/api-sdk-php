# # Canvas

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique identifier for the canvas |
**persistence_key** | **string** | Key used for persistent storage and reference |
**canvas_content** | **object** | JSON content of the canvas, containing layout and configuration | [optional]
**creator_id** | **string** | UUID of the user who created the canvas | [optional]
**primary_widget_id** | **string** | Primary widget for My widgets list and canvas-only deep-link (Convert per shape may add secondary widgets on the same canvas) | [optional]
**managed_user_id** | **string** | The managed user the canvas was made for (Widgetic&#39;s id for the user); null for a canvas that is the account&#39;s own. | [optional]
**created_at** | **\DateTime** | Timestamp when the canvas was created |
**updated_at** | **\DateTime** | Timestamp when the canvas was last updated |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
