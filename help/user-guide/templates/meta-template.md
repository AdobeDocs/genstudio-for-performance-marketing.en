---
title: Prepare a Meta ad template for GenStudio for Performance Marketing
description: Learn how to prepare a custom Meta ad template for use in Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Media Templates
exl-id: e69039b0-272d-4f39-b0e4-916be710fd5f
---
# Prepare Meta ad template for Adobe GenStudio for Performance Marketing

Creating a Meta ad template involves a structured approach tailored for social media. After a Meta ad template is designed and tested, you can prepare it for upload and use in GenStudio for Performance Marketing.

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

- Use of [sections](/help/user-guide/content/customize-template.md#sections-or-groups):
   - Only one section can be used, generating a single set of template elements.
- Exactly one image field is required.

**Supported aspect ratios**:

Aspect ratio must be set:

- Square 1:1 (1080 x 1080 pixels)
- Portrait 4:5 (1080 x 1350 pixels)
- Story 9:16 (1080 x 1920 pixels)
- Landscape: 1.91:1 (1080 pixel width)
- Custom image size: (50 x 50 pixels minimum image width)

If the ad is not designed in one of these aspect ratios, GenStudio for Performance Marketing automatically crops the image into the appropriate size.

**Recognized field names**:

For Meta ads, the `headline`, `body`, and `CTA` fields are automatically generated. Use content placeholders for the following fields:

- `image` (selected from Content JPEG, PNG, or GIF)
- `on_image_text`

See [Content placeholders](/help/user-guide/content/customize-template.md#content-placeholders) to understand more about using field names in templates.
