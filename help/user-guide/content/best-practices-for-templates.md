---
title: Best practices for templates
description: Follow best practices when using templates with Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
---
# Best practices for using templates

Templates significantly reduce the time and effort required to generate new content by providing a starting point that includes pre-configured layouts and design elements.

Use the following recommendations when using templates with GenStudio for Performance Marketing:

1. Know about [template elements](#know-about-template-elements)
1. Configure [channel guidelines](#configure-channel-guidelines) for effective personalization of content
1. Design with [accessibility standards](accessibility-for-templates.md) for an optimal experience
1. Follow [channel-specific template guidelines](#follow-channel-specific-template-guidelines)

>[!TIP]
>
>Learn more about basic template elements and procedures in [Work with Templates](use-templates.md). And deep-dive into [customizing a template](customize-template.md) for use in your next campaign.

## Know about template elements

As a best practice, familiarize yourself with the parts of a template. Each template type uses different elements to create a structure for channel-specific content creation. To customize your template, use the field names in place of these elements where you need GenStudio for Performance Marketing to generate content.

See [Template elements](use-templates.md#template-elements).

## Configure channel guidelines

Configure channel guidelines for each brand before using templates in GenStudio for Performance Marketing. The channel guidelines directly influence the type of content generated when using the template. For example, you can set character limits on the body of an email.

![Body specifications](/help/assets/channel-email-body.png)

See [channel guidelines](/help/user-guide/guidelines/brands.md#channel-guidelines).

## Follow channel-specific template guidelines

When creating templates, ensure they meet the specific requirements of the intended channel. Build templates that accommodate the layout and visual requirements for each channel. There are general guidelines that apply to any template, such as:

- Use clean and responsive HTML and inline CSS
- Use Adobe or Google fonts
- Do **not** use JavaScript

Consider the following tips and constraints when working with each template type to ensure optimal performance and compatibility:

>[!BEGINTABS]

>[!TAB Email]

Follow these design best practices when customizing email templates to work with GenStudio for Performance Marketing:

- Use Adobe or Google fonts
- Use clean and responsive HTML and inline CSS
- Do **not** use JavaScript
- Do **not** use fixed width in body or container
- Do **not** use base64 encoding for images because it can significantly increase the template size

**Constraints**:

- Use of [sections](customize-template.md#sections-or-groups):
   - A basic template (one section only) can generate a single set of template elements.
   - A complex template (multiple sections) can generate up to three sets of template elements.
- The maximum fields allowed in a template are 20
- The maximum HTML file size is 102 KB

**Recognized field names**:

For email, the `subject` field is automatically included. Use content placeholders for the following fields:

- `pre_header`
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (selected from Content JPEG, PNG, or GIF)

See [Content placeholders](customize-template.md#content-placeholders) to understand more about using field names in templates.

>[!TAB Meta ad]

Follow these design best practices when customizing Meta ad templates to work with GenStudio for Performance Marketing:

- Use 360 pixel width for column layouts
- Use a minimum resolution of 1080 x 1080 pixels for images
- Do **not** use relative font size
- Do **not** define viewport
- Do **not** use JavaScript
- Do **not** override an HTML element in the CSS
- Use the `<img>` tag instead of `background-image`
- Use masking to improve text readability over background images

**Constraints**:

- Use of [sections](customize-template.md#sections-or-groups):
   - Only one section can be used, generating a single set of template elements.

**Supported aspect ratios**:

- Square 1:1 (1080 x 1080 pixels)
- Portrait 4:5 (1080 x 1350 pixels)
- Story 9:16 (1080 x 1920 pixels)
- Landscape: 1.91:1 (1080 pixel width)
- Custom image size: (50 x 50 pixels minimum image width)

**Recognized field names**:

For Meta ads, the `headline`, `body`, and `CTA` fields are automatically generated. Use content placeholders for the following fields:

- `image` (selected from Content JPEG, PNG, or GIF)
- `on_image_text`

See [Content placeholders](customize-template.md#content-placeholders) to understand more about using field names in templates.

>[!TAB Banner & Display ad]

Follow these design best practices when customizing Banner and Display ad templates to work with GenStudio for Performance Marketing:

- Use Adobe or Google fonts
- Prepare assets that display well in slim dimensions
- Do **not** use embedded or encoded background images
- Use background images (`image` field) uploaded to the GenStudio for Performance Marketing content repository
- Do **not** use JavaScript

**Constraints**:

- Use of [sections](customize-template.md#sections-or-groups):
   - Only one section can be used, generating a single set of template elements.

**Supported dimensions**:

- Width x Height (pixels)
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

See [Content placeholders](customize-template.md#content-placeholders) to understand more about using field names in templates.

>[!TAB LinkedIn ad]

[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}

Follow these design best practices when customizing LinkedIn ad templates to work with GenStudio for Performance Marketing:

**Constraints**:

- Use of [sections](customize-template.md#sections-or-groups):
   - Only one section can be used, generating a single set of template elements.
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

See [Content placeholders](customize-template.md#content-placeholders) to understand more about using field names in templates.

>[!ENDTABS]
