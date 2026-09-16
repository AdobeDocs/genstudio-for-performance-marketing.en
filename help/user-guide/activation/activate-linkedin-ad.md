---
title: Activate a LinkedIn Ad
description: Learn how to activate a LinkedIn ad experience.
feature: Ad Activation
exl-id: edc95319-36c3-4cbf-a5c0-865b49482b50
TQID: https://experienceleague.adobe.com/1mcxWePqYd8tYp3e1D2UTSeBHSvPj4WrqeSyiUCxD8c
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
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
---
# Activate a LinkedIn ad

Adobe GenStudio for Performance Marketing supports the activation of LinkedIn ad experiences to [LinkedIn Campaign Manager](https://business.linkedin.com/marketing-solutions).

**Supported formats**: Single Image, Single Video.

You can [create a LinkedIn experience](/help/user-guide/create/create-linkedin.md) in GenStudio for Performance Marketing, then select it for activation.

Activating a LinkedIn ad follows the [same general steps](create-activation.md) required for activation to other paid ad channels. This page covers LinkedIn-specific prerequisites and setup fields. After you activate a LinkedIn experience in GenStudio for Performance Marketing, use LinkedIn Campaign Manager to review the experience and launch the ad.

GenStudio system managers and editors can activate ad experiences.

## Prerequisites

* A LinkedIn Campaign Manager account with full permission to manage campaigns and ads. This account must contain existing campaigns.
* LinkedIn ad accounts with full permission to create ads and post content on LinkedIn pages.

The target LinkedIn campaign and ad set must already exist in LinkedIn Campaign Manager. GenStudio for Performance Marketing does not create campaigns or ad sets.

>[!NOTE]
>
>LinkedIn renamed its campaign hierarchy: what LinkedIn Campaign Manager previously called a **campaign group** is now called a **campaign**, and what it previously called a **campaign** is now called an **ad set**. The **[!UICONTROL LinkedIn campaign]** and **[!UICONTROL LinkedIn ad set]** setup fields in [!DNL Activate] use this current terminology.

GenStudio for Performance Marketing currently supports Single Image and Single Video LinkedIn ads, which each carry only one image or video per post. If your experience includes multiple aspect ratios, [!DNL Activate] generates a separate row per ratio in the activation table so each can run as its own ad; delete any rows you don't need.

## Connect your LinkedIn accounts

Before your organization can activate experiences, a GenStudio system manager or editor must connect your LinkedIn ad accounts to GenStudio for Performance Marketing. You must have full admin access to both the ad account and the LinkedIn profile page to connect successfully. You only have to connect an ad account in **[!UICONTROL Settings]** once. After that, it's available to anyone who can access that instance.

This connection allows data to flow between GenStudio for Performance Marketing and LinkedIn, enabling the activation process.

After the sync completes, you can view the added accounts. Large amounts of data take longer to sync.

## LinkedIn setup fields

Approved assets, headlines, and introductory text are locked and can't be edited during activation, since they already went through review and approval in [!DNL Content]. You can edit:

* **Text fields**: Description, Call-to-action, Destination URL, URL Parameters, Tracking ID (used as the platform ad name)
* **Platform setup fields**: LinkedIn ad account, LinkedIn campaign, LinkedIn ad set
