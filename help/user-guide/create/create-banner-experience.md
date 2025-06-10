---
title: Create a banner experience
description: Learn how to create banner experiences in Adobe [!DNL GenStudio] for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."
role: User
level: Beginner
recommendations: noDisplay
exl-id: c5d541a9-a97b-44da-a15c-61aceefd0e8c
---
# Create a banner experience

This tutorial shows you how to create branded [banner experiences](banner-experiences.md) using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon in the left navigation area).

To design an engaging banner experience, it is recommended to [add guidelines to GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) and review the [basics of writing prompts](/help/user-guide/effective-prompts.md) before getting started.

## Choose a template

To create a banner experience, use an available template to provide the framework for your content. See [Best practices for templates](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) for information about supported banner dimensions.

**To choose a banner template**:

1. In _[!DNL Create]_, click **[!UICONTROL Banners]**.
1. Use the search option, adjacent to _Filter_, to find a specific banner template.
1. In the _Select template_ view, click on a banner template.
1. Click **[!UICONTROL Use]**.

   The Canvas, which is home base for content creation, is displayed.

## Add parameters

Incorporating [guidelines](/help/user-guide/guidelines/overview.md) and assets into _Parameters_ within the prompt drawer enhances the content generation process and is a crucial preparatory step for creating a banner experience.

**To add parameters and assets**:

1. Click the _Parameters_ icon to expand the prompt drawer.
1. In the _Parameters_ section, select guidelines—[!DNL Brands], [!DNL Personas], and [!DNL Products]—to inform content creation.

   If there are no brands, personas, or products available from these menus, [add guidelines to your GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. To add content to be used in the experience *and* to influence content generation:
   * Click **[!UICONTROL Select from Content]** to select assets (images) from your [!DNL Content] repository, filter and select one or more images.

      To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ dropdown menu. Filter and select one or more images.

   * Or, drag and drop assets into the **[!UICONTROL Select from Content]** section to upload one or more new assets.
1. Click **[!UICONTROL Use]**.

When you are finished adding parameters, collapse the prompt drawer by clicking the _Parameters_ icon again.

## Enter a prompt

Once you have selected the guidelines, use natural language to create a prompt to initiate the content generation for your new banner experience. To ensure high-quality results, it is essential to craft prompts that are detailed and descriptive.

![Enter a prompt](/help/assets/prompt-displayad.png){width="650" zoomable="yes"}

See [Write effective prompts](/help/user-guide/effective-prompts.md) to learn more about writing prompts.

**To enter a prompt**:

1. Enter a prompt in the _"Describe the experiences you want to generate"_ prompt box.
1. Click **[!UICONTROL Generate]**.

By default, four variations—fueled by the prompt, guidelines, and content you added—are generated and shown in the Canvas.

## Revise generated banners

Before selecting what to send for approval or publishing to [!DNL Content] you can edit banner sections and text fields, or delete a generated variant.

**To revise generated variants**:

* **To [edit the banner draft name](/help/user-guide/create/manage-variants.md#change-draft-name)**, click into the _Untitled Draft_ title at the top of the Canvas and enter a new title.
* **To [manually edit a banner](/help/user-guide/create/manage-variants.md#manually-edit-text)**, double-click into any of the banner sections or fields (such as the headline or CTA) and edit as needed.
* **To [regenerate a section of a variant](/help/user-guide/create/manage-variants.md#re-generate-sections)**, click an editable text field and use the _[!UICONTROL Suggested edits]_ options or enter a new prompt in the _[!UICONTROL Generate new text_ section] and click **[!UICONTROL Generate]**.
* **To [add or swap images in a variant](/help/user-guide/create/manage-variants.md#swap-image)**, click an image asset (or the image asset area if an image does not currently exist) and click the **[!UICONTROL Swap from content]** icon.
* **To [add a link to an image in a variant](/help/user-guide/create/manage-variants.md#add-image-link)**, click an image asset (or the image asset area if an image does not currently exist) and click the link icon.
* **To [add alt text for images in a variant](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**, click an image asset and use the _Alt text_ option to manually add or generate alt text per image.
* **To [change the size and aspect ratio of the ad](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, click the _[!UICONTROL Resize]_ button (box with a button icon on the left side of the Canvas) and select a new size and aspect ratio to apply to all variants. The variants are duplicated and resized.
* **To [crop or reposition images](/help/user-guide/create/manage-variants.md#crop-assets)**, click an image, click **[!UICONTROL Edit]** (pencil icon) and then **[!UICONTROL Crop]**. Adjust the image size and placement.
* **To [use Generative Expand to size and fit images](/help/user-guide/create/manage-variants.md#use-generative-expand) to your working template**, click an image, click **[!UICONTROL Edit]** (pencil icon) and then **[!UICONTROL Expand]**. Adjust the image to fit the needed aspect ratio and template.

<!-- # Preview for device
When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.
**To preview variants for desktop and mobile devices** toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear. -->

## Submit generation feedback

To [submit feedback](/help/user-guide/create/manage-variants.md#generation-feedback) about the quality of the generation output, click the options icon (three dots) and select **[!UICONTROL Good output]** or **[!UICONTROL Poor output]**.

## Verify content check alignment

To optimize the generated variants and ensure strict adherence to brand identity, platform guidelines, and accessibility standards, leverage the power of the [_Content check_ panel](/help/user-guide/guidelines/brand-validation.md#content-check-panel). This panel displays comprehensive content check details and illuminates improvement areas.

**To perform content checks on a variant**:

1. Click the _Content check_ panel icon in the right action bar to open the [_Content check_ panel](/help/user-guide/guidelines/brand-validation.md#content-check-panel). View a summary of the _Needs review_ and _Passed_ checks to see which sections and guidelines need improvement.

   ![_Content check_ panel](/help/assets/content-check-panel.png){height="400" zoomable="yes"}

1. [Manually revise variants](#revise-generated-variants) to ensure your variants are closely aligned with the performed content checks.

See [Brand validation](/help/user-guide/guidelines/brand-validation.md).

## Get reviews and approvals

Use the _Approvals_ panel, accessible as an icon on the right action bar of the Canvas, to obtain reviews, track review comments, and get approvals from stakeholders.

**To obtain reviews and approvals**:

1. [Launch an approval request](/help/user-guide/approvals/request-review.md) to solicit an [approval of drafted banner experiences](/help/user-guide/approvals/approve-content.md).
1. [Remove or add reviewers](/help/user-guide/approvals/review-and-edit.md#manage-approvals) during the review process.
1. [Access the content for review](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) and view the requests for revision.
1. Edit the drafts per review comments and [publish your banner experiences](#publish-and-export-experience).

See [Reviews and approvals](/help/user-guide/approvals/overview.md).

## Publish and export experience

To make the generated banners available for current and future use, publish it to [!UICONTROL Content] and export it for use in your marketing campaigns.

1. **To publish your new banner experiences**, click **[!UICONTROL Publish]** in the top toolbar, or within the approvals flow.
   1. Select _[!UICONTROL [!DNL Campaigns]]_ and add _[!UICONTROL More details]_ if desired.
   1. Click **[!UICONTROL Publish]**.

      ![Publish a banner](/help/assets/publish-displayad.png){width="450" zoomable="yes"}

1. **To export your new banners**, click **[!UICONTROL Export]** in the top toolbar.
   1. Select the format—HTML and images, PNG, or JPG—and click **[!UICONTROL Export]**.

      Exported HTML should be placed within a predefined web property, like a template or `div` container. Without these set dimensions, images may appear distorted when viewed independently.

See [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
