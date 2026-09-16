---
title: Activate a ChatGPT Ad
description: Learn how to activate a ChatGPT ad experience.
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
# Activate a ChatGPT ad

Adobe GenStudio for Performance Marketing supports the activation of ChatGPT ad experiences.

**Supported formats**: Chat Cards.

You can [create a ChatGPT experience](/help/user-guide/create/create-chatgpt-ad.md) in GenStudio for Performance Marketing, then select it for activation.

Activating a ChatGPT ad follows the [same general steps](create-activation.md) required for activation to other paid ad channels. This page covers ChatGPT-specific prerequisites and setup fields. After you activate a ChatGPT experience in GenStudio for Performance Marketing, use OpenAI Ads Manager to run final checks and turn the ad live.

GenStudio system managers and editors can activate ad experiences.

## Prerequisites

* An OpenAI Ads account and an API key from that account.
* The target ChatGPT campaign and ad group must already exist in OpenAI Ads Manager. GenStudio for Performance Marketing does not create new campaigns or ad groups.

## Connect your ChatGPT account

Before your organization can activate experiences, a GenStudio system manager must connect your OpenAI Ads account to GenStudio for Performance Marketing:

1. In OpenAI Ads Manager, go to **[!UICONTROL Settings]** > **[!UICONTROL API Keys]** > **[!UICONTROL Create New Key]**.
1. In GenStudio for Performance Marketing, go to **[!UICONTROL More]** > **[!UICONTROL Settings]** > **[!UICONTROL ChatGPT]** > **[!UICONTROL Connect]** > **[!UICONTROL Add Account]**.
1. Enter the name of your OpenAI Ads account, paste in your API key, then click **[!UICONTROL Add Account]**.

## ChatGPT setup fields

Approved assets, headlines (Title), and body copy are locked and can't be edited during activation, since they already went through review and approval in [!DNL Content]. You can edit:

* **Text fields**: Target URL, Tracking ID (used as the platform ad name)
* **Platform setup fields**: OpenAI Ads account, OpenAI Campaign, OpenAI Ad group

Target URL must use a valid `https://` format, for example `https://www.example.com`.
