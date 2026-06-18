---
title: Translate and Localize Experiences
description: Learn how to translate approved email and paid media experiences into multiple languages on the HTML canvas in Adobe GenStudio for Performance Marketing.
feature: Create Canvas, Content Generation
role: User
level: Beginner
---
# Translate and localize experiences

Adobe [!DNL GenStudio for Performance Marketing] offers out-of-the-box translation on the HTML canvas so global and regional marketers can scale approved experiences into multiple languages without external translation tools.

The feature uses Azure Open AI by default. Your organization can also connect a preferred translation service through [translation extensions](/help/extensibility/deploy-app.md#find-translation-extensions).

Translation starts from an approved experience saved in [!DNL Content]. The source experience can be in any language. Each translated variant opens on the [!DNL Create] canvas as an editable draft that you can export, send for review, and publish as a separate experience.

## Supported experiences

Out-of-the-box translation on the HTML canvas supports:

* [Email experiences](/help/user-guide/create/email-experiences.md)
* Paid media experiences, including [Meta](/help/user-guide/create/meta-experiences.md), [LinkedIn](/help/user-guide/create/linkedin-experiences.md), and [Display](/help/user-guide/create/display-ad-experiences.md) ads

## Before you begin

Confirm that the experience you want to translate is **approved** and available in the [!DNL Content] _[!UICONTROL Experiences]_ gallery. Draft or in-review experiences are not eligible translation sources.

If your organization registers a custom translation extension, GenStudio for Performance Marketing uses that service instead of the default Azure Open AI translation. See [Find translation extensions](/help/extensibility/deploy-app.md#find-translation-extensions).

## Translate from [!DNL Create] {#translate-from-create}

Start a translation from the [!DNL Create] landing page to localize an approved experience.

![Translate and localize copy on the Create landing page](./translate-create-workflow.png){width="600" zoomable="yes"}

**To translate from [!DNL Create]**:

1. In [!DNL Create], scroll to the _Content creation_ section.
1. Click **[!UICONTROL Translate & localize copy]**.
1. Select the approved email or paid media experience that you want to translate. Click the **[!UICONTROL Use]** button.
1. Select target languages from the list of supported languages. Click **[!UICONTROL Translate]**.

Translated variants appear on the canvas. 

## Translate from [!DNL Content] {#translate-from-content}

You can also start translation from [!DNL Content] when you are browsing approved experiences.

### From the Experiences gallery

![Translate action on an experience in the Content gallery](./translate-content-gallery.png){width="500" zoomable="yes"}

**To translate from the Experiences gallery**:

1. In [!DNL Content], open the **[!UICONTROL Experiences]** tab.
1. Locate the approved experience that you want to translate.
1. Click the options (three dots) menu on the experience card.
1. Click **[!UICONTROL Translate]**.
1. Select target languages from the list of supported languages. Click **[!UICONTROL Translate]**.

## Work with translations on the canvas

On the HTML canvas, the source experience cannot be edited because it is already approved. Email source experiences appear locked. You can edit text in translated variants directly on the canvas. See [Manage variants](/help/user-guide/create/manage-variants.md) for guidance on editing variant copy.

Translated experiences do not run brand validation or display a brand score. The source experience was already created with brand guidelines, reviewed, and approved.

Fragment regeneration is not supported for translated experiences.

### Delete a translated language

**To remove a translated language from the canvas**:

1. On the [!DNL Create] canvas, click the options (three dots) menu on the translated variant header.
1. Click **[!UICONTROL Delete]**.

![Delete a translated language from the canvas](./remove-translation-variant.png){width="500" zoomable="yes"}

   The translated language is removed from the canvas.

### Refresh a paid media translation

After you edit translated paid media copy, you can reload the original translation output.

**To refresh a paid media translation**:

1. On the [!DNL Create] canvas, open the options menu on the edited translated variant.
1. Click **[!UICONTROL Refresh translation]**.

>[!NOTE]
>
>Refresh translation is available for paid media experiences. Email translation does not support refresh translation at this time.

## Export, review, and publish

After translations load on the canvas, you can export them, send them for approval, and publish approved variants to [!DNL Content].

**To export translated experiences**:

1. On the [!DNL Create] canvas, click **[!UICONTROL Export]** in the toolbar.
1. Select an export format.
   * Email: **CSV and images** or **HTML only**
   * Paid media: **CSV + JPG**, **CSV + PNG**, or **HTML + images**
1. Click **[!UICONTROL Export]**.

You can also [export experiences from [!DNL Content]](/help/user-guide/content/manage-assets.md#export-experiences).

**To request review and approval**:

1. On the [!DNL Create] canvas, click **[!UICONTROL Request approval]**.
1. Assign at least one approver and send the request.

See [Request review and approval](/help/user-guide/approvals/request-review.md) for details on the review workflow.

**To publish approved translations**:

1. After approvers approve the translated variants, click **[!UICONTROL Publish]**.
1. In the publish window, confirm metadata such as campaign name, timeframes, regions, and keywords.

See [Publish approved content](/help/user-guide/approvals/publish-content.md).

Each published translation is saved to [!DNL Content] as a separate experience.

## Translated experience metadata

Published translations include metadata that links each variant back to its source, including:

* **Title** — follows the pattern `Translation from "<source title>" <channel>`, such as `Translation from "Summer campaign" Meta`
* **Created by** — the user who initiated the translation
* **Created date** — the date of the translation
* **Translated source** — a link to the source experience in [!DNL Content]
* **Translated from** — the source language

## Limitations

Keep the following constraints in mind when you translate experiences on the HTML canvas:

* The source experience must already be approved and saved in [!DNL Content].
* Brand validation does not run on translated variants.
* Fragment regeneration is not supported on translated experiences.
* Refresh translation is available for paid media only.

## Related information

* [Email experiences](/help/user-guide/create/email-experiences.md)
* [Meta experiences](/help/user-guide/create/meta-experiences.md)
* [Display ad experiences](/help/user-guide/create/display-ad-experiences.md)
* [Manage assets and experiences](/help/user-guide/content/manage-assets.md)
* [Find translation extensions](/help/extensibility/deploy-app.md#find-translation-extensions)
