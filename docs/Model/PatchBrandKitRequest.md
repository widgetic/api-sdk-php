# # PatchBrandKitRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**colors** | [**\WidgeticApi\Model\BrandColor[]**](BrandColor.md) | The whole list of colors (it replaces the saved list). | [optional]
**fonts** | [**\WidgeticApi\Model\PatchBrandKitRequestFonts**](PatchBrandKitRequestFonts.md) |  | [optional]
**spacing** | [**\WidgeticApi\Model\PatchBrandKitRequestSpacing**](PatchBrandKitRequestSpacing.md) |  | [optional]
**corner_radius** | **int** | One corner radius in pixels for the whole kit; the small, medium and large radii are made from it. 0 gives square corners. A radius step sent in &#x60;spacing&#x60; wins over the one made from this value. | [optional]
**instructions** | **string** | The kit owner&#39;s style notes (see &#x60;tokens.instructions&#x60;). An empty string removes them. | [optional]
**expected_version** | **int** | Refuse the change with a 409 when the kit was saved again since this version was read. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
