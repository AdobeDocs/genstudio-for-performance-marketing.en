---
title: Work with Templates
description: Discover how to use templates effectively to streamline your creative process in Adobe GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates
exl-id: 7705bb79-19ca-4c16-8f8b-95bf8687e96d
---
# Work with Templates

GenStudio for Performance Marketing enables content creators to produce consistent on-brand marketing content quickly using _templates_. A template significantly reduces the time and effort required to generate new content by providing a starting point that includes pre-configured layouts and design elements. To get started, upload a custom template in [!DNL Content] or use a starter template in [!DNL Create]. [Starter templates](/help/user-guide/templates/starter-templates.md) provide a quick way to begin with a standard design, while a custom template allows you to use your unique designs and layout.

While GenStudio for Performance Marketing does not support the direct creation of templates within the application, you can easily design and prepare templates using popular design tools, such as Adobe InDesign, Illustrator, or Express. Once your design is complete, you can adapt it for use in GenStudio for Performance Marketing. Begin using templates by following these steps:

1. **Design Your Template**: Use your preferred design tool to create the visual layout of your [template with elements](#template-elements) such as a preheader, headline, body, CTA, images, and footer.

2. **Code Your Template**: Convert your design into HTML and inline CSS to ensure it is clean and responsive across various devices. Consider the [accessibility guidelines](accessibility-for-templates.md) to aid in reaching your maximum intended audience.

3. **Prepare for GenStudio for Performance Marketing**: Adapt your HTML template using the Handlebars templating language. Insert placeholders to indicate where GenStudio for Performance Marketing should generate content dynamically. See how to [Customize a template](customize-template.md) for GenStudio for Performance Marketing.

By following these steps, you can create professional and effective templates that are ready for use in GenStudio for Performance Marketing, enabling you to produce on-brand content quickly and efficiently.

## Template elements

A template is a set of instructions defined with HTML and inline CSS that can be used to produce an email, social ad, or display ad experience. Template elements provide the structure for content creation.

The following is a list of elements that are used in templates and some details about their characteristics:

| **Element**          | **Channel**                              | **Description**                                                                                                                                              |
|----------------------|------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Preheader**        | Email                                    | A secondary subject line in an email, typically between 40-50 characters, that enhances the main subject line. It is visible in the inbox alongside the subject before the email is opened. |
| **Header**           | Email                                    | The top section of the email the recipient sees when opening the email sets the tone and provides context for the included content.                      |
| **Headline**         | Meta ad, Banner and Display ads, LinkedIn | The first content that the recipient sees should be compelling to catch interest.                                                                             |
| **Sub-headline**     | Email, Banner and Display ads            | A secondary text element that supports the headline. It is typically concise and designed to complement the main headline, drawing the reader's attention further into the content. |
| **Introductory text**| LinkedIn                                 | The primary message conveys the core message, similar to the body copy. It can use up to 150 characters, including spaces, a maximum of four emojis, and punctuation. |
| **Body**             | Email, Meta ad, Banner and Display ads   | The main text of the advertisement conveys the core message. It should be engaging, informative, and persuasive to encourage the desired action from the audience. |
| **CTA**              | Email, Meta ad, Banner and Display ads, LinkedIn | A call-to-action button uses a phrase and a link to encourage the recipient to take a specific action, such as clicking a link or making a purchase.      |
| **Images**           | Email, Meta ad, Banner and Display ads, LinkedIn | Enhance visual appeal, break up text, and support the message. Images should be high-quality and eye-catching.                                                   |
| **Footer**           | Email                                    | The bottom section of the email contains additional content such as contact details, social media links, disclaimers, and unsubscribe options.            |
| **Text Overlay**     | Meta ad                                  | Text placed on an image to support and enhance the headline and body content.                                                                                  |

>[!TIP]
>
>See the [recognized field names](customize-template.md#recognized-field-names) that GenStudio for Performance Marketing supports for templates of each Channel type.

## Customize template

You [customize your template](customize-template.md) for use in GenStudio for Performance Marketing by inserting content placeholders, or fields, that the generative AI uses to insert content. GenStudio for Performance Marketing recognizes certain fields, such as the `body` field, and adheres to the channel guidelines configured for the selected brand.

>[!TIP]
>
>Follow [accessibility guidelines](accessibility-for-templates.md) and [best practices](/help/user-guide/templates/best-practices-for-templates.md) so that you can reach more of your audience and provide an optimal experience.

## Manage templates

The _[!DNL Templates]_ gallery displays your inventory of templates customized for generating experiences in GenStudio for Performance Marketing.

### Search templates

Each [!DNL Content] view provides filter options to narrow your search for the ideal asset, experience, or template. There are filters based on [guidelines](/help/user-guide/guidelines/overview.md), [keywords](asset-details.md#user-defined-metadata), and [attribute categories](/help/user-guide/insights/attributes.md#categories) to narrow search results.

For example, you may want to find a template of a specific channel type or aspect ratio created by you:

- **[!UICONTROL Created by]**: limits the _[!UICONTROL Templates]_ list to show only the templates created by you or a specific person.
- **[!UICONTROL Aspect Ratio]**: limits the _[!UICONTROL Templates]_ list to show templates designed for a specific aspect ratio.

The following shows filter by the channel type, such as email, Display ads, Meta ads, and LinkedIn ads.

![Content template list](/help/assets/content-templates-filter.png "Search the LinkedIn templates"){width="650"}

The template search capability is available during [!UICONTROL Create] when selecting a template for owned or paid media. If certain filter options are not visible, it indicates that no templates in the repository match the corresponding metadata criteria. Ensure that templates are properly tagged with metadata to make them discoverable through these filters.

### Add a template

Before uploading a template, ensure it is fully prepared and ready for use in GenStudio for Performance Marketing by following the guidance in [Customize templates](customize-template.md).

**To add a template**:

1. In _[!DNL Content]_, select the **[!UICONTROL Templates]** section.

2. Click **[!UICONTROL Add template]**.

3. In the _[!UICONTROL Add your approved template]_ pane, browse for the HTML template file or drag the HTML template file to the drop space. Click **[!UICONTROL Next]**.

4. In the _[!UICONTROL Check detected fields]_ pane, review the fields. Verify that you are using the correct template and that all the details are as expected.

   Example Preview for an email template:

   ![Preview fields detected](/help/assets/template-detected-fields.png){width="650"}

   >[!TIP]
   >
   >If the template is not correct, click **[!UICONTROL Back]** and return to the previous step. Upload the corrected template file. Or use the [template code editor](/help/user-guide/templates/code-editor.md) to make simple corrections.

5. Click **[!UICONTROL Next]** when you are satisfied with the template preview.

6. In _[!UICONTROL Provide template details and upload]_, name your template and select a **[!UICONTROL Channel]** type.

   Template name and channel type are required. Additional requirements may include:

   - **Meta**: requires Aspect ratio
   - **Banner and Display ad**: requires Dimensions

7. Add as many details as you can to improve template identification in searches and filtering.

8. Click **[!UICONTROL Done]**.

### Refresh template

Templates may include static files, such as icons or logos. [Static content](/help/user-guide/content/customize-template.md#static-content) is not stored after creating the template preview. GenStudio for Performance Marketing continues to reference the source link provided in the template. Use refresh to update the template preview with the latest versions of these assets.

**To refresh the template**:

1. In _[!DNL Content]_, select the **[!UICONTROL Templates]** section.

2. Click on a template for a full view and a list of details.

3. Click **[!UICONTROL Refresh]** (circling arrows) from the upper right corner to perform a refresh of all assets used in the template.

### Create an experience with a template

Find and use an existing template in GenStudio for Performance Marketing to create more experiences.

**To create an experience with a template**:

1. In _[!DNL Content]_, select the **[!UICONTROL Templates]** section.

2. Click on a template for a full view and a list of details.

3. Click **[!UICONTROL Create Experience]** (paintbrush) from the upper right corner to use the template.

4. Continue to [Create](/help/user-guide/create/overview.md#create-use-cases) an experience.

## Templates from AJO and Marketo

You can upload a template that you created in Adobe Journey Optimizer (AJO) or Marketo. GenStudio for Performance Marketing detects application-specific patterns and ignores them, preserving the original form for continued use in AJO or Marketo. You do not need to make any changes to the original AJO or Marketo syntax.

Recognized application patterns include:

- **AJO**: `{{profile.*}}`, `{{context.*}}`
- **Marketo**: `{{my.*}}`, `{{lead.*}}`, `{{system.*}}`

>[!BEGINSHADEBOX]

**Prerequisites**

- The application (AJO, Marketo) and GenStudio for Performance Marketing must belong to the same IMS Org for integration
- Users must have the "Collaborator" role (the lowest level) or higher

>[!ENDSHADEBOX]

Next, [customize your template](/help/user-guide/templates/customize-template.md) with placeholders to indicate where GenStudio for Performance Marketing should generate content for you. [Add your template](#add-a-template) to the [!DNL Content] repository and validate the template. Make any minor corrections using the code editor.
