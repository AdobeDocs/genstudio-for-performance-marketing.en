---
title: Template guidelines
description: Follow best practices when using templates with Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
---
# Template for guidelines topic

Paragraph about the template type.

Follow these design best practices when customizing Banner and Display ad templates to work with GenStudio for Performance Marketing:

- Use Adobe or Google fonts
- Prepare assets that display well in slim dimensions
- Do **not** use embedded or encoded background images
- Use background images (`image` field) uploaded to the GenStudio for Performance Marketing content repository
- Do **not** use JavaScript

**Constraints**:

- Use of [sections](/help/user-guide/content/customize-template.md#sections-or-groups):
   - Only one section can be used, generating a single set of template elements.
- Exactly one image field is required.

## Supported dimensions

Width x Height (pixels) must be set.

| Orientation  | Dimensions (pixels)                                         | Notes                                                            |
|--------------|-------------------------------------------------------------|------------------------------------------------------------------|
| Vertical     | 300 x 600<br>160 x 600                                      | Common for skyscraper and half-page banners                      |
| Horizontal   | 300 x 250<br>728 x 90<br>336 x 280<br>320 x 50<br>970 x 250 | Standard leaderboard, medium rectangle, and banner sizes         |
| Custom       | 50 x 50 to 2000 x 2000                                      | Use for non-standard or unique placements; check platform limits |

## Recognized field names

For Banner and Display ads, the `cta` field is automatically generated. When customizing your template, apply content placeholders for these required fields:

- `headline`
- `sub_headline`
- `body`
- `image` (selected from Content JPEG, PNG, or GIF)

See [Content placeholders](/help/user-guide/content/customize-template.md#content-placeholders) to understand more about using field names in templates.

<!-- Potentially add an example

## Template example

+++Example: Display ad template

+++

-->
