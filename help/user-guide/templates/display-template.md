---
title: Display Ad Template Guidelines
description: Follow best practices when using display ad and banner templates with Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
exl-id: 076239b3-9444-48f9-bdd6-ef2b757bdf0d
TQID: https://experienceleague.adobe.com/HjkLWiyqK1quHoZB5lEE-qyB3zci12KlRAZC8ME-9Ao
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
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

See [Content placeholders](/help/user-guide/templates/customize-template.md#content-placeholders) to understand more about using field names in templates.

## Supported dimensions

Width x Height (pixels) must be set.

| Orientation  | Dimensions (pixels)                                         | Notes                                                            |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Vertical     | 300 x 600<br>160 x 600                                      | Common for skyscraper and half-page banners.                      |
| Horizontal   | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Standard leaderboard, medium rectangle, and banner sizes.         |
| Custom       | 50 x 50 to 2000 x 2000                                      | Use for non-standard or unique placements; check platform limits. |

