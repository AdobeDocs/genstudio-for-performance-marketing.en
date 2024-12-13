---
title: Adobe GenStudio for Performance Marketing release notes
description: Learn about the latest features and enhancements to Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
last-substantial-update: 2024-11-14
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
---
# GenStudio for Performance Marketing release notes

This release information details the latest updates to the GenStudio for Performance Marketing application.

## 2024.12.12 {#latest}

### New features

Content editors can now:

* Edit asset, experience, and template metadata. See [Asset details](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/asset-details). <!-- GS-4905 6935-->

* Export display ads and Meta ads as HTML. See [Create a display ad experience](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/create-display-ad) and [Create a meta ad experience](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/create-meta-ad). <!-- GS-7093 6655-->

* Export Meta or display ad experiences from the _Experiences_ view as JPEG or PNG files. <!-- GS-5152 -->

* View an asset's generated tags in the _Details_ view of any experience that uses the asset. See _Generated tags_ in [Asset details](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/asset-details#generated-tags). <!-- GS-3705 -->

* Assign custom width and height to web banners in display ad templates. These values are now saved as template metadata. See [Best practices for templates](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates) <!-- GS-6735 -->

* Assign custom dimensions to images during image upload. See [Best practices for templates](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/best-practices-for-templates). <!-- GS-7166 -->

* Use the **[!UICONTROL Refresh]** button on the [!DNL Content] Template _Asset details_ view to refresh the selected template.  <!-- GS-7102 -->

* Duplicate existing brands. <!-- BRANDS-548 -->

* Regenerate sections of display ad and email variants. See [Create a display ad experience](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/create-display-ad) and [Create an email experience](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/create-email-experience). <!-- GS-5080 5078-->

### Fixes and enhancements

* Display ad titles are now saved to [!DNL Content] as expected. <!-- GS-7239 -->

* The prompt drawer no longer closes when an editor clicks outside the drawer drop-down menu. <!-- GS-7275 -->

* The [!DNL Create] [!DNL Persona]/[!DNL Product] drop-down menu now loads as expected when a thumbnail URL service error occurs. <!-- GS-7277 -->

* Display ads that contain elements that overlay fragments are now editable. <!-- GS-7186 -->

* The Canvas **[!UICONTROL Brand]** button is now disabled when brand scores are not generated for an experience. <!-- GS-6429 -->

* The Canvas now displays resized experiences in consistent order. <!-- GS-7123 -->

* Manual crop now uses image dimensions, not template dimensions, when editing display ads. Previously, when an image was smaller than the dimensions specified in the display ad template, the bounding box used template dimensions, not image dimensions. <!-- GS-7315 -->

* Editors can now select up to four images when creating a display ad. <!-- GS-7189 -->

* Display ad and Meta ad drafts now load as expected when resized on a different browser. <!-- GS-7204 -->

* Unused template fields are no longer displayed in generated content.  <!-- GS-5670 -->

* Editors can now single-click on links to edit as expected in generated variants. <!-- GS-7423 -->

* [!DNL Create] now correctly respects collaborator privileges. <!-- GS-7614 -->

* The Canvas **[!UICONTROL Resize]** button is now disabled after all resize options have been selected and rendered. <!-- GS-5940 -->

* Reviewers with view-only access can now zoom in and out of variants during reviews. <!-- GS-7371 -->

* Keyboard focus has been added to only actionable buttons on the [!DNL Create] _Recent work_ view. <!-- GS-4060 -->

* The **Saving in progress** message displayed during email fragment save operations is now displayed only during the save operation. Previously, the Canvas displayed this message indefinitely. <!-- GS-6964 -->

* Editors now see an error message as expected when a draft fails to load in the [!DNL Create] _Recent Work_ area.  <!-- GS-8081 -->

* The Canvas now displays resized Meta ads and display ads in correct order.  <!-- GS-7375 -->

* Editors can now single-click into fields on email and display ads. <!-- GS-6297 -->

* Edit fragment capability for email and Meta ads is now triggered as expected by a single click. <!-- GS-8081 -->

* Improved performance of the [!DNL Create] **[!UICONTROL Back]** button. <!-- GS-6767 -->

## Earlier release notes

+++Notes from 2024.11.14

### New features

Added support for rich media templates, enabling customers to reuse assets that have already been published through their own managed content channels. <!-- GS-6107 -->

### Fixes and enhancements

* When resized in a browser other than the one used to generate the initial content, drafts now load as expected. <!-- GS-7204 -->

* All characters are now represented correctly in exported HTML. <!-- GS-7246 -->

* The buttons on the [!DNL Content] _Experiences_ **[!UICONTROL Export]** popup are no longer truncated in certain languages. <!-- GS-6873 -->

* Display ads created with templates sized at 50x50 are now exported in the expected image size. Previously, PNG files were exported at double the expected dimensions. <!-- GS-7192 -->

* Template errors that occurred when Display ads were resized are now resolved. <!-- GS-7322 -->

### Localization

This release includes improvements to localization throughout the UI, including:

* All strings in the [!DNL Content] _Upload asset_ popup are now correctly localized. <!-- GS-6872 6770 -->
* All tooltips in [!DNL Content] _Assets_ view **[!UICONTROL Search]** field are localized. <!-- GS-6879 -->
* When replacing an existing image in an email variant on the [!DNL Create] Canvas, the _Select from Content_ view is now localized. <!-- GS-6906 -->

+++

+++Notes from 2024.11.07

### Fixes and enhancements

* The _Save in progress_ spinner is no longer displayed when a user clicks **[!UICONTROL Upload New Image]** then cancels the operation before upload completes. <!-- GS-6780 -->

* Experience titles are now created correctly during experience regeneration. <!-- GS-7006 -->

* Issues with flickering scrollbars during draft loading have been resolved. <!-- GS-5587 -->

* The `View documentation` link in the [!DNL Content] _Add your approved template_ popup now works as expected. <!-- GS-6881 -->

* Deleting an image from the prompt drawer during a resize operation no longer results in an error. <!-- GS-7115 7009 -->

* Selecting **[!UICONTROL Delete]** from the [!DNL Create] action menu (…) now works as expected. <!-- GS-6871 -->

* Users can now control all Meta ad template interactive elements by keyboard alone. <!-- GS-4066 -->

* Added extraction of image dimensions from template image fields to Display ad templates. Smart crop requests are now sent for the actual dimension of the image and not the entire template. <!-- GS-6926 -->

* Localized the `Zoom to fit to screen` string in generated email and Meta ads. <!-- GS-5063 -->

* The [!DNL Create] prompt drawer now closes as expected when a user clicks away. <!-- GS-5254 -->

* Meta ads export now includes the selected call-to-action label as expected. <!-- GS-6504 -->

* Brand score is now updated and retained as expected for regenerated experiences. <!-- GS-6535 -->

* HTML export of Meta ads and display ads no longer include wrapper `div` and `chrome` elements. <!-- GS-7116 -->

* Issues with email draft rendering during publishing are now resolved. <!-- GS-6394 -->

* The Canvas **[!UICONTROL Brand]** button is now disabled when a brand score is not generated. <!-- GS-6429 -->

* The Facebook/Instagram toggle on the Canvas action bar now updates experience renderings as expected when the `ReadOnly` Canvas setting is enabled. <!-- GS-7039 -->

#### Image regeneration

* Resizing multiple Meta ad variants now works as expected. Previously, the Canvas did not display regenerated variants, but remained blank. <!-- GS-7010 -->

* Fragment regeneration now works as expected for resized experiences. <!-- GS-6836 -->

* Regenerating Meta ad images after resizing them no longer results in an error. Previously, resizing images before regeneration changed the channel metadata from `meta` to `facebook`. <!-- GS-7042 -->

+++

+++Notes from 2024.10.31

### New features

* The **[!DNL Content]** search filter now supports search by color tag. <!-- GS-5501 -->

* The **[!DNL Create]** Canvas now displays character counts for email fragments. <!-- GS-5819 -->

### Fixes and enhancements

* Missing screen reader labels have been added to mobile and desktop `view` elements. <!-- GS-5624 4729 -->

* The **[!DNL Create]** Canvas email subject line and pre-header text areas are now dynamic in height. <!-- GS-6258 -->

* Layout issues with email borders have been resolved. <!-- GS-6631 -->

* Keyboard focus now works as expected on the **[!DNL Content]** **[!UICONTROL Delete]** button. Previously, users could not access this button by the keyboard.  <!-- GS-4065 -->

## 2024.10.14 General Availability release

This release introduces Adobe GenStudio for Performance Marketing, a generative AI-based application that accelerates the planning, development, and analysis of marketing campaigns. GenStudio for Performance Marketing empowers marketing teams to create on-brand, multi-channel content for ads, emails, and campaigns while providing real-time insights to optimize content performance.

### Features

Major product features include:

**[!DNL Create]** introduces the Canvas, which offers a structured prompting experience that enables content editors to quickly generate content and variants. System managers train the product on organizational brand guidelines. [!DNL Create] ensures that all AI-generated content aligns with your brand guidelines—branding, customer personas, and product descriptions—and streamlines the production of high-impact, brand-consistent marketing content.

**[!DNL Content]** stores curated, brand-compliant approved assets and experiences. GenStudio for Performance Marketing users can easily find, edit, repurpose, and share approved assets, reducing the need to recreate content from scratch for every campaign.

**[!DNL Reviews and Approvals]** establishes a framework for stakeholders to review and approve generated variants before saving to **[!DNL Content]** or exporting.

**[!DNL Campaigns]** organizes and manages marketing campaigns, ensuring streamlined execution and tracking. Collaborators can visualize, plan, and track campaigns to manage multiple initiatives effectively and ensure timely delivery.

**[!DNL Insights]** offers real-time assessment of content performance, helping marketers optimize their strategies and make data-driven decisions.

GenStudio for Performance Marketing integrates with other Adobe Experience Cloud products including Adobe Express and Adobe AEM Assets.

+++
