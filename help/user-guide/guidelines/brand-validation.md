---
title: Brand validation in Adobe GenStudio for Performance Marketing
description: Learn how the built-in brand validation system works in GenStudio for Performance Marketing.
feature: Brands Service, Brand Personalization, Variant Generation, Compliance, Content Generation, Content Review
exl-id: 2e777186-3b7e-46a6-9d37-7c7b7c2aa7ae
---
# Brand validation

In GenStudio for Performance Marketing, brand validation is an essential component that works in collaboration with the generative AI functionality and guidelines—[[!DNL Brands]](/help/user-guide/guidelines/brands.md), [[!DNL Products]](/help/user-guide/guidelines/products.md), and [[!DNL Personas]](/help/user-guide/guidelines/personas.md). It ensures that all your content aligns with your brand identity, ADA standards, and individual channel platform guidance.

GenStudio for Performance Marketing conducts brand validation and other content checks on various aspects, including:

* Defined or default [!DNL Brand] guidelines
* Platform guidelines
<!-- * Ethical considerations related to gender, ethnicity, race, disability status, and age in AI-generated content -->
* American with Disabilities Act (ADA) standards

## Content check summary

A summary of brand validation and other content check information for each generated content variant is accessible through the _Content check_ summary icon for each variant in the Canvas.

The _Content check_ summary displays the:

* Percentage of compliance with your [[!DNL Brand]](brands.md) calculated as the number of [guidelines](overview.md) that passed validation versus the number of guidelines tested
* `Pass` or `Fail` result for the platform guidelines, such as Meta or LinkedIn
* `Pass` or `Fail` result for ADA accessibility standards

![Content check summary](/help/assets/content-check-summary.png){width="400" zoomable="yes"}

Click the percentage to see how compliant the variant is. The scores auto-update as you make edits to the variants. You can click _View and fix issues_ to ensure further compliancy.

See [Improve brand alignment](#improve-brand-alignment).

## Content check panel

The _Content check_ panel opens on the right side of the Canvas when clicked from the right action bar _or_ from the [_Content check_ summary icon](#content-check-summary) for a variant. This panel provides detailed brand validation. platform guidelines, and accessibility standards information and illuminates opportunities for improvement for each variant section.

![Content check panel](/help/assets/content-check-panel.png){height="250" zoomable="yes"}

The _Content check_ panel displays validation and [compliance information](/help/user-guide/guidelines/overview.md#compliance) for each section of the variant:

* Representation of the _Content check_ summary information for [!DNL Brand], platform guidelines, and accessibility standards
* _Needs review_ section displaying the number of failed guidelines and detailed information about each guideline needing revision
* _Passed_ section displaying the number of passed guidelines and detailed information about each passing guideline

See [Improve brand alignment](#improve-brand-alignment) to learn how to improve the _Content check_ panel scores.

### Content type

In the _Content check_ panel you can toggle which guideline and accessibility standards checks are performed. Click the _Content type_ icon (levels icon) at the top of the panel to toggle on or off:

* **[!DNL Brand]**—Performs the checks associated with [!DNL Brand] guidelines
* **Platform guidelines**—Performs the checks associated with the channel-specific platform, such as Meta
* **Accessibility**—Performs the checks associated with ADA accessibility standards

To **set the content type** for the checks you want performed, click to toggle off or on the available types and click **Apply**.

## Improve brand alignment

To maximize effectiveness of generated content and maintain consistent brand identity, use the [_Content check_ summary](#content-check-summary) and the [_Content check_ panel](#content-check-panel). You can manually modify specific sections to align with your [[!DNL Brand] guidelines](brands.md), platform guidelines checks, and accessibility standards checks.

**To improve brand alignment for generated variants**:

1. Click the _Content check_ panel icon in the right action bar to see validation and accessibility information for a single variant.

   You can see a summary of the _Needs review_ and _Passed_ checks to see which sections and guidelines need improvement.

   >[!NOTE]
   >
   > The _Brand voice_ guideline noted in the _Content check_ panel applies to the entire variant, not an individual section. The whole content variant is highlighted for suggested improvement.

1. Click to fix guidelines that are not currently compliant.
1. Click to expand and inspect each check that needs review in available sections such as _Headline_ and _Brand voice_.

   Use the reasoning provided for each check to guide you in revising the variants.

1. After making necessary revisions, click **[!UICONTROL Recheck score]** to re-check and validate your changes to ensure they are more closely aligned with your brand identity, platform guidelines, and accessibility standards.

   The content check process runs again. If the revised items pass validation, a green banner appears at the bottom of the Canvas to confirm the score was updated. If there was no change after a re-check, the banner confirms there was no change to the score. The percentage in the _Content check_ summary icon for the revised variant also shows your progress.

1. Continue revising sections to ensure the entire variant passes validation and accessibility checks. Navigate through each variant using the arrows adjacent to an individual variant in the Canvas.

