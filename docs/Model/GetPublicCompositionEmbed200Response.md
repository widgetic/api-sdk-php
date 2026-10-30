# # GetPublicCompositionEmbed200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**composition_id** | **string** |  | [optional]
**widget_id** | **string** |  | [optional]
**version** | **int** |  | [optional]
**widget_version** | **int** | Published widget version on the CDN artifact this composition uses. | [optional]
**player_version** | **int** | Version of the player: the gateway frame wrapper that shows the widget, and the host bridge it speaks with the embedding page and the widget (currently 6). Raised when the messages between page, frame, and widget change in a way a widget could notice, such as a new &#x60;widgetic:host&#x60; field or a new forwarded event (2 added &#x60;entries&#x60;, 3 added &#x60;adapters&#x60;, 4 added &#x60;entries.writeToken&#x60;, 5 added the A/B goal: &#x60;widgetic:ab-goal&#x60; to the widget and &#x60;widgetic:goal&#x60; back, 6 added the watch of a workflow: &#x60;widgetic:workflow-watch&#x60; to the widget, the watched values in &#x60;widgetic:submitted&#x60; and the watched action in &#x60;widgetic:goal&#x60;). It is not &#x60;widgetVersion&#x60; (the version of the published widget) and not the &#x60;version&#x60; inside a &#x60;widgetic:host&#x60; message. | [optional]
**data_source** | [**\WidgeticApi\Model\GetPublicCompositionEmbed200ResponseDataSource**](GetPublicCompositionEmbed200ResponseDataSource.md) |  | [optional]
**embed_url** | **string** |  | [optional]
**entry_write_token** | **string** | Signed per-composition write token for &#x60;POST /embed/compositions/{compositionId}/entries/{table}&#x60;, also handed to the widget inside &#x60;widgetic:host&#x60; as &#x60;entries.writeToken&#x60;. | [optional]
**entries** | [**\WidgeticApi\Model\GetPublicCompositionEmbed200ResponseEntries**](GetPublicCompositionEmbed200ResponseEntries.md) |  | [optional]
**adapters** | [**\WidgeticApi\Model\GetPublicCompositionEmbed200ResponseAdapters**](GetPublicCompositionEmbed200ResponseAdapters.md) |  | [optional]
**width** | **int** |  | [optional]
**height** | **int** |  | [optional]
**design** | **object** |  | [optional]
**content** | **object** |  | [optional]
**content_items** | **array<string,mixed>[]** |  | [optional]
**iframe_allow** | **string** | The browser features the widget needs the iframe that shows it to be allowed to use, as the value of that iframe&#39;s &#x60;allow&#x60; attribute (for example &#x60;camera; microphone&#x60;; the words are &#x60;camera&#x60;, &#x60;display-capture&#x60; and &#x60;microphone&#x60;). Present only for a widget that uses a module that needs one, and absent for every other widget. A page that embeds the frame itself copies it onto its own iframe (&#x60;allow&#x3D;\&quot;...\&quot;&#x60;); a page that does not leaves the widget to say, in its own words, that the feature is blocked there. The frame wrapper already passes it on to the iframe it holds. | [optional]
**media** | [**\WidgeticApi\Model\GetPublicCompositionEmbed200ResponseMedia**](GetPublicCompositionEmbed200ResponseMedia.md) |  | [optional]
**direct** | [**\WidgeticApi\Model\GetPublicCompositionEmbed200ResponseDirect**](GetPublicCompositionEmbed200ResponseDirect.md) |  | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
