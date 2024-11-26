---
title: Best practices for templates
description: Follow best practices when using templates with Adobe GenStudio for Performance Marketing.
feature: Templates, Content
last-substanial-update: 2024-11-15
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

Configure channel guidelines for each brand before using templates in GenStudio for Performance Marketing. The channel guidelines directly influence the type of content generated when using the template. For example, you can set character limits on the body of an email:

![Body specifications](/help/assets/channel-email-body.png)

See [channel guidelines](../guidelines/brands.md#channel-guidelines).

## Follow channel-specific template guidelines

Build templates that accommodate the layout and visual requirements for each channel. Consider the following tips and constraints when working with each template type to ensure optimal performance and compatibility:

>[!BEGINTABS]

>[!TAB Email]

Follow these design best practices when customizing email templates to work with GenStudio for Performance Marketing:

- Use Adobe or Google fonts
- Use clean and responsive HTML and inline CSS
- Do **not** use JavaScript
- Do **not** use fixed width in body or container
- Do **not** use base64 encoding for images

**Constraints**:

- For a basic template (one section) only generates a maximum of 1 set of template elements
- For a complex template (multiple sections) only generates a maximum of 3 sets of template elements
- Field maximum is 20
- Email size maximum is 120k

>[!TAB Meta ad]

Follow these design best practices when customizing Meta ad templates to work with GenStudio for Performance Marketing:

- Use 360 pixel width for column layouts
- Do **not** define viewports
- Do **not** override an HTML element in the CSS
- Add `object-fit: cover` value to `background-image` CSS class
- Do **not** use relative font size
- Use a minimum resolution of 1080x1080 for images

**Constraints**:

- Only generates 1 set of template elements

**Supported aspect ratios**:

- 1:1
- 4:5
- 9:16

>[!TAB Display ad]

Follow these design best practices when customizing display ad templates to work with GenStudio for Performance Marketing:

- Use Adobe or Google fonts
- Prepare assets that display well in slim dimensions
- Use background images (`image` field) uploaded to the GenStudio for Performance Marketing content repository; do **not** use embedded or encoded background images

**Constraints**:

- Only generates 1 set of template elements

**Supported dimensions**:

- Vertical: 300x600, 160x600​
- Horizontal: 300x250, 728x90, 336x280, 320x50, 970x250​

>[!ENDTABS]
