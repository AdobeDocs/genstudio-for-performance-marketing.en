---
title: Activate a TikTok Ad
description: Learn how to activate a TikTok in-feed video ad experience.
feature: Ad Activation
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
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
# Activate a TikTok ad

Adobe GenStudio for Performance Marketing supports the activation of TikTok ad experiences.

**Supported formats**: In-Feed Video Ads.

You can [create a TikTok experience](/help/user-guide/create/tiktok-experiences.md) in GenStudio for Performance Marketing, then select it for activation.

Activating a TikTok ad follows the [same general steps](create-activation.md) required for activation to other paid ad channels. This page covers TikTok-specific prerequisites and setup fields. After you activate a TikTok experience in GenStudio for Performance Marketing, use TikTok Ads Manager to run final checks and turn the ad live.

GenStudio system managers and editors can activate ad experiences.

## Prerequisites

* A TikTok Ads account with Operator or Admin access.
* At least one TikTok ad account enabled for use, connected by a GenStudio system manager or editor.
* The target TikTok campaign must already exist in TikTok Ads Manager. Budget, bid, optimization, and targeting for the ad group are defined in TikTok Ads Manager, not in GenStudio for Performance Marketing.

## Connect your TikTok account

Before your organization can activate experiences, a GenStudio system manager must connect your TikTok Ads account to GenStudio for Performance Marketing:

1. Go to **[!UICONTROL Settings]** > **[!UICONTROL TikTok]** > **[!UICONTROL Connect]**.
1. Sign in to your TikTok Ads Manager account in the window that opens, and complete OAuth sign-in. Your account must have Operator or Admin access to the ad account.

After the connection completes, confirm that at least one TikTok ad account is enabled for use.

## TikTok setup fields

Approved assets and primary text are locked and can't be edited during activation, since they already went through review and approval in [!DNL Content]. You can edit:

* **Text fields**: Call-to-action, Destination URL, Tracking ID (used as the platform ad name)
* **Platform setup fields**: TikTok Ads account, Campaign, Ad group
