---
title: Generate Image Variants
description: Create an an image, matching the style of a reference image, in Adobe [!DNL GenStudio] for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
badgeBeta: label="Beta" tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."
role: User
level: Beginner
recommendations: noDisplay
exl-id: c1118ada-7fee-43cd-aff4-eab69539afb4
TQID: https://experienceleague.adobe.com/NXtN00EKTe0lGI8jJMJWJfWx6mHoMQI1of1mJhgrR5U
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
    internal-label: Generative AI
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
subfeature_v2:
  - id: be495d08-ecd1-455f-951e-c22de504e667
    internal-label: Content generation
  - id: de1f9646-abd3-4e21-9de2-df62ce55c8dc
    internal-label: Create prompt
  - id: dee4e9a9-78d1-4953-8179-f8da6117027d
    internal-label: Create canvas
  - id: e4a0febc-5163-4017-82ce-fc7594509fb6
    internal-label: Generate images
  - id: f54ee13b-9545-4d68-9842-a12026e60aaf
    internal-label: Variant generation
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
    internal-label: Accessibility
---
# Generate image variants

With using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon), you can generate _[!DNL Image variants]_—generated assets that draw inspiration from a chosen image, capturing its visual impact and overall aesthetic.<!-- [two types of images](#image-types) using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon)—_[!DNL Image variants]_ and _[!DNL Similar images]_. -->

To design an eye-catching and effective image, it is recommended that you [add guidelines to GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) and review the [basics of writing prompts](/help/user-guide/effective-prompts.md).

## Image types

_[!DNL Image variants]_ are generated assets that draw inspiration from a chosen image, capturing its visual impact and overall aesthetic. These images are created using images already available in [!DNL Content] and a carefully crafted prompt that guides the design. They strictly follow both the brand guidelines and parameters chosen during the generation process.

_[!DNL Image variants]_ <!-- and _[!DNL Similar images]_ --> incorporate set guidelines, parameters, and a [thoughtfully-crafted prompt](/help/user-guide/effective-prompts.md) to deliver eye-catching image assets.

<!-- * _[!DNL Similar images]_—Image assets created with strong similarity to an existing selected image available in [!DNL Content]. When generating similar images, GenStudio for Performance Marketing redesigns the selected image, giving slight variations on the content to provide variety and nuance. -->

## Generate image variants

You can generate [!DNL Image variants] using defined guidelines, parameters, and a selected reference image. These elements, along with your prompt, guide the generation of consistent [!DNL Image variants].

### Choose a reference image

To create _[!DNL Image variants]_, select an existing image saved in [!DNL Content]. See [Best practices for templates](/help/user-guide/templates/best-practices-for-templates.md#follow-channel-specific-template-guidelines) for information about supported image dimensions.

**To choose a reference image**:

1. In _[!DNL Create]_, click **[!UICONTROL Generate image variants]**.
![Generate image variants](./gen-image-variants.png){width="400" zoomable="yes"}
1. Use the search option, adjacent to _Filter_, to find a specific image.

      ![Select reference image](/help/assets/select-img.png){width="400" zoomable="yes"}

   To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ drop-down menu. Filter and select one image.

1. In the _Select image_ view, click on an image.

   The selected image can be up to 10mb in size.

1. Click **[!UICONTROL Use]**.

   The Canvas, which serves as the central hub for content creation, is displayed.

### Add parameters

Incorporating [guidelines](/help/user-guide/guidelines/overview.md) and parameters enhances the content generation process and is a crucial preparatory step for producing [!DNL Image variants].

**To add guidelines and parameters**:

1. In the _Basic_ tab, select a [!DNL Brand] to inform content creation.

   If there are no brands available from this menu, [add guidelines to your GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Select an image category that best fits your desired result from _[!UICONTROL Image category]_.

   Image categories are available if a [!DNL Brand] was selected. The options are determined by the selected [!DNL Brand].

<!-- 
1. _(Optional)_ Select a custom model from _[!UICONTROL Model]_.

   Models are available if you access to [custom models in Firefly](https://adobedx.slack.com/archives/CMF1JGMLY/p1743534402774569). The _Models_ list will be blank if you do not have access. 
-->

1. Select the desired aspect ratio from _[!UICONTROL Aspect ratio]_.
1. Click **[!UICONTROL Select from Content]** in _[!UICONTROL Style reference]_ to add a reference image. The image you select influences the visual aesthetic and depth of the images you generate.

      To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ drop-down menu. Filter and select one image.

1. In the _Advanced_ tab, select the _Content type_.

   This is pre-selected based on the image category present for the selected [!DNL Brand]—_Art_ or _Photo_—and is uneditable.

1. Adjust the overall intensity of the image's existing visual characteristics in _[!UICONTROL Visual intensity]_.

### Enter a prompt

After selecting the parameters, craft a prompt using natural language to start generating image variants.

See [Write effective prompts](/help/user-guide/effective-prompts.md).

**To enter a prompt**:

1. Enter a prompt in the prompt box.
1. Click **[!UICONTROL Generate]**.

By default, four variations—fueled by the prompt, parameters, and content you added—are generated and shown in the Canvas.

### Edit in Adobe Express

After generating image variants, you can edit them directly in Adobe GenStudio for Performance Marketing using Adobe Express.

**To edit an individual image using Adobe Express**:

1. Hover over a generated image variant and click _[!UICONTROL Edit in Adobe Express]_.

   A _Powered by Adobe Express_ window appears.

1. Perform image editing, such as [cropping an image](https://helpx.adobe.com/express/create-and-edit-images/edit-images/crop-images.html), [removing an object](https://helpx.adobe.com/express/create-and-edit-images/create-and-modify-with-generative-ai/remove-objects-generative-fill.html), and applying effects.

   See [Adobe Express documentation](https://helpx.adobe.com/express/user-guide.html) to learn how revise images in GenStudio for Performance Marketing with Adobe Express.

1. Click _[!UICONTROL Apply changes]_ to save your edits.
1. Continue editing individual image variants as desired and applying changes to save your progress.

### Verify content check alignment

To optimize the generated variants and ensure strict adherence to brand identity, platform guidelines, and accessibility standards, leverage the power of the [_Content check_ panel](/help/user-guide/guidelines/brand-validation.md#content-check-panel). This panel displays comprehensive content check details and illuminates improvement areas.

**To perform content checks**:

1. Click the _Content check_ panel icon in the right action bar to open the [_Content check_ panel](/help/user-guide/guidelines/brand-validation.md#content-check-panel). View a summary of the *Needs review* and *Passed* checks to see which sections and guidelines need improvement.

   ![_Content check_ panel](/help/assets/content-check-img.png){width="500" zoomable="yes"}

1. Revise image variants to ensure your variants are closely aligned with the performed content checks.

See [Brand validation](/help/user-guide/guidelines/brand-validation.md).

<!-- 
## Generate Similar images

You can quickly generate images similar to a selected image within [!DNL Content] from the [!DNL Create] home.

**To create _[!DNL Similar images]_**:

1. In _[!DNL Create]_, click **[!UICONTROL Similar images]**.
1. Use the search option, adjacent to _Filter_, to find a specific image.

   To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ drop-down menu. Filter and select one image.

1. In the _Select image_ view, click on an image.
1. Click **[!UICONTROL Use]**.

   The Canvas, which serves as the central hub for content creation, is displayed. Four image variations similar to the original selected image appear.

   ![Generate similar images](/help/assets/generate-similar.png){width="400" zoomable="yes"} 
-->

## Publish and export images

Generated image drafts are shown in the _Recents_ section of the [!DNL Create] home.

To make the generated images available for current and future use, publish them to [!UICONTROL Content] and export it for use in your marketing campaigns.

1. **To publish your new images**, click **[!UICONTROL Publish]** in the top toolbar.
   1. _[!UICONTROL Add details]_, such as _[!UICONTROL Campaigns]_ or _[!UICONTROL Channels]_, if desired.
   1. Click **[!UICONTROL Publish]**.

1. **To export your new images**, click **[!UICONTROL Export]** in the top toolbar.
   1. Select the format—JPG or PNG—and click **[!UICONTROL Export]**.

See [[!DNL Content]](/help/user-guide/content/overview.md#search-and-find-approved-content).
