---
title: Create a LinkedIn Experience
description: Learn how to create brand-compliant LinkedIn experiences with Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
role: User
level: Beginner
badgeBeta: label="Beta" tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."
recommendations: noDisplay
exl-id: abe10fc8-d6d5-4cad-9273-400b622f22b7
---
# Create a LinkedIn experience

This tutorial demonstrates how to generate [LinkedIn experiences](/help/user-guide/create/meta-experiences.md) that adhere to your brand guidelines using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon in the left navigation area).

Before you begin generating a LinkedIn ad, it is important to [add guidelines](/help/user-guide/guidelines/add-guidelines.md) in GenStudio for Performance Marketing and learn the basics of [creating a prompt](/help/user-guide/effective-prompts.md).

## Choose a template

To generate a new LinkedIn experience, you need a template to provide the framework for your content. See [LinkedIn template guidelines](/help/user-guide/templates/linkedin-template.md) for information about supported LinkedIn aspect ratios.

You can select from your list of custom templates or choose a starter template.

**To choose a LinkedIn template**:

1. In _[!DNL Create]_, click **[!UICONTROL LinkedIn]**.
1. Select **[!UICONTROL Custom templates]** to browse your uploaded templates or **[!UICONTROL Starter templates]** to browse the pre-built templates.

      If you plan to add video assets to your Meta variants, you must choose a starter template. They are preloaded with system-defined content areas that facilitate the use of videos.

1. Click to select a template, and click **[!UICONTROL Use]**.

   This action opens the Canvas, which is the central hub for content creation.

## Add parameters

Adding [guidelines](/help/user-guide/guidelines/overview.md) and assets in _Parameters_ in the prompt drawer enhances the content generation process and is a crucial step in preparing to generate a LinkedIn experience.

**To add parameters and assets**:

1. Click the _Parameters_ icon to expand the prompt drawer.
1. In the _Parameters_ section, select guidelines—[!DNL Brands], [!DNL Personas], and [!DNL Products]—to inform content creation.

   ![Choose persona](/help/assets/persona-select-linkedin2.png){width="60%" align="center"}

   If there are no brands, personas, or products available from these menus, [add guidelines to your GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Add content (images or videos) for use in the experience *and* to influence content generation by clicking **[!UICONTROL Select from Content]**. Or, drag and drop images into the **[!UICONTROL Select from Content]** section to upload one or more new assets.

   Use the filter to search for content and select one or more images.

   If you are using a template that has a section for videos, video content (.mp4) will be pre-selected and filtered for you. Hover over a video to see an autoplayed preview.

   ![Choose visual content](/help/assets/content-select-meta.png){width="500" zoomable="yes"}

   To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ dropdown menu. Filter and select one or more images.

1. Click **[!UICONTROL Use]**.

When you are done adding parameters, you can collapse the prompt drawer by clicking the _Parameters_ icon again.

## Enter a prompt

After you select guidelines, craft a prompt using natural language to start generating content for your new LinkedIn experience. Detailed prompts ensure you receive good quality and useful output.

See [Write effective prompts](/help/user-guide/effective-prompts.md) to learn more about writing prompts.

**To enter a prompt**:

1. Enter a prompt in the _"Describe the experiences you want to generate"_ prompt box.
1. Click **[!UICONTROL Generate]**.

   See [Manage videos](#manage-videos) to understand how they are generated and how to manage them.

By default, four variations—all fueled by the prompt, guidelines, and content you added—are generated and shown in the Canvas.

Generated content loads progressively—as each section of the LinkedIn experiences are generated, they appear in the Canvas. See [LinkedIn experiences](/help/user-guide/create/linkedin-experiences.md#progressive-loading) to learn how those changes are loaded in the Canvas.

## Revise generated LinkedIn ads

Before sending variants for approval or publishing to [!DNL Content], you can edit the LinkedIn ads or delete a variant from the set of generated ads.

**To revise generated variants**:

* **To [edit the LinkedIn ad draft name](/help/user-guide/create/manage-variants.md#change-draft-name)**, click into the _Untitled Draft_ title at the top of the Canvas and enter a new title.
* **To [manually edit a LinkedIn ad](/help/user-guide/create/manage-variants.md#manually-edit-text)**, click into any of the ad sections (such as the subject line, header, or body copy) and edit as needed.
* **To change or select the call to action**, click the call-to-action button and select from the available button text options. In _Link_, enter a URL for the call-to-action text.
* **To [apply text formatting](/help/user-guide/create/manage-variants.md#manually-edit-text)** in a variant, click the on-image text for a variant and click **[!UICONTROL Format text]**.
* **To [regenerate a section of a variant](/help/user-guide/create/manage-variants.md#re-generate-sections)**, click an editable text field and use the _[!UICONTROL Suggested edits]_ options or enter a new prompt in the _[!UICONTROL Generate new text_ section] and click **[!UICONTROL Generate]**.
* **To [use Generative Expand to size and fit images](/help/user-guide/create/manage-variants.md#use-generative-expand) to your working template**, click an image, click **[!UICONTROL Edit]** (pencil icon) and then **[!UICONTROL Expand]**. Adjust the image to fit the needed aspect ratio and template.
* **To [crop or reposition images](/help/user-guide/create/manage-variants.md#crop-assets)**, hover over an image, click the crop icon that appears, and adjust the image size and placement.
* **To [change the size and aspect ratio of the ad](/help/user-guide/create/manage-variants.md#change-aspect-ratio)**, click the _[!UICONTROL Resize]_ button (box with a button icon on the left side of the Canvas) and select a new size and aspect ratio to apply to all variants. The variants are duplicated and resized.
* **To [add or swap assets (image or video) in a variant](/help/user-guide/create/manage-variants.md#swap-image)**, click an asset (or the asset area) and click the **[!UICONTROL Swap from content]** icon.
* **To [add alt text for images in a variant](/help/user-guide/create/manage-variants.md#add-alt-text-for-images)**, click an image asset and use the _Alt text_ option to manually add or generate alt text per image.
* **To [add accessibility labels](/help/user-guide/create/manage-variants.md#add-accessibility-labels) to your variants** click on an image or call-to-action link, then provide a brief description that explains what the link or button does.
* **To [delete a LinkedIn ad](/help/user-guide/create/manage-variants.md#delete-variant)**, click the options menu for a variant and click **[!UICONTROL Delete variant]**.

### Manage videos

Hover over each of the videos to see looped autoplay.

Videos are reframed to fit the selected aspect ratio during generation. Revert back to the original non-reframed video by clicking **[!UICONTROL Reframe Video]** and toggling it off.

## Submit generation feedback

To [submit feedback](/help/user-guide/create/manage-variants.md#generation-feedback) about the quality of the generation output, click the options icon (three dots) and select **[!UICONTROL Good output]** or **[!UICONTROL Poor output]**.

## Verify content check alignment

To optimize the generated variants and ensure strict adherence to brand identity, platform guidelines, and accessibility standards, leverage the power of the [_Content check_ panel](/help/user-guide/guidelines/brand-validation.md#content-check-panel). This panel displays comprehensive content check details and illuminates improvement areas.

**To perform content checks on a variant**:

1. Click the _Content check_ panel icon in the right action bar to open the [_Content check_ panel](/help/user-guide/guidelines/brand-validation.md#content-check-panel). View a summary of the *Needs review* and *Passed* checks to see which sections and guidelines need improvement.

   ![_Content check_ panel](/help/assets/content-check-panel.png){width="300"}

2. [Manually revise variants](#revise-generated-linkedin-ads) to ensure your variants are closely aligned with then completed content checks.

See [Brand validation](/help/user-guide/guidelines/brand-validation.md).

## Get reviews and approvals

Use the Approvals panel, accessible on the top menu bar of the Canvas, to obtain reviews, track review comments, and get approvals from stakeholders.

**To obtain reviews and approvals**:

1. [Launch an approval request](/help/user-guide/approvals/request-review.md) to solicit an [approval of drafted Meta ad experiences](/help/user-guide/approvals/approve-content.md).

   ![Send drafts for review and approval](/help/assets/send-approval-meta.png){width="450" zoomable="yes"}

1. [Remove or add reviewers](/help/user-guide/approvals/review-and-edit.md#manage-approvals) during the review process.
1. [Access the content for review](/help/user-guide/approvals/review-and-edit.md#access-content-for-review) and view the requests for revision.
1. Edit the drafts per review comments and [publish your Meta ad experiences](#publish-and-export-experience).

See [Reviews and approvals](/help/user-guide/approvals/overview.md) for more information.

## Publish and export experience

To make the generated LinkedIn ads available for current and future use, publish it to [!UICONTROL Content] and export it for use in your marketing campaigns.

1. **To publish your new experience(s)**, click **[!UICONTROL Publish]** in the top toolbar, or within the approvals flow.
1. **To export your new experience(s)**, click **[!UICONTROL Export]** in the top toolbar.
   1. Select the format—JPG, PNG, or GIF—and click **[!UICONTROL Export]**.

See [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content) for more information.
