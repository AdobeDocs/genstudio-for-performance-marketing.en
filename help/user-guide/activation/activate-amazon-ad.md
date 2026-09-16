---
title: Activate Amazon Ads
description: Learn how to activate Amazon Ads experiences.
feature: Ad Activation
exl-id: 539cb43c-a9d8-4473-8a7d-e81967111741
TQID: https://experienceleague.adobe.com/4L4JHcYLSsoQ50QbCW7Mof52h5jpz3z8n0UL8CaqLA8
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
---
# Activate Amazon Ads

Adobe GenStudio for Performance Marketing supports the activation of ad experiences to Amazon Ads.

**Supported formats**: Static Display.

Activating an Amazon Ads experience follows the [same general steps](create-activation.md) required for activation to other paid ad channels. This page covers Amazon Ads-specific prerequisites and setup fields. After you activate an experience in GenStudio for Performance Marketing, use Amazon Ads to review the experience and turn the ad live.

GenStudio system managers and editors can activate ad experiences.

## Prerequisites

* An Amazon Ads account with access to the target advertiser.
* Admin access to the advertiser, to read and write into Amazon Ads.

Amazon Ads organizes campaigns and ads within different accounts, and each account includes a creative library. The target account must already exist in Amazon Ads; GenStudio for Performance Marketing publishes ad experiences into that account's creative library, but does not create accounts.

## Connect your Amazon Ads account

Before your organization can publish assets in a creative library, a GenStudio system manager must connect your Amazon Ads account to GenStudio for Performance Marketing. You must have admin access to the advertiser to read and write into Amazon Ads. See [Connect paid media accounts](/help/user-guide/connectors/connect-channel.md).

After the sync completes, you can view the added accounts.

## Amazon Ads setup fields

Approved assets are locked and can't be edited during activation, since they already went through review and approval in [!DNL Content]. You can edit:

* **Text fields**: Tracking ID (used as the platform creative name)
* **Platform setup fields**: Account

Your creative experience is delivered to the selected account's creative library in Amazon Ads when activation completes.
