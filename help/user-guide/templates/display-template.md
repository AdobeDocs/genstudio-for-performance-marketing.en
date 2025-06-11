---
title: Display ad template guidelines
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
- Use background images (`image` field) uploaded to the GenStudio for Performance Marketing content repository
- Do **not** use JavaScript
- Only one section can be used, generating a single set of template elements

## Recognized field names

For banner and display ads, GenStudio for Performance Marketing automatically generates the `cta` field. When customizing your template, use content placeholders for the following required fields:

- `headline`
- `sub_headline`
- `body`
- `image` (required, selected from Content JPEG, PNG, or GIF)

See [Content placeholders](/help/user-guide/content/customize-template.md#content-placeholders) to understand more about using field names in templates.

## Supported dimensions

Width x Height (pixels) must be set.

| Orientation  | Dimensions (pixels)                                         | Notes                                                            |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Vertical     | 300 x 600<br>160 x 600                                      | Common for skyscraper and half-page banners                      |
| Horizontal   | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Standard leaderboard, medium rectangle, and banner sizes         |
| Custom       | 50 x 50 to 2000 x 2000                                      | Use for non-standard or unique placements; check platform limits |

<!-- Potentially add an example

## Template example

+++Example: Display ad template

+++

-->
