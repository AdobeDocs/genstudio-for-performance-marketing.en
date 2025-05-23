---
title: Template guidelines
description: Follow best practices when using templates with Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates
---
# Template for guidelines topic

Paragraph about the template type.

Follow these design best practices when customizing LinkedIn ad templates to work with GenStudio for Performance Marketing:

**Constraints**:

- Use of [sections](/help/user-guide/content/customize-template.md#sections-or-groups):
   - Only one section can be used, generating a single set of template elements.
- Exactly one image field is required.
- Maximum image size of 5 MB
- Maximum headline 70 characters
- Maximum introductory text 150 characters

**Supported aspect ratios**:

- Square 1:1
  - desktop or mobile
  - Min: 360 x 360 pixels
  - Max: 4320 x 4320 pixels
- Horizontal 1.91:1
  - desktop
  - Min: 640 x 360 pixels
  - Max: 7680 x 4320 pixels
- Vertical 1:1.91
  - mobile
  - Min: 360 x 640 pixels
  - Max: 2430 x 4320 pixels
- Vertical 2.3
  - mobile
  - Min: 360 x 640 pixels
  - Max: 2430 x 4320 pixels
- Vertical 4.5 (recommended)
  - mobile
  - Min: 360 x 640 pixels
  - Max: 2430 x 4320 pixels

**Recognized field names**:

For LinkedIn ads, the `headline`, `introductory_text`, and `CTA` fields are automatically generated. Use content placeholders for the following fields:

- `image` (selected from Content JPEG, PNG, or GIF)
- `on_image_text`

See [Content placeholders](/help/user-guide/content/customize-template.md#content-placeholders) to understand more about using field names in templates.
