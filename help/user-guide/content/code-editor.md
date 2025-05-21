---
title: Template code editor
description: Learn how to use the template code editor in GenStudio for Performance Marketing.
level: Intermediate
role: Developer
feature: Media Templates, Content Generation
exl-id: b46fc7a9-88c1-474a-9d7b-1df7740d8f5a
---
# Template code editor

The template code editor is designed to help you verify and refine your template for optimal use when generating new experiences with GenStudio for Performance Marketing. The editor supports the Handlebars syntax, which uses placeholders within the template to indicate where GenStudio for Performance Marketing should generate content for you.

>[!TIP]
>
>Before uploading your template HTML code in the [!DNL Content] _Templates_ view, prepare your template by inserting content placeholders defined in the [Customize templates](customize-template.md) guidance.

## Check detected fields

The _[!UICONTROL Check detected fields]_ pane shows a list of fields that GenStudio for Performance Marketing recognizes in your template. Review the list, and you can scroll through the HTML code to look at the formation of your template.

![Code editor view](/help/assets/template-detected-fields.png "Check detected fields"){width="600" zoomable="yes"}

If you notice that a field is missing from the list, search your template code and find the location for the missing field. Insert the correct placeholder using the Handlebars syntax and a [recognized field name](/help/user-guide/content/customize-template.md#recognized-field-names). Use the Find and Replace form, which appears at the bottom of the code editor, to search for specific strings in the code. (Windows `CTRL`+`F` or macOS `CMD`+`F`)

### Make a correction

If there are errors in your template, you may see a `Template is invalid` message that includes a brief explanation of the issue. In the following example, the message indicates that the `_image` field does not conform to the field naming convention established in the multi-pod template. The message further advises that you need to update the field name with the correct prefix. Find the `_image` field in the template code editor, and update the name as advised.

![Correct invalid template](/help/assets/animation/template-code-editor.gif){width="600" zoomable="yes"}

The _[!UICONTROL Check detected fields]_ pane updates to reflect the changes that you made. Once you are satisfied that the fields are correct and complete, click **[!UICONTROL Next]** to continue [uploading your template](/help/user-guide/content/use-templates.md#add-a-template).

## Common template issues and solutions

| **Error**                   | **Description**                                                                 | **Solution**                                                                                   |
|-----------------------------|---------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| Failed to parse             | The template content could not be parsed as valid Handlebars.                   | Check your template for HTML and Handlebars syntax errors and correct them to ensure valid formatting for [content placeholders](/help/user-guide/content/customize-template.md#content-placeholders). |
| Group not assigned          | An image field in a multi-group email template is not assigned to any group.    | Check for consistent use of section prefixes. Each [section](/help/user-guide/content/customize-template.md#sections-or-groups) can use only one of each field type (`headline`, `body`, `image` `cta`). Assign the `image` field to a valid group in your template. |
| Image missing               | A required image field is missing.                                              | Exactly one `image` field is required for certain template types, such as a Meta, display, or banner ad. Add the required `image` field to your template. |
| Invalid single group        | The email template contains exactly one group, which is invalid.                | A basic email template contains a single set of template elements, which do not require the group naming convention as defined in [Sections or groups](/help/user-guide/content/customize-template.md#sections-or-groups). Adjust your template to have zero sections by removing any group naming syntax. |
| No fields                   | The template does not contain any fields.                                       | Add [recognized field names](/help/user-guide/content/customize-template.md#recognized-field-names) using the Handlebars syntax to your template where you need GenStudio for Performance Marketing to generate a certain type of content. |
| Required properties missing | Some required metadata properties are missing.                                  | Each template type has requirements and constraints based on the channel guidelines. For example, Meta requires an aspect ratio, and display ads require dimensions. [Follow channel-specific template guidelines](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines).  |
| Reserved name used          | A prohibited or reserved field name is being used.                              | Certain [field names](/help/user-guide/content/customize-template.md#recognized-field-names), such as `subject` or `introductory_text`, are reserved. Rename fields that use reserved or prohibited names. |
| Too many fields             | The number of fields exceeds the global limit of 20.                            | Remove unnecessary fields to ensure that the total does not exceed 20. |
| Too many groups             | The number of groups exceeds the channel's allowed maximum.                     | Meta, display, and LinkedIn templates do not allow multiple sections. Email only requires group naming when defining two or three sections. Reduce the number of groups in your template to meet the [channel's requirements](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines). |
| Unsupported field           | The template is using a field that the channel does not support.                | Replace or remove unsupported fields according to the [recognized field names](/help/user-guide/content/customize-template.md#recognized-field-names). |
