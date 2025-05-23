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

**Supported dimensions**:

- Width x Height (pixels) must be set
- Vertical:
   - 300 x 600
   - 160 x 600​
- Horizontal:
   - 300 x 250
   - 728 x 90
   - 336 x 280
   - 320 x 50
   - 970 x 250​
- Custom: 50 x 50 to 2000 x 2000

**Recognized field names**:

For Banner and Display ads, the `CTA` field is automatically generated. Use content placeholders for the following fields:

- `headline`
- `sub_headline`
- `body`
- `image` (selected from Content JPEG, PNG, or GIF)

See [Content placeholders](/help/user-guide/content/customize-template.md#content-placeholders) to understand more about using field names in templates.
