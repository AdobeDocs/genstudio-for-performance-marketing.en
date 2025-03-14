---
title: Adobe GenStudio for Performance Marketing release notes
description: Learn about the latest features and enhancements to Adobe GenStudio for Performance Marketing.
recommendations: noDisplay
exl-id: 32f5104e-ae15-4092-8a34-642fc641baf9
---
# GenStudio for Performance Marketing release notes

This release information details the latest updates to the GenStudio for Performance Marketing application.

## 2025.03.13 {#latest}

### Create LinkedIn experiences

[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}

Added support for [creating LinkedIn experiences](/help/user-guide/create/create-linkedin.md). See the [LinkedIn ad](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) tab in channel-specific guidelines.

### Create banner experiences

[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}

Added support for [creating banner experiences](/help/user-guide/create/create-banner-experience.md). See the [Banner](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines) tab in channel-specific guidelines.

### Compliance

As part of the brand validation process, [compliance standards](/help/user-guide/guidelines/overview.md) have been introduced in [Content checks](/help/user-guide/guidelines/brand-validation.md). These checks review each variant in an experience against [!DNL Brand], [!DNL Product], and [!DNL Persona] guidelines, platform guidelines (such as for Meta), ethical considerations, and ADA standards. This process provides a comprehensive summary of the guidelines and standards that need revision for better compliance.

### Extensibility

The new GenStudio for Performance Marketing [extensibility framework](/help/extensibility/overview.md) provides tools for organizations to incorporate their own claims compliance protocols into content creation workflow and validation through Add-ons, or extensible applications.

### Templates

* **Template code editor**—The new [Template code editor](/help/user-guide/content/code-editor.md) helps you verify and refine your template for optimal use when generating new experiences with GenStudio for Performance Marketing.

  ![Code editor view](/help/assets/template-detected-fields.png "Check detected fields"){width="500" zoomable="yes"}

* **Links on image**—Customize your email template by enabling image links. See [Customize a template: Link on image](/help/user-guide/content/customize-template.md#link-on-image).
* **AJO and Marketo templates**—Upload a template that you created in Adobe Journey Optimizer (AJO) or Marketo. See [Work with templates from AJO and Marketo](/help/user-guide/content/use-templates.md#templates-from-ajo-and-marketo).

### Fixes and enhancements

* Enabled functionality for [default channel](/help/user-guide/guidelines/brands.md#channel-guidelines), [image](/help/user-guide/guidelines/brands.md#image-guidelines), [logo](/help/user-guide/guidelines/brands.md#logos), and [color](/help/user-guide/guidelines/brands.md#colors) guidelines for [[!DNL Brands]](/help/user-guide/guidelines/brands.md).
* Added ability to [add links to images](/help/user-guide/create/manage-variants.md#add-image-link) within a variant.
* Shifted the [Content check](/help/user-guide/guidelines/brand-validation.md) and Review and approval functionality to the new right action bar to maximize space on the Canvas and improve the user experience.
* Simplified the flow for [uploading or manually adding a brand](/help/user-guide/guidelines/add-guidelines.md#add-brands).
* Introduced the ability to [add or swap image assets within a variant](/help/user-guide/create/manage-variants.md#swap-image) on the Canvas.
* Improved user experience and visibility of channel categories [on the Create home](/help/user-guide/create/overview.md) by separating them into Owned media, Paid media, and Content sections.
* Improved filtering in [!DNL Insights] table and gallery views.

## Earlier release notes

+++Notes from 2025.02.13

### Landing page improvements for [!DNL Create]

The [!DNL Create] landing page in GenStudio for Performance Marketing includes UI improvements that enhance the user experience. The _Recent work_ section is refined and configured with the list view as the default view. Padding and other visual improvements streamline the look and feel of the [!DNL Create] Canvas.

### Insights export to CSV

You can now download the viewable table from any [!DNL Insights] view into a CSV file. This feature allows you to export and analyze data from various [!DNL Insights] views, facilitating data analysis and reporting options.

+++

+++Notes from 2025.01.16

### Integration with Adobe Workfront Proof

[!BADGE Beta]{type=Informative tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."}

The GenStudio for Performance Marketing and Adobe Workfront Proof integration Beta program launches this month. Workfront Proof boosts the content creation and activation lifecycle with approval templates, multi-stage workflows, and annotations. GenStudio for Performance Marketing users with Workfront Proof entitlements can use Proof's advanced capabilities within GenStudio for Performance Marketing to review and comment on GenStudio-generated content.

Beta programs provide a way to help shape product development and determine general availability readiness.

### Generate new Calls to Action

You can now generate new call-to-action (CTA) phrases when managing variants. Use the new _Rephrase_ and _Add link_ options to generate new phrases and edit the CTA link. Your template must be set up properly for these new CTA functions to work. Follow the guidelines in _Customize a template_: [Calls to action](/help/user-guide/content/customize-template.md#calls-to-action). For guidelines on managing CTAs in variants, see [Revise Call to action](/help/user-guide/create/manage-variants.md#revise-call-to-action). <!-- GS-6676 -->

### Fixes and enhancements

* Character counts are now displayed in all generated and manual fields of display ads. See _Character counts_ in [Meta experiences](/help/user-guide/create/meta-experiences.md#character-counts). <!-- GS-7732 -->

* _Collaborators_ can now view assets but not create, edit, or delete these assets. Previously, collaborator entitlements were not enforced as expected in [!DNL Create]. <!-- GS-7614 -->

* Content editors can now edit asset, experience, and template metadata. <!-- GS-4905 -->

* Custom image sizes within Meta ad templates are now supported. <!-- GS-7512 -->

* Persona, brand, and product selections are now preloaded during template generation. <!-- GS-8069 -->

* The email call-to-action link is no longer a required field. <!-- GS-8103 -->

* The [!DNL Brand] selector drop-down menu now works as expected for templates. Previously, the selector did not load successfully for some templates. <!-- GS-8908 -->

* Editors can now select a maximum of four images for single-pod emails and Meta ads. <!-- GS-2631 -->

* The year value of an approved experience's `Created by` field now stays consistent as expected after the experience's metadata has been edited. <!-- GS-8344 -->

* Content editors can now successfully select a template from [!DNL Create]. Previously, the application threw a console error when an editor selected a template.  <!-- GS-8798 -->

* Issues with resize and regenerate operations for Meta ads have been resolved. <!-- GS-8900 -->

* The **[!UICONTROL Back]** button now returns users to either the previous page or the [!DNL Create] landing page as expected. <!-- GS-8622 -->

+++

+++Notes from 2024.12.12

### New features

Editors can now perform the following metadata-related tasks:

* Edit asset, experience, and template metadata. See [Asset details](/help/user-guide/content/asset-details.md#user-defined-metadata). <!-- GS-4905 6935-->

* View an asset's generated tags in the _Details_ view of any experience that uses the asset. See _Generated tags_ in [Asset details](/help/user-guide/content/asset-details.md#generated-tags). <!-- GS-3705 -->

Editors can now specify custom values to these aspects of generated variants:

* Width and height to web banners in display ad templates. These values are now saved as template metadata. <!-- GS-6735 -->

* Dimensions to images in display ad experiences during image upload.<!-- GS-7166 -->

* See channel-specific guidelines in the [Best practices for templates](/help/user-guide/content/best-practices-for-templates.md#follow-channel-specific-template-guidelines).

Export options now include:

* Export display ads and Meta ads as HTML, JPEG, or PNG. See [Create a display ad experience](/help/user-guide/create/create-display-ad.md) and [Create a meta ad experience](/help/user-guide/create/create-meta-ad.md). <!-- GS-7093 6655 5152-->

Additional new capabilities allow editors to:

* Use the **[!UICONTROL Refresh]** button on the [!DNL Content] Template _Asset details_ view to refresh the selected template. <!-- GS-7102 -->

* Regenerate sections of display ad and email variants. See [Create a display ad experience](/help/user-guide/create/create-display-ad.md#revise-generated-display-ads) and [Create an email experience](/help/user-guide/create/create-email-experience.md#revise-generated-emails). <!-- GS-5080 5078-->

* Duplicate existing brands. See [Manage brands](/help/user-guide/guidelines/brands.md#manage-brands). <!-- BRANDS-548 -->

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

+++

+++Notes from 2024.11.14

### New features

Added support for displaying static content hosted on external domains. GenStudio for Performance Marketing validates the content source defined in the template and embeds a copy to produce the template preview. See [Static content](/help/user-guide/content/customize-template.md#static-content). <!-- GS-6107 -->

### Fixes and enhancements

* When resized in a browser other than the one used to generate the initial content, drafts now load as expected. <!-- GS-7204 -->

* All characters are now represented correctly in exported HTML. <!-- GS-7246 -->

* The buttons on the [!DNL Content] _Experiences_ **[!UICONTROL Export]** popup are no longer truncated in certain languages. <!-- GS-6873 -->

* Display ads created with templates sized at 50x50 are now exported in the expected image size. Previously, PNG files were exported at double the expected dimensions. <!-- GS-7192 -->

* Template errors that occurred when Display ads were resized are now resolved. <!-- GS-7322 -->

### Localization

This release includes improvements to localization throughout the UI, including:

* All strings in the [!DNL Content] _Upload asset_ popup are now correctly localized. <!-- GS-6872 6770 -->
* All tooltips in the [!DNL Content] _Assets_ view **[!UICONTROL Search]** field are localized. <!-- GS-6879 -->
* When replacing an existing image in an email variant on the [!DNL Create] Canvas, the _Select from Content_ view is now localized. <!-- GS-6906 -->

+++

+++Notes from 2024.11.07

### Fixes and enhancements

* The _Save in progress_ spinner is no longer displayed when a user clicks **[!UICONTROL Upload New Image]** then cancels the operation before upload completes. <!-- GS-6780 -->

* Experience titles are now created correctly during experience regeneration. <!-- GS-7006 -->

* Issues with flickering scroll bars during draft loading have been resolved. <!-- GS-5587 -->

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

+++

+++Notes from 2024.10.14 General Availability

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
