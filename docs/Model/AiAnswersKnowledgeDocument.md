# # AiAnswersKnowledgeDocument

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Use it to remove the document |
**title** | **string** | What the document is called. Visitors see it as the source of an answer, so write it for them |
**status** | **string** | &#x60;ready&#x60; documents are used to answer questions. A &#x60;processing&#x60; document is not: it is being added, or an add was interrupted. Remove one that stays in this state and add it again |
**char_count** | **int** | How many characters of text the document holds, after it was cleaned |
**chunk_count** | **int** | Into how many passages the text was cut. Zero until the document is ready |
**created_at** | **\DateTime** |  |
**ready_at** | **\DateTime** | When the document became ready. Null while it is not |

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
