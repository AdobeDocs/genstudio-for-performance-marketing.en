---
title: Activate a The Trade Desk Ad
description: Learn how to activate a static display ad experience to The Trade Desk.
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
# Activate a The Trade Desk ad

Adobe GenStudio for Performance Marketing supports the activation of ad experiences to The Trade Desk.

**Supported formats**: Static Display (single-asset only).

Activating a The Trade Desk ad follows the [same general steps](create-activation.md) required for activation to other paid ad channels, with one difference: The Trade Desk is a managed enterprise service, not a self-service ad platform, so account access works differently than for other channels. This page covers those differences along with The Trade Desk-specific prerequisites and setup fields.

GenStudio system managers and editors can activate ad experiences.

## Prerequisites

* An existing, live The Trade Desk account. GenStudio for Performance Marketing cannot create a new The Trade Desk account on your behalf.
* API access enabled by your The Trade Desk account team. Unlike other paid ad channels, you cannot enable this access yourself, and the connection does not use OAuth.
* The correct advertiser, seat, and permissions enabled by The Trade Desk for the GenStudio for Performance Marketing integration.
* An API token or credentials from your The Trade Desk account team, with permissions to publish creatives to the target advertiser account.
* A destination campaign that already exists in The Trade Desk. GenStudio for Performance Marketing activates into an existing campaign only; it does not create or configure campaigns in The Trade Desk.

## Connect your The Trade Desk account

Before your organization can activate experiences, work with your The Trade Desk account team to enable API access, then a GenStudio system manager connects the account to GenStudio for Performance Marketing:

1. Contact your The Trade Desk account team and request access to publish creatives from GenStudio for Performance Marketing into your The Trade Desk account. Confirm which advertiser ID, seat, or partner details to use for activation.
1. Obtain the API token or credentials from your The Trade Desk account team, and confirm the token supports creative publishing permissions for the target advertiser account.
1. In GenStudio for Performance Marketing, go to **[!UICONTROL Settings]** > **[!UICONTROL Channels]**, then click **[!UICONTROL Connect]** on the **[!UICONTROL The Trade Desk]** tile. Enter the Account Name, Advertiser ID, and API token or credentials, then save the connection.

If the connection fails, confirm with your The Trade Desk account team that API access has been enabled and that the token has the correct advertiser and seat permissions.

## The Trade Desk setup fields

Approved assets are locked and can't be edited during activation, since they already went through review and approval in [!DNL Content]. You can edit:

* **Text fields**: Tracking ID (used as the platform creative name)
* **Platform setup fields**: Account, Campaign

At this time, activation to The Trade Desk supports single-asset static display ads only.
