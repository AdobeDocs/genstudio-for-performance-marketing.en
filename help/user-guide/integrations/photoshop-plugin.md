---
title: Photoshop Plugin for Adobe GenStudio for Performance Marketing
description: Learn how to configure and use the Photoshop plugin for GenStudio for Performance Marketing.
feature: Generative AI
role: User
exl-id:
---
# Photoshop plugin for GenStudio for Performance Marketing

The GenStudio for Performance Marketing Photoshop plugin adds a new panel to Adobe Photoshop that allows users to perform GenStudio for Performance Marketing actions, like generating on-brand content.

This page describes how to install and configure the plugin, and how to use it.
Features of this plugin include:

* Log in to a GenStudio for Performance Marketing instance with an Adobe ID
* Map GenStudio for Performance Marketing content generation fields to text layers in a Photoshop document
* Specify a brand, product, persona, and text prompt for generating content
* Preview the generated on-brand content variations
* Apply generated content easily to mapped layers in the current document
* Export generated [!DNL Experiences] to a local source as flattened images
* Export generated [!DNL Experiences] to GenStudio for Performance Marketing

## Installation

Follow these instructions to install the plugin.

### Prerequisites

* Creative Cloud desktop application
* Photoshop, minimum version 25.6.0

### Installation steps

1. Download the plugin's distributable package: `genstudio-creative-cloud_1.0.0_PS.ccx`.
1. Double-click the package to launch it.
1. Acknowledge and accept the risk notifications about third-party, non-marketplace plugins.
1. To upgrade to the latest version of the plugin, simply download the updated distributable package and repeat the installation steps.

### Uninstalling the plugin

1. Launch the Creative Cloud desktop application.
1. Click the **[!UICONTROL Plugins]** option.
1. Click the ellipsis, **[!UICONTROL (...)]**, on the GenStudio for Creative Cloud card for options.
1. Choose **Uninstall**.

## Create a template

To generate content you'll need a GenStudio for Performance Marketing template created from the Photoshop document you'll be modifying.

To create a GenStudio-ready template:

1. Open the document in Photoshop.
1. Identify a text layer that will include generated content.
1. Rename the layer with the field name convention format: `{<name_of_generated_field>}`. For example; `{body}`, `{headline}`, `{cta}`.
1. Rename layers for all fields that are required by the channel intended for the template.

| Channel | Required fields |
|---------|----------------|
| Email | `subject`, `pre_header`, `cta`, `body`, `headline` |
| Meta | `body`, `headline`, `cta`, `on_image_text` |
| Display | `headline`, `body`, `cta` |

Note that multiple layers may share the same field designation, but each layer may only specify one field. For example, if there are multiple artboards in the document:

* ✓ You can specify a `{headline}` layer in each artboard
* ✓ You can specify multiple `{headline}` layers in a single artboard
* ✗ You CANNOT specify that a single layer receives both the `{headline}` and the `{cta}` field names

The document is now ready to be used with the plugin.

## Generate new content

1. Open Photoshop.
1. Open a GenStudio-ready template document that you've created ([see instructions above](#create-a-template)) or use the Acrobat display ad template: `branding-template-acrobat-handlebars.psd`.
1. Open the plugin panel at **Plugins > GenStudio for Creative Cloud > GenStudio Create**.
1. Click the **[!UICONTROL Login]** button. If prompted for permission to open a URL, optionally check **Remember my choice**, then click **[!UICONTROL Allow]**.
1. Use the web browser to log in with a profile that has access to GenStudio for Performance Marketing.
1. Select the channel that applies to the template you've opened. _Display ad_ for the template provided above.
1. Click **[!UICONTROL Let's go!]**.
1. Select the [!DNL Brand], [!DNL Persona], and [!DNL Product] context for the content that will be generated.
1. Provide a text prompt for the content in the **[!UICONTROL Text Prompt]** box.
1. Click the **[!UICONTROL Generate]** button. Variations will generate and appear on cards in the plugin panel.
1. Review the generated content, and select the variations to apply by clicking the cards in the panel.
1. Click the **[!UICONTROL Apply Content]** button. 

New documents will be added to your Photoshop workspace with the generated content applied to the template fields. These documents will be named with a variation suffix.
