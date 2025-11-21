---
title: Best Practices for Templates
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

## Uploading images for templates

Images used in templates should come from the content repository, and need to be uploaded correctly to ensure the image is displayed accurately.

When a template features an edge-to-edge (full bleed) image, the selected image is automatically resized to fit the full template dimensions. However, if the image doesn't match the template aspect ratio, the image is cropped to fit the template dimensions and may not display as expected. 

There's no "autofit" functionality for images included in templates.

To resolve image cropping, users must define the aspect ratio of the image to be used in the template when it's uploaded to the content repository. When uploading an approved template:

1. [Proceed through the template upload process](/help/user-guide/templates/use-templates.md#add-a-template) until you reach the **[!UICONTROL Add details]** page.

2. Define the aspect ratio of the image to be used in the template in **[!UICONTROL Ad width (px)]** and **[!UICONTROL Ad height (px)]**. This will define the image window for the section of the template displaying the image.

3. In the **[!UICONTROL More details]** section, select the **[!UICONTROL Image size]** dropdown and choose _Crop to a fixed size_.
   ![Cropped to a fixed size](../content/images/crop-to-fixed-size.png "Cropped to a fixed size"){width="80%"}

To determine an image's size and aspect ratio in browser:

1. Inspect the image.
   - Windows/Linux:
     - Press F12.
   - macOS:
     - Press Command + Option + I.
   
1. Hover over the image.
   
1. Note the aspect ratio. Use this to define the aspect ratio of the image in the template.

When these details are not applied during upload, the image is assumed to be the entire aspect ratio of the template and images that don't match that aspect ratio exactly will appear cropped.

![Image cropped in a display ad](../content/images/cropped-display.png "Image cropping"){width="60%"}

**❌ Cropped image in a display ad template**

![Image displayed in a display ad](../content/images/full-fit.png "Image displayed in display ad"){width="60%"}

**✅ Image fully displayed**

## Follow channel-specific template guidelines

When creating templates, ensure they meet the specific requirements of the intended channel. Build templates that accommodate the layout and visual requirements for each channel. There are general guidelines that apply to any template, such as:

- Use clean and responsive HTML and inline CSS
- Use Adobe or Google fonts
- Do **not** use JavaScript

{{note-css-effects}}

See further tips and constraints when working with each template type to ensure optimal performance:

- [Emails](/help/user-guide/templates/email-template.md)
- [Display and banner ads](/help/user-guide/templates/display-template.md)
- [LinkedIn](/help/user-guide/templates/linkedin-template.md)
- [Meta ads](/help/user-guide/templates/meta-template.md)
