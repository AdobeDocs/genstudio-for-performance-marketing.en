---
title: Activate Meta ad
description: Learn how to activate a Meta ad experience.
feature: Experiences
---
# Activate a Meta ad

Adobe GenStudio for Performance Marketing supports the activation of Meta ads to Instagram and Facebook. The Activate a Meta ad workflow follows the same general steps described in [Create an activation](create-activations.md), but supports fine-tuning your approved experiences for Meta.

After activating your Meta experience in GenStudio for Performance Marketing, use Meta Ads Manager to fine-tune the experience for specific Meta ad placements. 

Here are the general steps for activating a Meta ad experience:

* Set up your Meta Ads Manager accounts.
* Prepare your ad experience in the _Creative setup_ view.
* Confirm your Meta account setup.
* Preview and activate your ad from Meta Ads Manager.

## Step 1: Set up your Meta accounts

Before launching an activation, confirm that your connected Meta ad accounts include:

* Facebook page
* Meta campaign
* Meta ad set
* Instagram profile (optional)

You must have permission to post content to Meta Ads Manager.

## Step 2: Connect to your Meta accounts

Data connectors enable the flow of data between marketing tools and GenStudio for Performance Marketing. Connect your Meta accounts to GenStudio for Performance Marketing before your organization can activate experiences.

Before you begin, confirm that GenStudio for Performance Marketing has permission to sync data and activate in Meta Ads Manager.

**To connect GenStudio for Performance Marketing with your Meta accounts**:

1. From _Settings_, click **[!UICONTROL Connect]** on the Meta Ads tile. The _Meta ads account_ view opens.

1. Select **[!UICONTROL Allow pop-ups]** from your browser, if prompted.

1. Select one or more of your ad accounts to connect, then click **[!UICONTROL Select]**.

After the sync has completed, you can view the added accounts. Large amounts of data take longer to sync.

## Step 3: Prepare your experience for activation

Only GenStudio system managers and editors can activate an ad experience.

1. From _[!DNL Activate]_, click **[!UICONTROL New]** on the Meta product tile. The _Creative setup_ view opens.

1. Assign a name to your experience. You can use this name to search for this experience in the _Activated experiences_ table.

### Select your media assets

Use the _Media_ section to select at least one image asset to include in your experience. Ad placements are associated with supported image aspect ratios, which are listed as options in the _Placements_ drop-down menu.

**To upload an asset from Content**:

1. From _[!DNL Activate]_, click **[!UICONTROL New]** on the Meta tile. The _Creative setup_ view opens.

1. Click **[!UICONTROL Select]**, then select **[!UICONTROL Select from Content]**.

1. Select the experience for upload. An _Activate Meta ad_ page opens. 

1. Select at least one asset for upload. Use the filter on the left to identify assets. 

1. Click Use to include the selected asset in your creative. 

If upload is unsuccessful, an informative error message that includes a link to the asset in _[!DNL Content]_, opens.

**To upload an asset**:

You can import up to six static images from either OneDrive or Dropbox. Select an aspect ratio for each image that you upload.

1. From _[!DNL Activate]_, click **[!UICONTROL New]** on the Meta tile. A popup opens, displaying a choice of selecting an experience from [!DNL Content] or uploading one from a device.

1. Click **[!UICONTROL Upload from device]**. The finder feature on your desktop opens.

1. Select the experience for upload. An _Activate Meta ad_ page for this experience opens. At least one asset must be uploaded.

**Select aspect ratios for your images**:

You can assign specific aspect ratios for visual assets in a creative. The _Placement_ menu displays the supported ad placements for Facebook posts or Instagram stories, organized by aspect ratio. GenStudio for Performance Marketing supports up to six aspect ratios. Select a specific channel placement.

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

Experience details are saved as metadata and aid users when searching for an experience and boost the experience's visibility in [!DNL Content]. Use these optional, user-defined details to identify the experience's purpose and the context, or campaigns, in which it is deployed.

| Detail     | Description |
|------------|-------------|
| Campaigns   | All GenStudio for Performance Marketing campaigns to which the ad experience belongs |
| Brand   | Guidelines that define organizational that are uploaded to GenStudio for Performance Marketing |
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

## Step 5: Preview and activate your ad

You can preview the ad in specific aspect ratios placements from the _Activate details_ view right panel. Use the dropdown menu to select a specific channel placement and aspect ratio to view. When you select a placement in the _Preview_ panel, only your view of the ad is affected. Your placement selection in the _Preview_ panel is not saved.

**To complete activation of your ad experience**:

Click **[!UICONTROL Publish]**. The complete Meta ad experience and its associated metadata are pushed directly into the selected Meta Ads Manager ad set. From Meta Ads Manager, you can manage the final steps of deploying the ad experience and Meta campaign.

## Log in to Meta Ads Manager to complete activation

After your activation has completed, you must log into Meta Ads Manager to review your ad experience and finalize publication to specific Meta channels.

