---
title: Activate Meta ad
description: Learn how to activate a Meta ad experience.
feature: Experiences
---
# Activate a Meta ad

Adobe GenStudio for Performance Marketing supports the activation of Meta ads, or creatives, to Instagram and Facebook.

You can [create a Meta experience](/help/user-guide/create/create-meta-ad.md) in GenStudio for Performance Marketing and select it for activation, or construct a new experience from approved assets in [!DNL Activate].

Activating a Meta ad follows the [same general steps](create-activations.md) required to activate to other paid channels. It supports preparing your ad experiences for Meta's specific requirements. After your Meta experience, or creative, is complete in GenStudio for Performance Marketing, use Meta Ads Manager to fine-tune the experience for specific Meta ad placements before final publication.

## Step 1: Set up your Meta accounts

Before launching an activation, [log in to Meta](https://adsmanager.facebook.com/) to access your Meta Ads Manager account. Confirm that your connected Meta ad accounts include:

* Facebook page
* Meta campaign
* Meta ad set
* Instagram profile (optional)

You must have permission to post content to Meta Ads Manager. 

## Step 2: Connect to your Meta accounts

Data connectors enable the flow of data between marketing tools and GenStudio for Performance Marketing. A GenStudio system manager must connect your Meta accounts to GenStudio for Performance Marketing before your organization can activate experiences. 

**To connect GenStudio for Performance Marketing with your Meta accounts**:

1. From _Settings_, click **[!UICONTROL Connect]** on the Meta Ads tile. The _Meta ads account_ view opens.

1. Select **[!UICONTROL Allow pop-ups]** from your browser, if prompted.

1. Select one or more of your ad accounts to connect, then click **[!UICONTROL Select]**.

After the sync has completed, you can view the added accounts. Large amounts of data take longer to sync.

## Step 3: Prepare your experience for activation

GenStudio system managers and editors can activate ad experiences.

1. From _[!DNL Activate]_, click **[!UICONTROL New]** on the Meta product tile. The _Creative setup_ view opens.

1. Assign a name to your experience. After activation, you can use this name to search for this experience in the _Activated experiences_ table.

### Select your media assets

Use the _Media_ section to select at least one image asset to include in your experience. Ad placements are associated with supported image aspect ratios, which are listed as options in the _Placements_ drop-down menu.

#### Aspect ratios

Selecting an image asset for your ad experience, or creative, requires choosing an appropriate aspect ratio. Aspect ratios define the proportional relationship between an image's width and height, and they are crucial for the effectiveness of ad placements. Paid media channels carefully specify valid aspect ratios for each ad placement on their platform.

The _Creative setup_ > _Placement_ menu displays the supported ad placements for Facebook posts or Instagram stories, organized by aspect ratio.

When adding image assets to your activation, you must select the aspect ratio based on the final ad placements for your experience. File types are restricted to JPEG, PNG, and GIF.

After you have added assets to your experience, the _Creative setup_ _Media_ area displays the image by default with a 1:1 aspect ratio. Alternative aspect ratios include the values that the paid ad channel supports. They are grouped by vertical and horizontal orientation. GenStudio for Performance Marketing supports the inclusion of up to six aspect ratios per activated experience.

#### Upload from Content

_[!DNL Content]_ provides a central view for your organization's approved assets and experiences. You can focus the [_[!DNL Content]_  gallery](/help/user-guide/content/manage-assets.md) displayed inventory of assets using the **[!UICONTROL Search]** (magnifying glass) and _Filter_ menu options. 

**To upload an asset from Content**:

1. From _[!DNL Activate]_, click **[!UICONTROL New]** on the Meta Ads tile. The _Creative setup_ view opens.

1. Click **[!UICONTROL Select]**, then select **[!UICONTROL Select from Content]**. The _Select content_ view opens, displaying a gallery of image assets that you search through or filter.

1. Use _[!DNL Content]_ gallery's search and filter tools to select at least one asset for upload.

1. Click **[!UICONTROL Use]** to include the selected asset in your creative. The _Creative setup_ window includes the asset in its default aspect ratio in the _Media_ area. The _Preview_ panel previews the asset in the ad placement that supports this aspect ratio.

If upload is unsuccessful, an informative error message that includes a link to the asset in _[!DNL Content]_, opens.

#### Upload an external asset

You can upload up to six static images external to the _[!DNL Content]_ gallery from either Microsoft OneDrive or Dropbox. Select an aspect ratio for each image that you upload. After upload, assets are saved to _[!DNL Content]_.

**To upload an external asset**:

1. From _[!DNL Activate]_, click **[!UICONTROL New]** on the Meta tile. The _Creative setup_ window opens.

1. In the _Media_ section, click **[!UICONTROL Select]**. A drop-down menu displays options to _Select from Content_ or _Upload_.

1. Click **[!UICONTROL Upload]**. The _Add aspect ratios_ window opens.

1. Select images in the supported aspect ratios by dragging and dropping image files into the image upload area. Alternatively, you can browse your device for assets.

1. (Optional) To upload assets from your device, click **[!UICONTROL Browse]**, then select _Browse files_ or _Browse folders_ to identify assets for upload.

1. In the _Add details_ area, add informative details to your uploaded assets to facilitate search and filtering in _[!DNL Content]_. These details are saved as metadata.

1. When you have uploaded your assets and assigned details, click **[!UICONTROL Add Assets]** on the bottom right.

#### Preview ad placements

The _Preview panel_ on the _Creative_ setup page lets you interactively view your text and assets in the context of a specific ad placement. Use the _Select placement_ drop-down menu to switch among supported ad placements. Previews provide the opportunity to finalize decisions about ad elements for specific placements. When you select a placement in the _Preview_ panel, only your view of the ad is affected. Your placement selection in the _Preview_ panel is not saved.

### Add ad text

Use the _Text_ section of the _Activate Meta ad_ page to add compelling, brand-adherent text to required text fields. Text includes the primary (body) text for the ad and call-to-action text.

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

_Primary text_ and _headline_ are required by GenStudio for Performance Marketing only, not Meta.

### Assign metadata

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

After assembling your creative, click **[!UICONTROL Next]** to confirm your Meta setup.

## Step 4: Confirm Meta account setup

After preparing your creative, you must confirm your Meta account information and assign a tracking ID to the ad experience. The _Meta ad setup_ view is populated with options that are derived from the configured Meta accounts.

| Detail     | Description |
|------------|-------------|
| Accounts   | Meta accounts that have been connected to GenStudio for Performance Marketing |
| Facebook page   | Facebook page where the experience is published |
| Instagram account   | Instagram accounts that have been connected to GenStudio for Performance Marketing|
| Campaigns    | Meta campaigns to which the ad experience belongs |
| Ad sets   |Meta ad sets to which the activated ad experience belongs. The settings determine the final placements of the ad. |

### Tracking ID

Tracking IDs (ad name) provide a mechanism for collecting metrics that are linked to the experience performance. Enter the ad name in this field.

Click **[!UICONTROL Next]** in the upper right to preview your ad experience and finalize activation.

## Step 5: Preview and activate your ad

The _Review_ page displays your ad experience as assembled in the _Creative setup_ and provides a final opportunity to view and edit your experience. Click **[!UICONTROL Edit section]** next to the _Creative setup_ label to make your changes. You can also click **[!UICONTROL Back]** in the upper right to return to the _Creative setup_ page.

### Complete activation of your ad experience

Click **[!UICONTROL Publish]**. The complete Meta ad experience and its associated metadata are pushed directly into the selected Meta Ads Manager ad set. Experiences are delivered to Meta Ads Manager inactivated. From Meta Ads Manager, you can manage the final steps of deploying the ad experience and Meta campaign.

## Log in to Meta Ads Manager to complete activation

After your activation completes, you must log in to Meta Ads Manager. From [Meta Ads Manager](https://adsmanager.facebook.com/), you can review your ad experience and finalize publication to specific Meta channels.
