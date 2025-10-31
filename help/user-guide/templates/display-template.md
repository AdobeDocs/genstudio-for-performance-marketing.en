---
title: Display Ad Template Guidelines
description: Follow best practices when using display ad and banner templates with Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
---
# Display ad template guidelines

Display templates are pre-designed layouts used to create visually engaging banner and display ads. They provide a flexible framework for incorporating images, text, and call to action, ensuring consistency and efficiency when producing multiple ad variations. When preparing your template for use in GenStudio for Performance Marketing, make sure that all assets are optimized for web display and meet the required file formats and sizes.

Follow these design best practices when customizing Banner and Display ad templates to work with GenStudio for Performance Marketing:

- Use Adobe or Google fonts
- Prepare assets that display well in slim dimensions
- Exactly one image field is required
- Do **not** use embedded or encoded background images
- Use background images (`image` field) uploaded to the GenStudio for Performance Marketing content repository. Adhere to the guidelines in [Uploading images for display ads](#uploading-images-for-display-ads) for the best results
- Do **not** use JavaScript
- Only one section can be used, generating a single set of template elements

## Recognized field names

When customizing your banner or display ad template, use content placeholders for the following required fields:

- `headline`
- `sub_headline`
- `body`
- `image` (required, selected from Content JPEG, PNG, or GIF)

GenStudio for Performance Marketing automatically generates the following fields. You do not have to apply content placeholders for:

- `cta`

See [Content placeholders](/help/user-guide/content/customize-template.md#content-placeholders) to understand more about using field names in templates.

## Supported dimensions

Width x Height (pixels) must be set.

| Orientation  | Dimensions (pixels)                                         | Notes                                                            |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Vertical     | 300 x 600<br>160 x 600                                      | Common for skyscraper and half-page banners.                      |
| Horizontal   | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Standard leaderboard, medium rectangle, and banner sizes.         |
| Custom       | 50 x 50 to 2000 x 2000                                      | Use for non-standard or unique placements; check platform limits. |

## Uploading images for display ads

Images used in display ads should come from the content repository, and need to be uploaded correctly to ensure the image is displayed accurately in the template.
When a display template features an edge-to-edge (full bleed) image, the selected image is automatically resized to fit the template dimensions. However, if the image doesn't match the template aspect ratio, the image is cropped to fit the template dimensions and may not display as expected. 

There's no "autofit" functionality for images in display ad templates.

To resolve image cropping, users must upload the image to the content repository


Core issue: Users of GSPeM assume autofit for image sizing within their banner, display, and template will be automatically applied during upload when template aspect ratio is defined. While this is true for full bleed templates (where image = aspect ratio of entire templates), 

For templates where image does not = aspect ratio of entire template:

1. Define the aspect ratio of the image in the template.

1. Select "Cropped to a fixed size".
   ![Cropped to a fixed size](/help/assets/cropped-to-fixed-size.png "Cropped to a fixed size"){width="30%"}

To inspect an image's size and aspect ratio in browser:

1. Inspect the image.
   
1. Hover over the image.
   
1. Note the aspect ratio. Use this to define the aspect ratio of the image in the template.

If this workflow is not applied during upload, the image is assumed to be the entire aspect ratio and the cropping will not show as expected on customer side.
