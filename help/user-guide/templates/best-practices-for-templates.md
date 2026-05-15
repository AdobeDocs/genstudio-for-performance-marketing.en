---
title: Best Practices for Templates
description: Follow best practices when using templates with Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer, User
feature: Media Templates, Content Generation, Brand Personalization
exl-id: 3ff24fec-e836-4202-80f8-ba165e173b75
TQID: https://experienceleague.adobe.com/fiKHSZ-YFZ2gSD5iZ-aKaZtsC49Mrj1dqHpHqtbXZVM
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
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
    internal-label: Accessibility
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
    internal-label: Personalization
---
# Best practices for using templates

Templates significantly reduce the time and effort required to generate new content by providing a starting point that includes pre-configured layouts and design elements.

Adhere to the following recommendations when using templates with GenStudio for Performance Marketing:

1. Know about [template elements](#know-about-template-elements)
1. Configure [channel guidelines](#configure-channel-guidelines) for effective personalization of content
1. Design with [accessibility standards](accessibility-for-templates.md) for an optimal experience
1. Follow [channel-specific template guidelines](#follow-channel-specific-template-guidelines)
1. When using [Express templates](/help/user-guide/templates/express-templates.md), consider the specific tips under [Express to GenStudio template best practices](#express-to-genstudio-template-best-practices).
>
>Learn the basics of template elements and procedures in [Work with Templates](use-templates.md). And deep-dive into [customizing a template](customize-template.md) for specific instructions to use in your next campaign.

## Use the right template elements

 Each template type uses different elements to create a structure for channel-specific content creation. [Familiarize yourself with the parts of a template](use-templates.md#template-elements) and include the best elements for your content and template type. 
 
 When customizing your template, use the field names in place of these elements where you need GenStudio for Performance Marketing to generate content.

See [Template elements](use-templates.md#template-elements).

## Using placeholder text in templates

Placeholder text can help define syntax or structure for content to be filled in later in a template by a user. For example, {first_name}.{last_name}@email.etc. to define an email address. However, some common delimiters are already reserved for other meanings in GenStudio for Performance Marketing:

❌ `< >` - In use for HTML tags.
❌ `{{ }}` - In use for Handlebar expressions.

Use single brackets (whether straight or curly) to indicate placeholder text to avoid confusion with existing tags.

✅ `{first_name}` - Placeholder for first name.

## Configure channel guidelines

Defining clear channel guidelines is essential to ensure that your generated content aligns with your brand's requirements and objectives. Channel guidelines let you specify rules for elements like tone, length, and style used in your template. For example, you can set a maximum character count for the body or require a specific call-to-action style. By setting these guidelines in advance, you reduce the need to write out detailed instructions in each AI prompt, streamlining the content generation process and ensuring consistency across your emails.

Review and define your Brand's [channel guidelines](/help/user-guide/guidelines/brands.md#channel-guidelines) for all key fields in your template. If you don't define guidelines, then the [default channel guidelines](/help/user-guide/guidelines/brands.md#default-channel-guidelines) are applied, which may not fully reflect your brand requirements.

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
   ![Cropped to a fixed size](images/crop-to-fixed-size.png "Cropped to a fixed size"){width="80%"}

To determine an image's size and aspect ratio in browser:

1. Inspect the image.
   - On Windows/Linux:
     - Press F12.
   - On macOS:
     - Press Command + Option + I.
   
1. Hover over the image.
   
1. Note the aspect ratio. Use this to define the aspect ratio of the image in the template.

When these details are not applied during upload, the image is assumed to be the entire aspect ratio of the template and images that don't match that aspect ratio exactly will appear cropped.

![Image cropped in a display ad](images/cropped-display.png "Image cropping"){width="60%"}

**❌ Cropped image in a display ad template**

![Image displayed in a display ad](images/full-fit.png "Image displayed in display ad"){width="60%"}

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

## Express to GenStudio template best practices

The following tips help you get reliable results when you convert designs from [!DNL Adobe Express] into templates for [!DNL GenStudio for Performance Marketing].

### Use Multi-variation templates

In [!DNL Adobe Express], pages can represent multiple size or aspect ratio variations in one template file.
When you select the template in [!DNL GenStudio for Performance Marketing], all variations appear in the canvas.

This behavior improves on HTML templates, which support only one variation per file.

### Locking fields to control what marketers can edit

Use locking to communicate intent. For example, lock a legal disclaimer so it is never AI-generated, but leave a headline flexible for generation.

Right-click any element in [!DNL Adobe Express] to set lock behavior:

- **[!UICONTROL Full lock]** — The element is static, and AI does not generate content for it.
- **[!UICONTROL Lock, allow image replace]** — Locks size and position but lets users swap the image. This option works well for logos.
- **[!UICONTROL Lock, allow text replace]** — Locks size and position but lets users edit text. AI does not auto-generate content for it.
- **Fully flexible** (unlocked) — Users can move and resize the element, and AI treats it as content to generate.

### Name layers for better AI mapping

When you convert a design to a template, AI scans the design and maps fields such as headline, CTA, and body copy. AI maps simple templates accurately more often than highly complex layouts.

**Best practice:** In placeholder copy, include the intended field type (for example, `headline`, `sub-headline`, or `CTA`) to help the AI map fields correctly. This approach can reduce mapping errors.

### Convert to template

1. In [!DNL Adobe Express], click **[!UICONTROL Share]** > **[!UICONTROL Convert to Template]**.
1. Only the **[!UICONTROL Info]** tab and **[!UICONTROL Locks]** tab carry over to [!DNL GenStudio for Performance Marketing].
1. At conversion time, choose how unlocking works:
   - **[!UICONTROL Allow users to unlock]**
   - **[!UICONTROL Prevent all unlocking]**
   - **[!UICONTROL Set a passphrase]** — A middle ground that discourages casual changes without blocking access permanently.

### Keep a copy of the original design file

Converting creates a separate [!DNL Adobe Express] template file, however the original design file stays editable.

**Tip:** Keep the original so you can revise the design, create variations, and generate new templates later.

### Share for greater visibility

After conversion, the template is visible only to you by default. You can share it with individuals or with the whole organization.

**Requirement:** [!DNL Adobe Express] and [!DNL GenStudio for Performance Marketing] must use the same IMS organization for templates to sync. Templates usually appear in [!DNL GenStudio for Performance Marketing] almost immediately after conversion.

### Control AI field mapping

After you select a template, AI maps fields once per template, assigning labels such as **[!UICONTROL primary media]**, **[!UICONTROL generated]**, or **[!UICONTROL locked]**. You can adjust mappings manually when AI assigns fields incorrectly.

Use the **[!UICONTROL Enable generation]** toggle per field to turn on or off before you generate. You can adjust mappings manually when AI assigns fields incorrectly. Permanent corrections to template mappings are planned for a future release.

### Design in [!DNL Adobe Express], assemble in [!DNL GenStudio for Performance Marketing]

Consider these design workflows to utilize each service at its best:

- Complete design work such as colors, layouts, and graphics in [!DNL Adobe Express].
- Use [!DNL GenStudio for Performance Marketing] to assemble and generate content from those templates.
- Use [!DNL Adobe Express] brands (colors, logos, fonts, and graphics) for design governance.
- Use [!DNL GenStudio for Performance Marketing] brands for font color changes after generation.

### Email limitations

Email is **not** supported on the Horizon Canvas for the [!DNL Adobe Express] template workflow. Email continues to use the traditional HTML template process.

### Take advantage of custom fonts

Teams often ask how custom fonts work with [!DNL Adobe Express] templates. Admins may need to accept the Custom Fonts qualifying offer in the admin console before those fonts are available; see [Using [!DNL Adobe Express] templates](express-templates.md).
