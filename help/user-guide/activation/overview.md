---
title: Overview of Activate
description: Learn how to activate content with Adobe CX Enterprise and third-party applications.
level: Beginner
feature: Ad Activation
exl-id: 365fe253-d189-467e-a723-f54cd74ff60b
TQID: https://experienceleague.adobe.com/-Nal0YqjTzKw4g2SM3IuMf0a13e87CWdTqBZPd0dBkU
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
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
---
# Adobe GenStudio for Performance Marketing Activate

GenStudio for Performance Marketing [!DNL Activate] is where you prepare and send ad experiences to paid ad channels, such as Meta or LinkedIn. _Activation_ takes an approved ad experience and its assets, applies the setup a specific channel requires, then directly delivers it to that channel in an inactive, off status. From there, you can do a final review in the channel's own ad manager before your ad goes live.

[!DNL Activate] sends your experience straight to the channel: you don't need to export files or manually upload them to the channel's own ad manager.

A GenStudio system manager or editor must connect the ad account for each paid ad channel before you can activate an ad experience to that channel.

## Activate capabilities

Use [!DNL Activate] to prepare ad experiences for their target paid ad channels. [Activate experiences in bulk](create-activation.md) across multiple paid ad channels in a single activation table, then [manage your activations](manage-activations.md) to see the status and details of every activated experience.

>[!VIDEO](https://video.tv.adobe.com/v/3503538?learn=on)

### Activate approved experiences from Content

Select one or more approved, published experiences from [!DNL Content], or start from the [!DNL Activate] landing page. Unlike earlier versions of [!DNL Activate], a single activation table can include experiences for multiple paid ad channels at once, organized by ad format and channel.

>[!NOTE]
>
>[!DNL Content] calls a destination like Meta or LinkedIn a **channel**. [!DNL Activate] calls the same destination a **platform** (for example, in **[!UICONTROL Platform setup]**). The two terms refer to the same thing.

### Configure ad and platform setup details

Each row in the activation table represents one ad. Approved creative assets, headlines, and body copy are locked because they already went through review and approval. You can edit the remaining fields, such as call-to-action text, destination URL, and platform setup details like the ad account, campaign, and ad set. Edit fields for one row at a time, or select multiple rows to edit shared fields in bulk.

### Review and publish your experiences to their ad channels

Confirm that every row shows [!UICONTROL Ready to Activate]. [!DNL Activate] flags missing or invalid fields, incompatible calls to action, and duplicate tracking IDs as [!UICONTROL Needs Attention]. When every row is ready, click **[!UICONTROL Send to Platform]** to publish all ads in the table. [!DNL Activate] reports each ad's status in near real time, and successfully published ads include a deep link to the ad in the destination platform's native ad manager. Failed ads return an error message and can be retried.
