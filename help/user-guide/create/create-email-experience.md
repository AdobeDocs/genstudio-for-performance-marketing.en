---
title: Create an email experience
description: Learn how to create email experiences in Adobe GenStudio for Performance Marketing.
feature: Content, Brands Service, Guidelines, Content Generation, Create, Experiences, Variant Generation
role: User
level: Beginner
recommendations: noDisplay
exl-id: 34446202-da98-45ff-869a-b43496a477f8
---
# Create an email experience

This tutorial demonstrates how to generate branded [email experiences](/help/user-guide/create/email-experiences.md) using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon in the left navigation area).

To create an effective email experience, it is recommended that you [add guidelines to GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) and brush up on the [basics of crafting a prompt](/help/user-guide/effective-prompts.md) before you begin.

## Choose a template

To create a new email experience, use an available template to provide the framework for your content.

**To choose an email template**:

1. In _[!DNL Create]_, click **[!UICONTROL Email]** in the _"What do you want to create today?"_ section.
1. Use the search option, adjacent to _Filter_, to find a specific email template.
1. Click to select an email template and click **[!UICONTROL Use]**.

   The Canvas, the epicenter of content creation, appears.

## Add parameters

Adding [guidelines](/help/user-guide/guidelines/overview.md) and assets in _Parameters_ in the prompt drawer supercharges the content generation process and is an integral preparatory step for generating an email experience.

**To add parameters and assets**:

1. Click the _Parameters_ icon to expand the prompt drawer.
1. In the _Parameters_ section, select guidelines—[!DNL Brands], [!DNL Personas], and [!DNL Products]—to inform content creation.

   ![Choose persona](/help/assets/persona-select.png){width="600" zoomable="yes"}

   If there are no brands, personas, or products available from these menus, [add guidelines to your GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Add content for use in the experience *and* to influence content generation:
   * Click **[!UICONTROL Select from Content]** to select assets (images) from your [!DNL Content] repository, filter and select one or more images.

      ![Choose visual content](/help/assets/content-select-email.png){width="500" zoomable="yes"}

      To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ dropdown menu. Filter and select one or more images.

   * Or, drag and drop assets into the **[!UICONTROL Select from Content]** section to upload one or more new assets.
1. Click **[!UICONTROL Use]**.

>[!NOTE]
>If your email template has multiple sections, select [!DNL Products] and content (visual assets) for each email section in _Multi-section emails_. Multi-section emails support one visual asset per section. You can only add visual assets to multi-section emails from [!DNL Content]—you cannot drag and drop or upload assets from your local source.
>![Add content and parameters for each email section](/help/assets/parameters-multisection-email.png){width="450" zoomable="yes"}

When you are finished adding parameters, you can collapse the prompt drawer by clicking the _Parameters_ icon again.

## Enter a prompt

After guidelines are selected, craft a prompt using natural language to start generating content for your new email experience. Detailed prompts yield higher quality output than vague or ambiguous prompts.

See [Write effective prompts](/help/user-guide/effective-prompts.md) to learn more about writing prompts.

**To enter a prompt**:

1. Enter a prompt in the _"Describe the experiences you want to generate"_ prompt box.
1. Click **[!UICONTROL Generate]**.

By default, four variations—all fueled by the prompt, guidelines, and content you added—are generated and shown in the Canvas.

Generated content loads progressively—as each section of the email experiences are generated they appear in the Canvas. See [Email experiences](/help/user-guide/create/meta-experiences.md#progressive-loading) to learn how those changes are loaded in the Canvas.

## Revise generated emails

Before selecting what to send for approval or publishing to [!DNL Content] you can edit email sections or delete a variant from the set of generated emails.

**To revise generated variants**:

* **To [edit the email draft name](/help/user-guide/create/manage-variants.md#change-draft-name)**, click into the _Untitled Draft_ title at the top of the Canvas and enter a new title.
* **To [manually edit an email](/help/user-guide/create/manage-variants.md#manually-edit-text)**, click into any of the editable text fields (such as the subject line, header, or body copy) and edit as needed
* **To [change or select the Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action)**, click the call-to-action button and select _[!UICONTROL Rephrase]_ or _[!UICONTROL Add link]_.
* **To [regenerate a section of a variant](/help/user-guide/create/manage-variants.md#re-generate-sections)**, click an editable text field and use the _[!UICONTROL Suggested edits]_ options or enter a new prompt and click **[!UICONTROL Generate]**.
* **To [add or swap images in a variant](/help/user-guide/create/manage-variants.md#swap-image)**, click an image asset (or the image asset area if an image does not currently exist) and click **[!UICONTROL Select/swap from content]** or **[!UICONTROL Upload New Image]** to add or swap an image in an individual variant.
* **To [delete an email](/help/user-guide/create/manage-variants.md#delete-variant)**, click to select the email title (for example, "Email 1/4") and click **[!UICONTROL Delete variant]**.

## Submit generation feedback

To [submit feedback](/help/user-guide/create/manage-variants.md#generation-feedback) about the quality of the generation output, click the options icon (three dots) and select **[!UICONTROL Good output]** or **[!UICONTROL Poor output]**.

## Preview for device

When revising and preparing email experiences, you can [toggle between previews for desktop and mobile views](/help/user-guide/create/manage-variants.md#preview-for-device) to ensure coherence and visual appeal of draft variants.

## Verify brand alignment

To optimize the generated emails and ensure strict adherence to brand identity, leverage the power of the [_Brand guidelines check_](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check)—providing a summary of brand alignment for a variant—and the [_Brand validation_ panel](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel)—displaying comprehensive brand validation details and illuminating improvement areas.

**To verify brand alignment**:

1. Click the [**[!UICONTROL [!DNL Brand] guidelines check]**](/help/user-guide/guidelines/brand-validation.md#brand-guidelines-check) icon for a variant and see a summary of how that variant performs when checked against your brand.

   ![Brand guidelines check](/help/assets/brand-guidelines-check.png){width="350" zoomable="yes"}

1. To get the details of the sections and guidelines that need improvement, click **[!UICONTROL Review]** _or_ click the [_Brand validation panel_](/help/user-guide/guidelines/brand-validation.md#brand-validation-panel) in the right action bar.

1. Toggle through each email to see how you can improve the generated content to be more brand-aligned.

   ![Brand validation panel](/help/assets/brand-validation-panel.png){width="600" zoomable="yes"}

1. [Manually revise emails](#revise-generated-emails) to ensure your emails are closely aligned with your brand.

See [Brand validation](/help/user-guide/guidelines/brand-validation.md).

## Get reviews and approvals

Use the Approvals panel, accessible as an icon on the right action bar of the Canvas, to obtain reviews, track review comments, and get approvals from stakeholders.

**To obtain reviews and approvals**:

1. [Launch an approval request](/help/user-guide/approvals/request-review.md) to solicit an [approval of drafted email experiences](/help/user-guide/approvals/approve-content.md).
1. [Remove or add reviewers](/help/user-guide/approvals/review-and-edit.md#manage-approvals) during the review process.
1. [Access the content for review](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) and view the requests for revision.
1. Edit the drafts per review comments and [publish your email experiences](#publish-and-export-experience).

See [Reviews and approvals](/help/user-guide/approvals/overview.md) for more information.

## Publish and export experience

To make the generated emails available for current and future use, publish it to [!UICONTROL Content] and export it for use in your marketing campaigns.

1. **To publish your new email experience(s)**, click **[!UICONTROL Publish]** in the top toolbar, or within the approvals flow.
1. **To export your new email experience(s)**, click **[!UICONTROL Export]** in the top toolbar.
   1. Select the format—CSV and images or HTML only—and click **[!UICONTROL Export]**.

See [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) for more information.
