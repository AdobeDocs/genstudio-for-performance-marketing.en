---
title: Activation workflow
description: Learn about the activation workflow for ad experiences.
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
---
# Activation workflow

_[!DNL Activate]_ supports the activation of ad experiences in channel-specific formats, such as a Meta or Google Campaign Manager 360 ad experience.

A GenStudio for Performance Marketing experience is a marketing campaign component, such as an ad, that is prepared as an ad experience to a specific audience on a paid ad channel or email. Experiences for activation contain three main components:

* **Media assets**: Media assets are the images (GIFs, PNG, JPEG) included in your ad experience. Activation currently supports static images.

  Selecting an image asset for your ad experience requires choosing an appropriate aspect ratio. Aspect ratios define the proportional relationship between an image's width and height, and they are crucial for the effectiveness of ad placements. Paid media channels carefully specify valid aspect ratios for each ad placement on their platform. When adding image assets to your activation, you must select the aspect ratio based on the final ad placements for your experience. File types are restricted to JPEG, PNG, and GIF.

* **Text**: Text comprises all forms of copy that are included in your ad, including headlines, body text, and call-to-action elements.

* **Metadata**: User-defined attributes that you can assign to content. Metadata enhances performance analysis, filtering, and tracking. It is typically not visible to users.

Creating an activation involves refining each of these ad components for a designated channel placement and marketing campaign. GenStudio for Performance Marketing supports activating one experience to one paid channel.

## Workflow phases

Although unique placement requirements define each paid channel, all ad activations share the same high-level steps. Activating an experience to any paid channel has three core phases:

1. **Connect GenStudio for Performance Marketing to your target channel**. A GenStudio system manager must connect your channel accounts before you can activate an experience.

1. **Prepare your experience for activation**. You can prepare experiences for activation in two ways:

   * Activate an approved experience with predefined settings directly from _[!DNL Content]_. This streamlined way of activating one or more ad experiences to a single channel. Once you select an experience from the _[!DNL Content]_ gallery, you cannot edit or add assets to your ad experience. Activate from _[!DNL Content]_ is available for Meta and Google Campaign Manager 360 ad experiences.

   * Assemble your ad experience by selecting visual assets from _[!DNL Content]_, adding text elements, and selecting aspect ratios. This method involves more steps but offers greater creative flexibility. Preparation includes selecting the media assets in the appropriate aspect ratio for your specific ad placement and assigning text to call-to-action elements and body copy. You can add informative metadata that aids users in searching for the experience after activation. Each ad channel placement specifies valid aspect ratios for visual assets included in the placement.

1. **Review and publish your experience to the target channel**. Use the _Preview_ panel during experience setup to assess your choice of ad placement and text elements before finalizing your activation. Your final pre-publication review occurs in the destination channel's ad management app. For example, after activating a Meta ad experience in GenStudio for Performance Marketing, you must log into Meta Ads Manager, review your ad experience, then select its specific attributes before publishing it.

Once an ad experience is live on its target paid media channel, _[!DNL Insights]_ can track and analyze its performance data.

## Supported channels

Each paid media channel has a unique activation workflow. Select the paid channel for activation guidelines:

* [Meta](activate-meta-ad.md)
* [Google Campaign Manager 360](activate-cm360-ad.md)
