---
title: Activate a Google Campaign Manager 360 ad
description: Learn how to activate a Google Campaign Manager 360 experience.
feature: Ad Activation
---
# Activate a Google Campaign Manager 360 ad

Adobe GenStudio for Performance Marketing supports the activation of Google Campaign Manager 360 ads, or creatives, to designated Campaign Manager 360 advertisers. GenStudio system managers and editors can activate creatives.

You can initiate activation of a Google Campaign Manager 360 ad experience from either the _[!DNL Content]_ gallery or  _[!DNL Activate]_ home.

## Step 1: Set up your Google Campaign Manager 360 accounts

Before launching an activation, [log in to your Google Campaign Manager 360 account](https://campaignmanager.google.com). Confirm that your connected Google Campaign Manager 360 accounts include access to Campaign Manager 360 advertisers. When you publish a Campaign Manager 360 creative from GenStudio for Performance Marketing, it is delivered to the advertiser selected during creative creation.

Campaign Manager 360 allows marketers to organize campaigns and their components into structured units called _advertisers_. Advertisers can group campaigns and related assets by client or product group, for example. Advertisers streamline the management of all aspects of selected campaigns, including creatives, landing pages, and audience properties.

## Step 2: Connect to your Google Campaign Manager 360 accounts

Before your organization can activate experiences, a GenStudio system manager needs to connect your Google Campaign Manager 360 accounts to GenStudio for Performance Marketing. This connection allows data to flow between GenStudio for Performance Marketing and external marketing tools such as Google Campaign Manager 360, enabling the activation process. See [Connect paid media accounts](/help/user-guide/settings/connect-channel.md).

After the sync is complete, you can view the added accounts. Large amounts of data take longer to sync.

## Step 3: Prepare your creative for activation

You can start the activation process from either the _[!DNL Content]_ Experience gallery or the _[!DNL Activate]_ home.

* _[!DNL Content]_ Experience gallery: Use only approved experiences. No editing of text or visual assets. Each experience can contain only one asset.
* _[!DNL Activate]_ home: Customize your creative during setup. Add or delete text and assets as needed.

### Prepare your creative from Content

You can prepare your creative by selecting an approved experience—can contain only one asset and is uneditable—from _[!DNL Content]_.

**To prepare your creative from _[!DNL Content]_**:

1. Select an experience from the _[!DNL Content]_ Experiences view for activation.

   Use the _[!DNL Content]_ gallery's search and filter tools to identify the experience you want to activate.

1. Click **[!UICONTROL Activate]** in the top right corner.

   The Google Campaign Manager 360 _Creative setup_ page opens for this experience. It is pre-populated with details, which you cannot revise, from the selected experience.

1. Select an advertiser from the **[!UICONTROL Advertiser]** drop-down menu.

   Your Google Campaign Manager 360 account settings determine the available advertisers.

After selecting your advertiser, click **[!UICONTROL Next]** to confirm your Google Campaign Manager 360 setup.

### Prepare your creative from Activate

Preparing a creative from _[!DNL Activate]_ provides an opportunity to select and edit exactly the assets and text you want to include.

1. From _[!DNL Activate]_, click **[!UICONTROL New]** on the Google Campaign Manager 360 product tile. The _Creative setup_ view opens.

1. Assign a name to your experience. After activation, you can use this name to search for this experience in the _Activated experiences_ table.

#### Select your media assets

Use the _Media_ section to select at least one image asset to include in your experience. Ad placements are associated with supported image aspect ratios, which are listed as options in the **[!UICONTROL Placements]** drop-down menu. This menu displays the supported ad placements for Facebook posts or Instagram stories, organized by aspect ratio.

GenStudio for Performance Marketing saves assets to _[!DNL Content]_ after upload. The _Media_ area displays the image by default with a 1:1 aspect ratio. Alternative aspect ratios include only the values supported by the paid ad channel. They are grouped by vertical and horizontal orientation. GenStudio for Performance Marketing supports the inclusion of up to six aspect ratios per activated experience.

**To upload an asset from Content**:

_[!DNL Content]_ provides a central view for your organization's approved assets and experiences. You can use the **[!UICONTROL Search]** (magnifying glass) and _Filter_ menu tools to refine your view of [_[!DNL Content]_ gallery](/help/user-guide/content/manage-assets.md) assets and experiences.

1. From _[!DNL Activate]_, click **[!UICONTROL New]** on the Google Campaign Manager 360 Ads tile. The _Creative setup_ view opens.

1. In the _Media_ section, click **[!UICONTROL Select]** and select **[!UICONTROL Select from Content]**.

   The _Select content_ view opens, displaying a gallery of image assets that you search through or filter.

1. Use _[!DNL Content]_ gallery's search and filter tools to select at least one asset for upload.

1. Click **[!UICONTROL Use]** to include the selected asset in your creative.

   The _Creative setup_ window includes the asset in its default aspect ratio in the _Media_ area. The _Preview_ panel previews the asset in the ad placement that supports this aspect ratio.

If upload is unsuccessful, an informative error message that includes a link to the asset in _[!DNL Content]_ opens.

**To upload an external asset**:

You can upload up to six static images that are external to the _[!DNL Content]_ gallery from either Microsoft OneDrive or Dropbox.

1. From _[!DNL Activate]_, click **[!UICONTROL New]** on the Google Campaign Manager 360 tile. The _Creative setup_ window opens.

1. In the _Media_ section, click **[!UICONTROL Select]** and select either **[!UICONTROL Select from Content]** or **[!UICONTROL Upload]**.

1. Click **[!UICONTROL Upload]**. The _Add aspect ratios_ window opens.

1. Select images by dragging and dropping image files into the image upload area.

   Alternatively, you can browse your device for assets. To upload assets from your device, click **[!UICONTROL Browse]**, then select _Browse files_ or _Browse folders_ to identify assets for upload.

1. In the _Add details_ area, add informative details to your uploaded assets to facilitate search and filtering in _[!DNL Content]_.

   These details are saved as metadata.

1. When you have uploaded your assets and assigned details, click **[!UICONTROL Add Assets]**.

#### Add ad text

Use the _Text_ section of the _Activate Google Campaign Manager 360 ad_ page to add compelling, brand-adherent text to required text fields. Text includes the primary (body) text for the ad and call-to-action text.

| Field           | Required                  | Character limit (max)           |
|-----------------|---------------------------|---------------------------------|
| Ad name         | yes                       | 500                             |
| Primary text    | yes                      | 500                             |
| Headline        | yes                      | 255                             |
| Description     | no                        | 125                             |
| Call to action  | yes                       | drop-down menu options only     |
| Display URL     | no                        | 1000                            |
| Website URL     | yes                       | 1000                            |
| Image           | at least one required     |                                 |

GenStudio for Performance Marketing requires _Primary text_ and _headline_, not Google.

#### Assign metadata

Experience details are saved as metadata and aid users when searching for an experience. Those details boost the experience's visibility in [!DNL Content]. Use these optional, user-defined details to identify the experience's purpose and the context, or campaigns, in which it is deployed.

| Detail     | Description |
|------------|-------------|
| Campaigns   | All GenStudio for Performance Marketing campaigns to which the ad experience belongs |
| Brand   | Guidelines, user-defined or default, that allow users to establish brand guidelines capturing the essence of a brand's identity. |
| Products   | Products associated with your organization and identified in GenStudio for Performance Marketing|
| Personas   | Personas associated with your organization and identified in GenStudio for Performance Marketing|
| Timeframe   | The quarter, season, year, or other organizationally defined unit of time during which the ad experience is active |
| Region   | Geographic region in which the experience is launched |
| Language   | Languages for which the ad experience is used |
| Keywords   | User-defined keywords that facilitate the search and categorization of the ad experience |

After assembling your creative, click **[!UICONTROL Next]** to confirm your Google Campaign Manager 360 setup.

## Step 4: Confirm Google Campaign Manager 360 account setup

After preparing your creative, you must confirm the Google Campaign Manager 360 account advertiser and assign a tracking ID to the creative. The Google Campaign Manager 360 account view is populated with options that are derived from the configured Google Campaign Manager 360 accounts.

### Tracking ID

Tracking IDs (ad name) provide a mechanism for collecting metrics that are linked to the experience performance. Enter the ad name in this field.

Click **[!UICONTROL Next]** in the upper right to preview your ad experience and finalize activation.

## Step 5: Preview and activate your ad

The _Review_ page displays your ad experience as assembled in the _Creative setup_ and provides a final opportunity to view and edit your experience.

If you launched this activation from Activate, you can click **[!UICONTROL Edit section]** next to the _Creative setup_ label to make your changes. You can also click **[!UICONTROL Back]** in the upper right to return to the _Creative setup_ page. Experiences directly selected from Content cannot be edited.

### Step 6: Complete activation of your ad experience

1. Click **[!UICONTROL Publish]**.

   The complete Campaign Manager 360 ad experience and its associated metadata are pushed directly into the selected Campaign Manager 360 advertiser. Creatives are delivered to their target channel in an inactive state. From Campaign Manager 360, you can manage the final steps of deploying the creative and campaign.

1. [Log in to your Google Campaign Manager 360 account](https://campaignmanager.google.com) to review your ad experience and finalize publication to specific Campaign Manager 360 channels.
