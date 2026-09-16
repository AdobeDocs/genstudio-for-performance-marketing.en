---
title: Activate a Google Campaign Manager 360 Ad
description: Learn how to activate a Google Campaign Manager 360 experience.
feature: Ad Activation
exl-id: e4ee4e04-8dd0-4e05-a0f7-0ddca2fbb6be
TQID: https://experienceleague.adobe.com/pQbT2OC7-jK33HhJWgTBBtJrmEvr48mGkl8v-fTkOLQ
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
---
# Activate a Google Campaign Manager 360 ad

Adobe GenStudio for Performance Marketing supports the activation of ad experiences to Google Campaign Manager 360.

**Supported formats**: Static Display, Video Display, HTML5 Zip Display.

Activating a Google Campaign Manager 360 ad follows the [same general steps](create-activation.md) required for activation to other paid ad channels. This page covers prerequisites and setup fields specific to Google Campaign Manager 360. After you activate an experience in GenStudio for Performance Marketing, use Google Campaign Manager 360 to review the experience and launch the ad.

GenStudio system managers and editors can activate ad experiences.

## Prerequisites

* A Google Campaign Manager 360 account with access to the target advertiser.
* Admin access to the advertiser, to read and write into Campaign Manager 360.

Campaign Manager 360 organizes campaigns and ads within different advertisers, and each advertiser includes a creative library. The target advertiser must already exist in Campaign Manager 360; GenStudio for Performance Marketing publishes ad experiences into that advertiser's creative library, but does not create ads.

## Connect your Google Campaign Manager 360 account

Before your organization can publish assets in a creative library, a GenStudio system manager or editor must connect your Google Campaign Manager 360 account to GenStudio for Performance Marketing. You must have admin access to the advertiser to read and write into Campaign Manager 360. See [Connect paid media accounts](/help/user-guide/connectors/connect-channel.md).

After the sync completes, you can view the added accounts.

## Google Campaign Manager 360 setup fields

Approved assets are locked and can't be edited during activation, since they already went through review and approval in [!DNL Content]. You can edit:

* **Text fields**: Tracking ID (used as the platform creative name)
* **Platform setup fields**: Advertiser

Your creative experience is delivered to the selected advertiser's creative library in Google Campaign Manager 360 when activation completes.
