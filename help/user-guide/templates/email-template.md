---
title: Prepare an email template for GenStudio for Performance Marketing
description: Learn how to prepare an email template for use in Adobe GenStudio for Performance Marketing.
level: Intermediate
feature: Media Templates
exl-id: 8b1e8d32-5a23-45ce-a2d4-ae6de3698c45
---
# Prepare a marketing email template for use in GenStudio for Performance Marketing

Start with a well-designed HTML email template, typically created in a design program such as Adobe XD. Once your template is ready, you can prepare it for upload and use in GenStudio for Performance Marketing. As a best practice, email templates should:

Follow these design best practices when customizing email templates to work with GenStudio for Performance Marketing:

- Use Adobe or Google fonts
- Use clean and responsive HTML and inline CSS
- Do **not** use JavaScript
- Do **not** use fixed width in body or container
- Do **not** use base64 encoding for images because it can significantly increase the template size

**Constraints**:

- Marketing emails can have 0, 2, or 3 [sections](/help/user-guide/content/customize-template.md#sections-or-groups):
   - A basic template (zero sections) can generate a single set of template elements, which does not require the group naming convention.
   - A complex template (multiple sections) can generate up to three sets of template elements, which requires you to adhere to the group naming convention: (`groupname_fieldname`)
- The maximum fields allowed in a template are 20
- The maximum HTML file size is 102 KB

**Recognized field names**:

For email, the `subject` field is automatically included. Use content placeholders for the following fields:

- `pre_header` (rich text not enabled)
- `headline`
- `sub_headline`
- `body`
- `cta`
- `image` (selected from Content JPEG, PNG, or GIF)

See [Content placeholders](/help/user-guide/content/customize-template.md#content-placeholders) to understand more about using field names in templates.
