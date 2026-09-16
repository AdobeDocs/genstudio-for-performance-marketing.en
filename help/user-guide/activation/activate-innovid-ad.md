---
title: Activate a Innovid Ad
description: Learn how to activate a Innovid experience.
feature: Ad Activation
exl-id: ebb2aa9e-8efb-45b0-9ba2-7b27b8888708
TQID: https://experienceleague.adobe.com/VTzk2CDlTqawM1ckdHPVzs2ES-y0Ui0mkOLnVD88bJk
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
---
# Activate an Innovid ad

Adobe GenStudio for Performance Marketing supports the activation of ad experiences to Innovid.

**Supported formats**: Static Display, HTML5 Zip Display.

Activating an Innovid experience follows the [same general steps](create-activation.md) required for activation to other paid ad channels. This page covers Innovid-specific prerequisites and setup fields. After you activate an experience in GenStudio for Performance Marketing, use Innovid to review the experience and launch the ad.

GenStudio system managers and editors can activate ad experiences.

## Prerequisites

* Access to the target Innovid account.
* Admin access to that account, to read from and write to Innovid.

Innovid organizes campaigns and ads within different accounts, and each account has a creative library. The target creative library must already exist in Innovid; GenStudio for Performance Marketing publishes ad experiences into that creative library, but does not create accounts or creative libraries.

## Connect your Innovid account

Before your organization can publish assets in a creative library, a GenStudio system manager must connect your Innovid account to GenStudio for Performance Marketing. You must have admin access to that account to read from and write to Innovid. See [Connect paid media accounts](/help/user-guide/connectors/connect-channel.md).

After the sync completes, you can view the added accounts.

## Innovid setup fields

Approved assets are locked and can't be edited during activation, since they already went through review and approval in [!DNL Content]. You can edit:

* **Text fields**: Tracking ID (used as the platform creative name)
* **Platform setup fields**: Account, Creative Library, Concept Name

Your creative experience is delivered to the selected creative library in Innovid when activation completes.
