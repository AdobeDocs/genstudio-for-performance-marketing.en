---
title: Activate a Meta Ad
description: Learn how to activate a Meta ad experience.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
TQID: https://experienceleague.adobe.com/hDR0ngNiGnCXCCOgNhVG8gX4kHGrNvfybPbuMLwYk7U
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
subfeature_v2:
  - id: d87258a7-722c-4afd-b632-adddc447c7aa
    internal-label: Ad activation
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
---
# Activate a Meta ad

Adobe GenStudio for Performance Marketing supports the activation of Meta ad experiences to Instagram and Facebook.

**Supported formats**: Image, Video, Carousel.

[Create a Meta experience](/help/user-guide/create/create-meta-ad.md) in GenStudio for Performance Marketing, then select it for activation.

Activating a Meta ad follows the [same general steps](create-activation.md) required for activation to other paid ad channels. This page covers Meta-specific prerequisites and setup fields. After you activate a Meta experience in GenStudio for Performance Marketing, use [Meta Ads Manager](https://adsmanager.facebook.com/) to review the experience and launch the ad.

Unlike some other channels, a Meta ad can include multiple aspect ratios within a single ad. If your experience has multiple aspect ratios, [!DNL Activate] still generates only one row for it, not one row per aspect ratio.

GenStudio system managers and editors can activate ad experiences.

## Prerequisites

Confirm that your connected Meta ad accounts have full permission to manage ads in these components of the Meta advertising platform:

* Meta Ad Account
* Facebook page
* Meta campaign
* Meta ad set
* Instagram profile (optional)

The target Meta campaign and ad set must already exist in Meta Ads Manager. GenStudio for Performance Marketing does not currently create campaigns or ad sets.

## Connect your Meta accounts

Before your organization can activate experiences, a GenStudio system manager must connect your Meta accounts to GenStudio for Performance Marketing. This connection allows data to flow between GenStudio for Performance Marketing and Meta, enabling the activation process. See [Connect to Meta Ads](/help/user-guide/connectors/meta-ads.md).

To select an Instagram account, make sure in Meta Business Manager that [the Instagram account you want to use is connected to the same ad account](/help/user-guide/connectors/meta-ads.md#connect-an-instagram-account) selected during onboarding. If this connection is missing, the Instagram account may not appear in the **[!UICONTROL Instagram profile]** drop-down menu during activation.

After the sync completes, you can view the added accounts. Large amounts of data take longer to sync.

## Meta setup fields

Approved assets, headlines, and body copy are locked and can't be edited during activation, since they already went through review and approval in [!DNL Content]. You can edit:

* **Text fields**: Description, Call-to-action, Destination URL, URL Parameters, Tracking ID (used as the Meta ad name)
* **Platform setup fields**: Ad account, Facebook page, Instagram profile, Meta campaign, Meta ad set
