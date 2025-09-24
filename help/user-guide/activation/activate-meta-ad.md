---
title: Activate a Meta Ad
description: Learn how to activate a Meta ad experience.
feature: Ad Activation
exl-id: 157df612-a774-422c-bca3-2fde9e9d1c88
---
# Activate a Meta ad

Adobe GenStudio for Performance Marketing supports the activation of Meta ad experiences to Instagram and Facebook.

You can [create a Meta experience](/help/user-guide/create/create-meta-ad.md) in GenStudio for Performance Marketing and select it for activation, or construct a new experience from approved assets in [!DNL Activate].

Activating a Meta ad follows the [same general steps](create-activation.md) required for activation to other paid channels. The activation process supports preparing your ad experience for Meta's specific requirements. After you activate a Meta experience in GenStudio for Performance Marketing, use [Meta Ads Manager](https://adsmanager.facebook.com/) to fine-tune the experience for specific Meta ad placements before final publication.

GenStudio system managers and editors can activate ad experiences.

## Step 1: Set up your Meta accounts

Before launching an activation, [log in to Meta](https://adsmanager.facebook.com/) to access your Meta Ads Manager account.

>[!BEGINSHADEBOX]

**Prerequisites**:

Confirm that your connected Meta ad accounts have full permission to manage ads in these components of the Meta advertising platform:

* Facebook page
* Meta campaign
* Meta ad set
* Instagram profile (optional)

>[!ENDSHADEBOX]

## Step 2: Connect to your Meta accounts

Before your organization can activate experiences, a GenStudio system manager must connect your Meta accounts to GenStudio for Performance Marketing. This connection allows data to flow between GenStudio and external marketing tools such as Meta, enabling the activation process.

See [Connect to Meta Ads](/help/user-guide/connectors/meta-ads.md).

After the sync has completed, you can view the added accounts. Large amounts of data take longer to sync.

## Step 3: Prepare your experience for activation

You can launch an activation in two ways:

* **Activate directly from [!DNL Content]**. Selecting an approved experience with predefined settings is the most streamlined way to launch an activation to a single channel.

* **Assemble your ad experience from [!DNL Activate] > _Experience setup_**. You can create an experience by selecting visual assets from [!DNL Content], adding text elements, and selecting aspect ratios. This approach has more steps but provides greater flexibility when crafting your creative experience.

### Activate an approved experience from Content

You can select more than one experiences to activate to a single paid channel. You may be asked to select a platform before continuing with activation.

If you have selected more than one experience to activate as a group, use the left sidebar to focus the _Experience setup_ view on the selected experience's details.

1. Use the [!DNL Content] gallery's search and filter tools to identify the experience you want to activate, then click **[!UICONTROL Activate]**.

   The Meta ads _Experience setup_ page opens for this experience. It is pre-populated with details from the selected experience. You can edit the **[!UICONTROL Call-to-action]**, **[!UICONTROL Website URL]**, and **[!UICONTROL Display link]** fields. If you select more than one experience to activate, the _Experience setup_ view includes a left sidebar that displays thumbnails of all selected experiences. Use this left sidebar to focus the _Experience setup_ view on the selected experience's details.

1. Select a campaign from the **[!UICONTROL Campaigns]** drop-down menu.

   If you are working with multiple experiences, toggle through experiences on the left sidebar until you have completed preparing each experience.

1. Click **[!UICONTROL Next]** to confirm your Meta ads setup.

1. Assign a name to each experience. After activation, you can use this name to search for this experience in the _Activated experiences_ table.

### Assemble experience components

If you choose not to directly activate an approved experience from [!DNL Content], you can select assets, assign aspect ratios, and draft text elements.

**To prepare your experience for activation**:

1. From [!DNL Activate], click **[!UICONTROL New]** on the icon representing your chosen paid channel. The _Experience setup_ view opens.

   The _Experience setup_ page provides a central location for preparing your ad activation. Preparing your ad includes these three tasks:

1. Assign a name to your experience. After activation, you can use this name to search for this experience in the _Activated experiences_ table.
1. Select media assets. You can use assets from [!DNL Content] or upload external assets (for example, from OneDrive or Dropbox).
1. [Add text](#add-ad-text).
1. [Add metadata](#assign-metadata).

   The _Preview panel_ supports an interactive view of your text and assets in the context of a specific ad placement. Use the _Select placement_ drop-down menu to switch among supported ad placements. Previews provide the opportunity to finalize decisions about ad elements for specific placements. When you select a placement in the _Preview_ panel, only your view of the ad is affected. Your placement selection in the _Preview_ panel is not saved.

### Select your media assets

Use the _Media_ section to select at least one image asset to include in your experience. Ad placements are associated with supported image aspect ratios, which are listed as options in the _Placements_ drop-down menu. This menu displays the supported ad placements for Facebook posts or Instagram stories, organized by aspect ratio.

After upload, assets are saved to [!DNL Content]. The _Media_ area displays the image by default with a 1:1 aspect ratio. Alternative aspect ratios include only the values supported by the paid ad channel. They are grouped by vertical and horizontal orientation. GenStudio for Performance Marketing supports the inclusion of up to six aspect ratios per activated experience.

**To upload an asset from Content**:

[!DNL Content] provides a central view for your organization's approved assets and experiences. You can focus the [[!DNL Content] gallery](/help/user-guide/content/manage-assets.md) displayed inventory of assets using the **[!UICONTROL Search]** (magnifying glass) and _Filter_ menu options.

1. From [!DNL Activate], click **[!UICONTROL New]** on the channel card. The _Experience setup_ view opens.

1. Click **[!UICONTROL Select]**, then select **[!UICONTROL Select from Content]**. The _Select content_ view opens, displaying a gallery of image assets that you search through or filter.

1. Use [!DNL Content] gallery's search and filter tools to select at least one asset for upload.

1. Click **[!UICONTROL Use]** to include the selected asset in your ad experience. The _Experience setup_ window includes the asset in its default aspect ratio in the _Media_ area. The _Preview_ panel previews the asset in the ad placement that supports this aspect ratio.

If upload is unsuccessful, an informative error message that includes a link to the asset in _[!DNL Content]_ opens.

**To upload an external asset**:

You can upload up to six static images external to the [!DNL Content] gallery from either Microsoft OneDrive or Dropbox.

1. From [!DNL Activate], click **[!UICONTROL New]** on the Meta tile. The _Experience setup_ window opens.

1. In the _Media_ section, click **[!UICONTROL Select]**. A drop-down menu displays options to _Select from Content_ or _Upload_.

1. Click **[!UICONTROL Upload]**. The _Add aspect ratios_ window opens.

1. Select images in the supported aspect ratios by dragging and dropping image files into the image upload area. Alternatively, you can browse your device for assets.

1. (Optional) To upload assets from your device, click **[!UICONTROL Browse]**, then select _Browse files_ or _Browse folders_ to identify assets for upload.

1. In the _Add details_ area, add informative details to your uploaded assets to facilitate search and filtering in _[!DNL Content]_. These details are saved as metadata.

1. When you have uploaded your assets and assigned details, click **[!UICONTROL Add Assets]** on the bottom right.

### Add ad text

Use the _Text_ section of the _Activate Meta ad_ page to add compelling, brand-adherent text to required text fields. Text includes the primary (body) text for the ad and call-to-action text. You cannot edit the _Primary text_, _Headlines_, and _Description_ fields. You can edit the _Call-to-action_, _Display link_, and _Website URL_ fields.

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

GenStudio for Performance Marketing requires _Primary text_ and _headline_, not Meta.

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

After assembling or selecting your experience, click **[!UICONTROL Next]** to confirm your Meta setup.

## Step 4: Confirm Meta account setup

After preparing your ad experiences, you must confirm your Meta account information. The _Meta ad setup_ view is populated with options that are derived from the configured Meta accounts.

| Detail     | Description |
|------------|-------------|
| Accounts   | Meta accounts that have been connected to GenStudio for Performance Marketing |
| Facebook page   | Facebook page where the experience is published |
| Instagram account   | Instagram accounts that have been connected to GenStudio for Performance Marketing|
| Campaigns    | Meta campaigns to which the ad experience belongs |
| Ad sets   |Meta ad sets to which the activated ad experience belongs. The settings determine the final placements of the ad. |

### Create a new ad set

You can create a new ad set during platform setup by cloning an existing ad set during platform setup. Meta ad sets define the timing, channel details, and audience for a specific ad. A Meta campaign can contain multiple ad sets, but an ad set is exclusively associated with one campaign. 

**To create a new ad set**:

1. Select a campaign from the _Meta campaigns_ drop-down menu.
   
   The selected campaign determines the ad sets available as options in the _Ad sets_ drop-down menu.

1. Click **[!UICONTROL + Create new ad set]**.
   
   The _Create new ad set_ popup opens, identifying the Meta campaign where the new ad set is created.

1. Select the ad set you want to clone from the _Use configuration from_ drop-down menu.
   
   GenStudio for Performance Marketing assigns a default ad set name by appending `- Copy` to the selected ad set name.

1. (Optional but recommended) Enter a unique ad name in the **[!UICONTROL New ad set name]** field to replace the default value. 

1. Click **[!UICONTROL Create ad set]**.

   You are returned to the _Platform setup_ view, where the new ad set is pre-selected. A success message appears, including a link to the ad set in Meta Ads Manager. This ad set is available for future activations.

>[!NOTE]
>
>If the ad set is successfully created but the ad set name could not be saved, the ad set is saved in Meta Ads Manager under its default name (_original ad set name - Copy_).

### Tracking ID

Tracking IDs (ad name) provide a mechanism for collecting metrics that are linked to the experience performance. Enter the ad name in this field.

Click **[!UICONTROL Next]** in the upper right to preview your ad experience and finalize activation.

## Step 5: Preview and activate your ad

The _Review_ page displays your ad experience as assembled in the _Experience setup_ and provides a final opportunity to view and edit your experience. Click **[!UICONTROL Edit section]** next to the _Experience setup_ label to make your changes. You can also click **[!UICONTROL Back]** in the upper right to return to the _Experience setup_ page.

### Step 6: Complete activation of your ad experience

1. Click **[!UICONTROL Publish]**.

   The complete Meta ad experience and its associated metadata are pushed directly into the selected Meta Ads Manager ad set. Experiences are delivered to Meta Ads Manager in an inactive state. From Meta Ads Manager, you can manage the final steps of deploying the ad experience and Meta campaign.

1. [Log in to Meta Ads Manager](https://adsmanager.facebook.com/) to review your ad experience and finalize publication to specific Meta channels.
