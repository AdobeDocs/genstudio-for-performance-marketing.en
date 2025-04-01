---
title: Create images
description: Create an an image, matching the style of a reference image or by quickly generating image variations, in Adobe [!DNL GenStudio] for Performance Marketing.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation, Custom Models
badgeBeta: label="Beta" tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."
role: User
level: Beginner
recommendations: noDisplay
---
# Create images

This tutorial demonstrates how to generate two types of images using GenStudio for Performance Marketing [[!DNL Create]](/help/user-guide/create/overview.md) (paintbrush icon in the left navigation area)—[on-brand images](images.md#on-brand-images) and [similar images](images.md#similar-images).

To design an eye-catching and effective images, it is recommended that you [add guidelines to GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md) and review the [basics of writing prompts](/help/user-guide/effective-prompts.md) before you begin.

## Generate on brand images

On brand images are created using defined guidelines, parameters, and a selected reference image. These elements, along with your prompt, guide the generation of consistent on-brand image variations.

### Choose a reference image

To create an on brand image, select an existing image saved in [!DNL Content]. See [Best practices for templates](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) for information about supported on brand image dimensions.

**To choose a reference image**:

1. In _[!DNL Create]_, click **[!UICONTROL On brand image]**.
1. Use the search option, adjacent to _Filter_, to find a specific image.
1. In the _Select image_ view, click on an image.
1. Click **[!UICONTROL Use]**.

   The Canvas, which serves as the central hub for content creation, is displayed.

### Add parameters

Incorporating [guidelines](/help/user-guide/guidelines/overview.md) and parameters enhances the content generation process and is a crucial preparatory step for producing an on brand image.

**To add guidelines and parameters**:

1. In the _Basic_ tab, select a [!DNL Brand] to inform content creation.

   If there are no brands available from this menu, [add guidelines to your GenStudio for Performance Marketing](/help/user-guide/guidelines/add-guidelines.md).

1. Select an image category that best fits your desired result from _[!UICONTROL Image category]_. These options are determined by the selected [!DNL Brand].
1. _(Optional)_ Select a custom model from _[!UICONTROL Model]_.

   Models are available if you access to [custom models in Firefly](https://adobedx.slack.com/archives/CMF1JGMLY/p1743534402774569). The _Models_ list will be blank if you do not have access.

1. Select the desired aspect ratio from _[!UICONTROL Aspect ratio]_.
1. Click **[!UICONTROL Select from Content]** in _[!UICONTROL Style reference]_ to add a reference image. The image you select influences the visual aesthetic and depth of the images you generate.

      To use assets from a connected [!DNL AEM Assets Content Hub] repository, choose a repository from the _Location_ dropdown menu. Filter and select one image.

1. In the _Advanced_ tab, select the _Content type_. If the brand you selected for image generation includes an image category guideline, the content type will be pre-selected with that guideline—Art or Photo—and is uneditable.
1. Adjust the overall intensity of the image's existing visual characteristics in _[!UICONTROL Visual intensity]_.

### Enter a prompt

After parameters are selected, craft a prompt using natural language to start generating on brand images.

See [Write effective prompts](/help/user-guide/effective-prompts.md) to learn more about writing prompts.

**To enter a prompt**:

1. Enter a prompt in the prompt box.
1. Click **[!UICONTROL Generate]**.

By default, four variations—fueled by the prompt, parameters, and content you added—are generated and shown in the Canvas.

## Generate similar images

