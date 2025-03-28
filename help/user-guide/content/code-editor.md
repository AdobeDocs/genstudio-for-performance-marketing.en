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
