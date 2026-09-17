---
title: Activation Workflow
description: Learn about the activation workflow for ad experiences.
feature: Ad Activation
exl-id: 17e1bade-d52a-4953-a85c-c10d093e73d6
TQID: https://experienceleague.adobe.com/HSwFeL1qCzgFao2Ii64Hx-kaADRnd3dxaswFMzJ7nfA
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
    internal-label: Channels
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
---
# Activation workflow

[!DNL Activate] activates published experiences to their paid ad platforms. A GenStudio for Performance Marketing experience is a marketing campaign component, such as an ad, that is prepared for a specific audience on a paid ad platform. Experiences for activation contain three main components:

* **Media assets**: Images or video included in your ad experience. Supported file types and aspect ratios vary by platform and format.

* **Text**: All forms of copy included in your ad, including headlines, body text, and call-to-action elements.

* **Metadata**: User-defined attributes that enhance performance analysis, filtering, and tracking. Metadata is typically not visible to the final ad audience.

You prepare and approve these components in [!DNL Content] before activation. [!DNL Activate] doesn't create or edit approved assets, headlines, or body copy. It only applies the setup each platform needs, then publishes the experience.

A single activation table can include experiences for multiple paid ad platforms and ad formats at once.

>[!VIDEO](https://video.tv.adobe.com/v/3503538?learn=on)

## Connect your platform accounts

A GenStudio system manager or editor must connect the ad accounts for each paid ad platform before you can activate an experience to that platform. To see the steps for this process, see [Connect paid media accounts](/help/user-guide/connectors/connect-channel.md).

## Start an activation

Start an activation from one of two entry points:

* **From [!DNL Content]**: Filter to Experiences, select one or more published experiences, then click **[!UICONTROL Activate]** on the top action bar.

  ![Selecting published experiences in Content and clicking Activate to start an activation](./images/content-select-activate.png)

* **From [!DNL Activate]**: On the [!DNL Activate] landing page, click **[!UICONTROL + New activation]**. This opens the same Experience gallery, where you select experiences for activation.

In either case, search by experience name or filter by multiple channels to find the experiences you want.

If your selection includes display-format experiences, specify which display platform to use: Google Campaign Manager 360, Innovid, Amazon Ads, or The Trade Desk. Then click **[!UICONTROL Start activation]**. For other formats, such as Meta, LinkedIn, TikTok, YouTube, and ChatGPT, [!DNL Activate] infers the platform from the experience's channel and skips this step.

[!DNL Activate] then generates an activation table listing all your selected experiences.

![A newly generated activation table grouped into Meta and LinkedIn sub-tables, with every ad flagged Needs attention until its fields are complete](./images/activation-table.png)

The table is organized into sub-tables by ad format and platform, for example Meta single image or LinkedIn single image. Each row represents one ad. For most platforms, such as LinkedIn, TikTok, and display platforms, an experience with multiple aspect ratios generates one row per aspect ratio; delete any rows you don't need. Meta is the exception. A Meta ad can include multiple aspect ratios within a single ad, so a multi-aspect-ratio Meta experience still generates only one row.

## Manage your activation table

Your activation table saves as a draft automatically when it opens. You can leave and resume the draft at any point before publishing.

To add more experiences to an activation table you already opened, click **[!UICONTROL Add more experiences]** in the top right of the table. This reopens the Experience gallery so you can select additional experiences, which [!DNL Activate] adds to the existing table.

**[!UICONTROL Add more experiences]** also lets you activate to more than one display platform in the same table. Display-format experiences ask you to choose a single display platform first, but you can click **[!UICONTROL Add more experiences]**, select more display-format experiences, and choose a different display platform than the one already in your table. For example, you can add The Trade Desk ads to a table that already contains Innovid ads.

Once your table has the right experiences, configure each ad's fields next.

## Configure ad and platform setup details

Edit fields inline per row, or select multiple rows within the same format table and click **[!UICONTROL Edit details]** on the toolbar that appears to bulk-edit those fields at once.

![Selecting multiple ads in an activation table to bulk-edit details or platform settings](./images/bulk-edit-action-bar.png)

Approved assets, headlines, and body copy are locked and can't be edited in the activation table, since they already went through review and approval in [!DNL Content]. The remaining fields can be edited, and vary by platform. [!DNL Activate] only shows the columns relevant to the platforms and formats you selected. Use the table below as a reference for what's editable per platform.

**Editable fields by platform**

| Platform | Formats supported | Locked copy | Editable text fields | Editable platform setup fields |
|---|---|---|---|---|
| Meta | Image, Video, Carousel | Headline, Body | Description, Call-to-action, Destination URL, URL Parameters, Tracking ID | Ad account, Facebook page, Instagram profile, Meta campaign, Meta ad set |
| LinkedIn | Single Image, Single Video | Headline, Introductory Text | Description, Call-to-action, Destination URL, URL Parameters, Tracking ID | Ad account, Campaign, Ad Set |
| Google Campaign Manager 360 | Static Display, Video Display, HTML5 Zip Display | n/a | Tracking ID | Advertiser |
| Amazon Ads | Static Display | n/a | Tracking ID | Account |
| Innovid | Static Display, HTML5 Zip Display | n/a | Tracking ID | Account, Creative Library, Concept Name |
| TikTok | In-Feed Video Ads | Primary Text | Call-to-action, Destination URL, Tracking ID | Ad account, Campaign, Ad group |
| YouTube | Shorts in Google Ads Demand Gen campaigns | Description | Call-to-action, Business name, Destination URL, URL Parameters, Tracking ID | Account, Campaign, Ad Group, Logo |
| ChatGPT | Chat Cards | Title, Body | Target URL, Tracking ID | OpenAI ad account, OpenAI Campaign, OpenAI Ad group |
| The Trade Desk | Static Display | n/a | Tracking ID | Account, Campaign |

To configure platform setup fields for a group of ad formats, click **[!UICONTROL Manage platform settings]** and edit the fields in the resulting dialog.

![The Manage platform settings dialog for choosing a Meta ad account, campaign, and ad set](./images/manage-platform-settings.png)

The **[!UICONTROL Tracking ID]** fields are initially blank. A Tracking ID is the same thing as the ad platform's ad name or creative name, and is passed to the ad platform as the identifying name for the ad. Use this field to identify that ad for reporting and troubleshooting. Enter the values you want to use in the **[!UICONTROL Tracking ID]** fields.

![Editing a Tracking ID field inline in the activation table](./images/tracking-id-edit.png)

To move between **[!UICONTROL Tracking ID]** fields more quickly, use these keyboard shortcuts:

* Press **Enter** to open the edit field for the selected **[!UICONTROL Tracking ID]**.
* Press the **Up** or **Down** arrow key to move to the previous or next **[!UICONTROL Tracking ID]** field in that column.
* Press **Enter** again to save your edit.

## Review and publish your experiences to their ad platforms

Confirm that every row shows [!UICONTROL Ready to Activate]. [!DNL Activate] flags missing or invalid fields, incompatible calls to action, and duplicate tracking IDs as [!UICONTROL Needs Attention]. When every row is ready, click **[!UICONTROL Send to platforms]** and confirm in the publish dialog.

![An activation table where every row shows Ready to activate, enabling Send to platforms](./images/ready-to-activate.png)

[!DNL Activate] reports each ad's status in near real time: Pending, then Sent to platforms or Failed. If an ad fails, hover over its status to see the platform's error. You can retry every failed ad in the table at once by clicking **[!UICONTROL Try again]**, rather than retrying each one individually. Rows already sent to platforms are locked from resubmission and include a deep link to the ad in the destination platform's native ad manager. Your final pre-publication review, and launching ads, happens in the destination platform's own ad manager: [!DNL Activate] always delivers ads in an inactive state.

![An activation table showing a mix of Pending and Sent to platforms statuses after publishing](./images/activation-status-pending.png)

Your activation tables appear on the [!DNL Activate] landing page.

## Supported platforms

Each paid ad platform has specific setup fields and prerequisites. Select the paid ad platform for activation guidelines:

* [Meta](activate-meta-ad.md)
* [LinkedIn](activate-linkedin-ad.md)
* [Google Campaign Manager 360](activate-cm360-ad.md)
* [Amazon Ads](activate-amazon-ad.md)
* [Innovid](activate-innovid-ad.md)
* [TikTok](activate-tiktok-ad.md)
* [YouTube](activate-youtube-ad.md)
* [ChatGPT](activate-chatgpt-ad.md)
* [The Trade Desk](activate-trade-desk-ad.md)
