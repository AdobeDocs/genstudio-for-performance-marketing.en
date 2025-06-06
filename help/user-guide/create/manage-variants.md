---
title: Manage variants
description: Customize and enhance generated variants and assets to suit your digital marketing needs.
feature: Create Canvas, Create Prompt, Generative AI, Variant Generation, Content Generation
exl-id: 06f495bb-feec-45fc-9ba6-e941f79e390c
---
# Manage variants

Adobe GenStudio for Performance Marketing [!DNL Create] enables you to customize and enhance generated variants—[emails](/help/user-guide/create/email-experiences.md), [Meta ads](/help/user-guide/create/meta-experiences.md), and more—for use in digital marketing initiatives.

When [creating experiences](/help/user-guide/create/overview.md), you can modify content and assets of generated variants individually or in a batch. The ability to manage variants at the individual micro level allows you to manage each piece of generated content.

## Change draft name

Generated variant drafts have a default name shown at the top of the Canvas. Default draft names use the following convention that includes the channel type, date, and time of generation.

*Example*: "Meta: Untitled Draft - 09.5.24, 9:56 AM"

**To change the default name**:

1. After generating a set of variants, click into the default _Untitled Draft_ name at the top of the Canvas.
1. Select text and enter a new name.
1. Click off the text field to save it.

## Manually edit text

You can edit the text fields in generated variants. Refine the text for your audience by experimenting with different phrases and verbiage. For example, you can manually revise text in variants to preview the appearance of a headline with a chosen image.

**To edit text manually in generated variants**:

1. After generating a set of variants, double-click editable text in a variant.
1. Enter new text.
1. Click off the text field to save it.

## View layers

You can quickly select an individual layer of a variant and make changes, such as re-generating sections or cropping images. When you select an individual layer, the editable fields or images within the layer are highlighted.

**To view the layers of a variant**:

1. After generating a set of variants, click an editable field or image within a variant.
1. Click _[!UICONTROL View Layers]_.
1. Click to select a layer from the list. The selected layer is highlighted for the variant.

   Proceed with making any necessary edits to the selected layer.

## Re-generate sections

GenStudio for Performance Marketing has the built-in functionality to regenerate sections of generated variants. You can rephrase, shorten, or lengthen text, or add fresh prompts to generate new content.

For example, you can re-generate the headline section of one Meta ad variant to see how it looks with a specific background asset. You can _[!UICONTROL Rephrase]_, _[!UICONTROL Shorten]_, or _[!UICONTROL Lengthen]_ a section's content, or _[!UICONTROL Generate new text]_ to add a new prompt.

![Re-generate sections](/help/assets/regenerate-sections.png){width="300" zoomable="yes"}

**To re-generate individual variant sections**:

1. After generating a set of variants, single-click any editable text in a variant.
1. To alter the existing text, select _[!UICONTROL Rephrase]_, _[!UICONTROL Shorten]_, or _[!UICONTROL Lengthen]_.
1. To generate new phrasing options, select _[!UICONTROL Generate new text]_ and enter a new prompt.
   1. Click **[!UICONTROL Generate]**.
1. As you are re-generating a section's text, click the regenerate icon (circling arrows) to see more text options.
1. From the results that appear, select the desired option and click **[!UICONTROL Replace]**.

   The variant is updated with the revised text.

## Revise Call to action

After generating a set of variants, you can revise the call-to-action (CTA) text and link.

>[!NOTE]
>
>You can edit CTA label text using the _[!UICONTROL Rephrase]_ option if the label text is a generated template field (not hard-coded in the template). You can edit a CTA link using the _[!UICONTROL Edit link]_ option if the link is existing and editable (not hard-coded in the template).

**To revise the CTA in a variant**:

1. Click a CTA button in one of the variants.

   The button is selected, displays the character count, and presents two options: _[!UICONTROL Rephrase]_ and _[!UICONTROL Add link]_.

1. Click **[!UICONTROL Rephrase]**.

   1. Choose from the list of regenerated phrases or click **[!UICONTROL Refresh results]** for more options.

   1. Click **[!UICONTROL Replace]**.

      The CTA text refreshes and a _"A button label was replaced"_ message appears confirming the change.

1. Click **[!UICONTROL Add link]**.

   1. Type or paste in a URL and click **[!UICONTROL Apply]**.
   
      To revise an existing link in your CTA, edit the existing URL or paste in a new URL and click **[!UICONTROL Apply]**.

The added or revised link is applied to all CTAs in the set of variants.

## Crop assets

You can manually crop and reposition image assets in individual generated variants.

**To crop and reposition images in variants**:

1. After generating a set of variants, hover over an image within a variant.
1. Click the crop icon that appears in the left corner of the image.
1. Adjust the image bounding box and drag the image into the desired position.
1. Click **[!UICONTROL Apply]** to apply the crop to a single image or **[!UICONTROL Apply to all images]** to apply to all images in the variants.

   The cropped image is saved and visible for the variants.

## Change aspect ratio

You can quickly change the [aspect ratio of Meta ads](/help/user-guide/templates/meta-template.md#supported-aspect-ratios) to accommodate the desired ad sizing. Choose an image aspect ratio that closely matches your template dimensions to avoid unwanted cropping or stretching. For example, if your template is 1200 × 628 pixels (a wide rectangle), using a 1:1 square image may crop the sides, potentially cutting off important content. The optimal image size would be 628 x 628 pixels, which matches the height of the template.

>[!NOTE]
>
>Varying aspect ratios and sizes may be available based on available templates.

**To change the aspect ratio of generated Meta ads**:

1. After generating a set of variants, select the aspect ratio resize icon (arrow pointing to box corner) on the left side of the Canvas.

   The aspect ratio that is currently used for your ads is shown in the top portion of the _[!UICONTROL Resize]_ window.

   The number of variations affected by this revision are noted in the top right corner of the window. _Example_: "4 of 4 variations"

1. Select an [available aspect ratio](/help/user-guide/templates/meta-template.md#supported-aspect-ratios).

   Only aspect ratio sizes that are not currently represented in the Canvas are available to choose.

1. Click **[!UICONTROL Duplicate and resize]**.

   [!DNL Create] builds a copy of each variant based on the new selected aspect ratio. All variants, including ones in the initial aspect ratio, are present in the Canvas.

   For instance, if you generate four variants in a 1:1 aspect ratio initially and then change the aspect ratio to 4:5, _eight_ total variants are now available on the Canvas.

## Swap image

You can add or swap images in generated variants right from the Canvas.

**To add or swap images in a variant**:

1. After generating a set of variants, click an image asset (or the image asset area if an image does not currently exist).
1. Click the **[!UICONTROL Swap from content]** icon.
1. Use the filters and search function in the GenStudio assets [!DNL Content] view to further narrow your search results.

   You can also use images available in connected Adobe Experience Manager (AEM) Assets Content Hub repositories by selecting that repository from the [**[!UICONTROL Location]** menu](/help/user-guide/content/manage-assets.md#location).

1. Click to select an image and click **[!UICONTROL Use]**.

   The image is added or swapped into the applicable variant.

## Add image link

Similar to adding or swapping images in generated variants, you can add a link to images. The template you used to generate variants _must_ contain a [content placeholder for the link](/help/user-guide/content/customize-template.md#content-placeholders) to enable this functionality.

**To add an image link in a variant**:

1. After generating a set of variants, click an image asset.

   If the variant does not currently have a placed image asset, click the image asset area.

1. Click the link icon.
1. Click **[!UICONTROL Remove link]** to remove the existing default link.
1. Add a link in the text field and click **[!UICONTROL Apply]**.

   The defined link is applied to all images in the variant set.

## Add alt text for images

When you add content (images) during the creation process, you can define alt text for every image included. Adding alt text to images improves accessibility, search engine optimization, and the user experience.

To enable alt text functionality, [add a content placeholder](/help/user-guide/content/customize-template.md#alternative-text) in the template.

**To add alt text to images in generated variants**:

1. After generating a set of variants, click an image within an individual variant.
1. Click the **[!UICONTROL Alt text]** button (icon of image and paper).
1. To manually add alt text:
   1. Click into the text box and add alt text.
   1. Click **[!UICONTROL Apply]**.
1. To generate alt text for the image:
   1. Leave the text field empty and click **[!UICONTROL Generate]**.
   1. Click **[!UICONTROL Generate]** again if you are not satisfied with the initial result.
   1. Click **[!UICONTROL Apply]**.
1. Repeat for each image in your variants set.

## Add Aria-labels

Provide an accessible name for image and call to action links in your variants by adding Aria-labels. Aria-labels supplement visible text to help users understand the purpose of the link or button.

**To add Aria-labels to image or call to action links in your variants**:

1. After generating a set of variants, click an image or call to action within a variant.
1. Click the **[!UICONTROL ARIA-label]** button.
1. Click into the text box and add a short description of what the link on the call to action button or image does. For instance, you could use "Shop at WKND's official site" for a call to action button link.
1. Click **[!UICONTROL Apply]**.

To enable Aria-label functionality, [add a content placeholder](/help/user-guide/content/customize-template.md) in the template.

## Preview for device

When revising and preparing email experiences, you can toggle between previews for desktop and mobile views to ensure coherence and visual appeal of draft variants.

**To preview variants for desktop and mobile devices**, toggle the device preview option—between **desktop** and **mobile**—in the right menu bar (computer and phone icons) to preview how variants appear.

## Delete variant

You can delete any generated variants that you do not plan to save or reuse.

Delete needless variants so that the working Canvas shows only the variants you are actively refining or using.

**To delete a generated variant**:

1. After generating a set of variants, click the options icon (three dots) above a variant.

   The variant is highlighted and a shortcut menu appears.

1. Select **[!UICONTROL Delete]** from the available options.

   The variant is deleted.

## Brand validation

Use the _Content check_ panel to maintain consistent brand identity, [ADA accessibility standards, platform guidelines](/help/user-guide/guidelines/overview.md#content-checks), and alignment of variants.

See [Brand validation](/help/user-guide/guidelines/brand-validation.md).

## Generation feedback

Feedback on the quality of generated brand-aligned assets can be submitted to improve the content generation process. Indicating whether the results are of high or poor quality helps enhance the overall content quality and user safety of GenStudio for Performance Marketing.

![Submit feedback on content generation](/help/assets/generation-feedback.png){width="500" zoomable="yes"}

Generation feedback is applicable to an individual variant, not for the collected set of variants.

**To submit generation feedback**:

1. After generating a set of variants, click the options icon (three dots) above a variant.

   The variant is highlighted and a shortcut menu appears.

1. Select **[!UICONTROL Good output]** or **[!UICONTROL Poor output]**.

   A feedback popup appears to collect further information. Generated content and prompt information is included in your feedback.

1. Add the following information in the feedback popup:
   1. Select the _[!UICONTROL Also include your reference content and layer data]_ option to include that extra reference information in the collected feedback.
   1. From the _[!UICONTROL What worked well?]_ or _[!UICONTROL What went wrong?]_ section, select the options that describe what makes the content generation high or poor quality.
   1. Add any other helpful or related information in the _[!UICONTROL Notes]_ field.
1. Click **[!UICONTROL Submit]**.

   A banner appears to confirm you submitted feedback.
