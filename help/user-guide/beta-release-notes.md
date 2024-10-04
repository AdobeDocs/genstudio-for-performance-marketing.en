---
title: Adobe GenStudio for Performance Marketing Beta release notes
description: Learn about the latest features and enhancements to Adobe GenStudio for Performance Marketing.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
---
# Adobe GenStudio for Performance Marketing Beta release notes

These notes highlight significant Adobe GenStudio for Performance Marketing fixes and enhancements for the week ending October 4.

## New features and enhancements

* Filtering capability across the product has been enhanced. Issues with filtering by age and gender in [!DNL Insights] have been resolved.  <!-- GS-1198 -->

* You can edit image assets (JPG or PNG) directly using Adobe Express. Content editors can use the _[!UICONTROL Powered by Adobe Express]_ Canvas to remove backgrounds, apply generative fills, adjust effects, and crop images without leaving GenStudio for Performance Marketing. <!-- GS-4615 -->

* Improved the experience of progressive loading for generated variants, generated email, and contextual messaging. <!-- GS-4651 3062-->

* Content editors can now use the adjust crop feature to crop rendered images in variants. <!-- GS-2342 -->

* Issues with resizing and duplicating templates have been resolved. <!-- GS-4895 -->

* Brand validation now explains the cause of failures that occur during validation.

* Template previews now display on-image text as expected. <!-- GS-5917 -->

## Additional enhancements and fixed issues

* The [!DNL Create] Canvas now renders custom fonts from templates as expected. <!-- GS-3415 -->

* The correct font is now applied during Meta ad export. <!-- GS-5875 -->

* Issues with template upload that resulted in successful upload but lack of visibility in the product interface have been resolved. <!-- GS-4815 5650-->

* Users can now manually crop Meta ads after resizing them. <!-- GS-5871 -->

* Users no longer need to log in twice to a channel Meta ads account when they are also logged in to Facebook. <!-- GS-3009 -->

* The Canvas view of assets and experiences now remains consistent across the content creation, review, and approval process. <!-- GS-5877 -->

* The Canvas now displays only four variants when regenerating after a resize operation. <!-- GS-5869 -->

* Browser-based spellcheck now works as expected in the [!DNL Create] Canvas. <!-- GS-5760 -->

* Display Ads are now exported as PNG files when **[!UICONTROL Export as PNG]** is selected. Previously, display ads were exported as JPEG when PNG format was selected. <!-- GS-5545 -->

* Padding has been increased between the **[!UICONTROL Manual crop]** button and **[!UICONTROL Generate]** button. Previously, the **[!UICONTROL Manual crop]** button was partially obscured. <!-- GS-6084 -->

* Template previews now display Google fonts as expected. <!-- GS-5946 -->

* Imported TypeKit and Google fonts are now loaded as expected during export. <!-- GS-5948 -->

* Resolved issues with generating content with custom templates. Previously, when a content editor tried to generate an asset using a custom template, the generation popup was not displayed, and the console displayed errors. <!-- GS-5262 -->

* The DisplayAds draft Canvas now maintains its position when a user right-clicks the Canvas before left-clicking out of the context menu. Previously, the Canvas shifted when the user left-clicked, which rendered the draft content partially inaccessible.  <!-- GS-5687 -->

* Loading shimmer effects now persist until image regeneration is complete.  <!-- GS-5811 -->

* Brand validation scores are no longer invalidated after a user makes edits to generated email, Meta ads, or display ads. Previously, this score was hidden. <!-- GS-5379 -->

* Templates that have CSS styles attached to their `body` element are now leveraged as expected during export of experiences. <!-- GS-5947 -->

* Corrected issues with the manual crop of large dimension images. <!-- GS-6039 -->

* Only one pop-up message now appears when a user adds a new asset in [!DNL Content]. <!-- GS-5020 -->

* Improved Canvas performance during text editing.  <!-- GS-5118 -->

* Added missing spaces between strings on the [!DNL Create] Email or Meta ad Canvas. <!-- GS-5019 -->

* Editors can now save a file with names that contain special characters after editing in Express. <!-- GS-6131 -->

### Localization

This release includes improvements to localization throughout the product interface, including these interface areas:

* The URL for the **[!UICONTROL Learn more]** option destination in the [!DNL Create] prompt menu. <!-- GS-5029 -->

* Number formats adjacent to the [!DNL Insights] > [!DNL Experience] search input fields. <!-- GS-4494 -->

## Known issue

* Regenerated email fragments do not appear in the variant after selection. (However, variants appear after the draft is reopened.) <!-- GS-5913 -->