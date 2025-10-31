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

When a display template features an edge-to-edge (full bleed) image, the selected image is automatically resized to fit the full template dimensions. However, if the image doesn't match the template aspect ratio, the image is cropped to fit the template dimensions and may not display as expected. 

There's no "autofit" functionality for images in display ad templates.

To resolve image cropping, users must define the aspect ratio of the image in the template when it's uploaded to the content repository. When uploading an approved display ad template:

1. [Proceed through the template upload process](/help/user-guide/content/use-templates.md#add-a-template) until you reach the **[!UICONTROL Add details]** page.

1. Define the aspect ratio of the image to be used in the template in **[!UICONTROL Ad width (px)]** and **[!UICONTROL Ad height (px)]**. This will define the image window for the section of the template displaying the image.

1. In the **[!UICONTROL More details]** section, select the **[!UICONTROL Image size]** dropdown and choose _Crop to a fixed size_.
   ![Cropped to a fixed size](./crop-to-fixed-size.png "Cropped to a fixed size"){width="80%"}

To determine an image's size and aspect ratio in browser:

1. Inspect the image.
   - Windows/Linux:
     - Press F12.
   - macOS:
     - Press Command + Option + I.
   
1. Hover over the image.
   
1. Note the aspect ratio. Use this to define the aspect ratio of the image in the template.

When these details are not applied during upload, the image is assumed to be the entire aspect ratio of the template and images that don't match that aspect ratio exactly will appear cropped.

![Image cropped in a display ad](./cropped-display.png "Image cropping"){width="60%"}

**❌ Cropped image in a display ad template**

![Image displayed in a display ad](./full-fit.png "Image displayed in display ad"){width="60%"}

**✅ Image fully displayed**
