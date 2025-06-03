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

Defining clear channel guidelines is essential to ensure that your generated content aligns with your brand's requirements and objectives. Channel guidelines let you specify rules for elements like tone, length, and style used in your template. For example, you can set a maximum character count for the body or require a specific call-to-action style. By setting these guidelines in advance, you reduce the need to write out detailed instructions in each AI prompt, streamlining the content generation process and ensuring consistency across your emails.

Review and define your Brand's [channel guidelines](/help/user-guide/guidelines/brands.md#channel-guidelines) for all key fields in your template. If you do not define guidelines, then the [default channel guidelines](/help/user-guide/guidelines/brands.md#default-channel-guidelines) are applied, which may not fully reflect your brand requirements.

![Body specifications](/help/assets/channel-email-body.png)

Learn how [Brands, Products, and Personas guidelines](/help/user-guide/guidelines/overview.md) influence generated content and how to tailor them for your marketing goals.

## Follow channel-specific template guidelines

When creating templates, ensure they meet the specific requirements of the intended channel. Build templates that accommodate the layout and visual requirements for each channel. There are general guidelines that apply to any template, such as:

- Use clean and responsive HTML and inline CSS
- Use Adobe or Google fonts
- Do **not** use JavaScript

{{note-css-effects}}

See further tips and constraints when working with each template type to ensure optimal performance and compatibility:

- [Emails](/help/user-guide/templates/email-template.md)
- [Display and banner ads](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Meta ads](/help/user-guide/templates/meta-template.md)
