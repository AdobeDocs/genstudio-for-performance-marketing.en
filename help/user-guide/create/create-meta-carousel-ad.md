---
title: Create Meta Ad Experience - Carousel Ads
description: Learn how to create multi-card Meta carousel ad experiences, manage cards, and generate on-brand concepts in [!DNL GenStudio for Performance Marketing].
role: User
---

# Create a Meta carousel ad experience

A Meta carousel ad is a paid-ad format that shows two to ten swipeable cards, each with its own image or video, headline, and link.

This page covers the steps that are specific to carousel ads. For the shared steps that this page does not repeat, such as choosing a template, adding parameters, revising variants, and publishing, see [Create a Meta ad experience](/help/user-guide/create/create-meta-ad.md).

## Prerequisites

Before you create a carousel ad, make sure you have a template whose pages all share one aspect ratio, either 1:1 or 4:5. Each template page becomes one card. For more information, see [Meta ad template guidelines](/help/user-guide/templates/meta-template.md).

## Choose the carousel format

After you select a template and open the Canvas, choose the carousel format in the prompt drawer.

1. In the _[!DNL Create your ads]_ panel, expand _[!UICONTROL Parameters]_.
1. From the **[!UICONTROL Format]** dropdown menu, select **[!UICONTROL Carousel ad]**.

   ![The Create your ads panel with the Format dropdown set to Carousel ad and a list of cards](./carousel-format-cards.png){width="70%" zoomable="yes"}

If you start from a single-page template, [!DNL GenStudio for Performance Marketing] duplicates the page to meet the two-card minimum. If the template pages do not all share one aspect ratio, the format switch is blocked until you use a template with a consistent aspect ratio.

## Manage cards

Build the card set in the prompt drawer before you generate. To add more cards, duplicate an existing card.

* **To duplicate a card**, select **[!UICONTROL Duplicate]** from the card options.
* **To reorder cards**, drag a card by its handle to a new position.
* **To delete a card**, select **[!UICONTROL Delete]** from the card options. The last two cards cannot be deleted, because a carousel requires at least two cards.

For each card, select one image and, if needed, set a per-card product that overrides the parent product. You select one image per card individually. Per-card destination URLs are set later in [!DNL Activate]. For more information, see [Activate a Meta ad](/help/user-guide/activation/activate-meta-ad.md).

## Write a carousel prompt

Your prompt signals the intent of the carousel, so describe how the cards relate to each other. Carousel copy can follow one of two approaches:

* **Modular:** Each card is a self-contained ad, and no copy flows across cards. Use this approach for a set of related but independent messages, such as several products.
* **Sequential:** The copy connects across cards to tell a story, a step-by-step sequence, or a how-to. Use this approach when the cards build on one another.

You can also describe whether the carousel features a single product or multiple products, plus any per-card detail.

For example, this prompt describes a modular carousel that features multiple products:

```properties
Create a multi-product carousel for our end-of-summer skincare sale. For each card, lead with the product's core benefit and emphasize the sale value.
```

This prompt describes a sequential carousel that tells a story across five cards:

```properties
Create a narrative carousel for our compliance alert-management platform. Start with shared intro text about the cost of alert fatigue. Across five cards, build the story: rising review costs, too many low-value alerts, false positives as the hidden cost driver, a solution that cuts false positives by more than 50%, and a closing learn-more call to action.
```

For prompt fundamentals, see [Write effective prompts](/help/user-guide/effective-prompts.md).

## Generate and review concepts

After you set up the cards and prompt, generate the carousel and review the results.

1. Select **[!UICONTROL Generate]**.

   [!DNL GenStudio for Performance Marketing] generates four carousel concepts. Each concept is a complete multi-card carousel with its own brand score.

   ![Four generated carousel concepts, each with a brand score and an Edit button](./carousel-concepts.png){width="80%" zoomable="yes"}

1. Select a concept, then select **[!UICONTROL Edit]** to open it for editing.
1. Use the arrows to move between cards, then edit the text or select **[!UICONTROL Swap]** to change a card's image. For more information about editing, see [Manage variants](/help/user-guide/create/manage-variants.md).

If you reorder cards before you generate, the Canvas updates immediately. If you reorder cards in the prompt drawer after you generate, the change applies only after you generate again, and a regeneration warning appears.

## Understand per-card and shared fields

Some carousel fields apply to each card individually, and others apply to the whole ad. The following table describes how each field behaves for Meta carousel ads.

| Field | Scope |
|---|---|
| Headline | Per card |
| Description | Per card, optional, set in [!DNL Activate] |
| Call to action | Shared across the ad |
| Primary text | Shared across the ad |
| Media | Per card (image, video, or mixed) |
| On-image text | Per card |
| Destination URL | Per card, set in [!DNL Activate] |

## Publish, export, and activate

When your carousel is ready, publish and export it the same way you do for other Meta ads. A carousel is stored as a single experience that corresponds to one concept. Export delivers a CSV file plus the card media. See [[!DNL Content]](/help/user-guide/content/overview.md) for how published experiences are stored. To activate your carousel to Meta, see [Activate a Meta ad](/help/user-guide/activation/activate-meta-ad.md).
