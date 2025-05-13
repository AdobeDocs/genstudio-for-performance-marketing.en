---
title: Adobe GenStudio for Performance Marketing Campaigns
description: Learn about creating a campaign.
feature: Campaign Planning, Campaign Brief
---
# Create a Campaign

A GenStudio for Performance Marketing campaign defines the essential characteristics of a digital campaign. Campaigns are dynamic, evolving as individual stages are deployed and as your team evaluate the success of each stage. GenStudio for Performance Marketing supports the dynamic process of launching a campaign, tracking the performance of individual campaign components, and refocusing ad experiences based on performance metrics.

The key elements of your campaign are stored in a campaign object, which creates a shared context for all assets and experiences labeled with the same unique campaign name. This label identifies the campaign throughout GenStudio for Performance Marketing.

GenStudio system managers and Genstudio editors can create a campaign.

## Step 1: Define campaign basics

Campaign basics, or details, define the foundational characteristics of your marketing campaign. These details are similar to the defining characteristics included in a campaign brief. 

Basic _Details_ fields are defined in this table:

| Detail     | Description |
|------------|-------------|
| Campaign name   | Unique name used to identify the campaign. This name is available as a campaign label through the product. |
| Description     | Summary of campaign for internal stakeholders   |
| Objective       | Primary goals of the campaign, such as increasing brand awareness, generating leads, or driving sales. |
| Key messaging   | Defines the central message to be communicated in all campaign assets.<br>Focuses content creators on the campaign's strategic message and tone.                                                                                              |
| Start           | The quarter, season, or year during which the ad experience becomes active.                       |
| End             | The quarter, season, or year during which the ad experience ends.                                 |
| Status          | Upcoming-Campaign starts in the future<br>Active-Campaign is in progress<br>Complete-Campaign ended |
| Last modified   | (Read-only) Timestamp that identifies the last time campaign details or content were edited.                  |

**To enter campaign details**:

1. From [!DNL Campaigns], click **[!UICONTROL Add campaign]**. The _Create a campaign_ view opens.

   Details encompass both optional and mandatory fields that define your campaign. These details are saved in [!DNL Content] as metadata attributes of the campaign.

1. Double-click the _New campaign_ header and enter an informative, unique name. This name becomes a _campaign label_ in GenStudio for Performance Marketing, allowing you to associate assets or experiences with the campaign during upload and creation.

1. Enter values in _Details_ fields that describe your campaign. Consult the _Campaign details_ table for definitions of these campaign features.

## Step 2: Assign channels and regions

Channel and region settings specify where the campaign is deployed and identify its distribution channels. GenStudio for Performance Marketing uses predefined templates, or _records_, to represent different objects. These object types include channels, regions, personas, and products. When you create a campaign, you associate these predefined personas, regions, products, and channel records with that campaign.

* Channel settings define the public distribution channels for your campaign, including paid media accounts, email marketing services, and display ad networks. GenStudio for Performance Marketing analyzes data from these channels about your active campaigns, assets, and experiences. [[!DNL Insights]](/help/user-guide/insights/overview.md) then processes this data to provide channel-specific performance analysis.

* Region settings specify where your campaign is deployed. Connecting regional data sources tailors content and strategy to local audience preferences and behaviors It also supports more precise targeting and performance analysis based on regional metrics.

**To select distribution channels for your campaign**:

1. Click the + sign (**[!UICONTROL Connect records +]**) next to **[!UICONTROL Channels]**.
   The _Select Channels_ popup opens.

1. Select the channels on which the campaign is deployed. Valid values include `Email`, `Paid media`, `Web`, and `Display ads`.
   Optionally, choose **[!UICONTROL See all]** to open a view of all supported channels.

**To assign regions to your campaign**:

1. Click the + sign (**[!UICONTROL Connect records +]**) next to **[!UICONTROL Regions]**.
   The _Select Regions_ popup opens. You can search for a specific supported region.

1. Select the regions in which your campaign is focused. Valid regions include `AMER`, `LATAM`, `EMEA`, `APAC`, and `Japan`.
   Optionally, choose **[!UICONTROL See all]** to open a view of all supported regions.

## Step 3: Assign personas and products

Personas and products are also saved as records. A Persona record, for example, defines the characteristics of a customer segment—your generated content's target audience. It can include information about demographics and history of customer interactions. The personas that are available in the Personas drop-down list are defined on an organization level by your organization's personas guidelines.

**To assign personas to your campaign**:

1. Click the + sign (**[!UICONTROL Connect records +]**) next to **[!UICONTROL Personas]**.
   The _Select Personas_ popup opens. You can search for a specific supported personas.

1. Select the personas that your campaign is targeting. Valid personas are defined by your organization during [guidelines creation](/help/user-guide/guidelines/personas.md).

   Optionally, choose **[!UICONTROL See all]** to open a view of all available personas.

**To assign products to your campaign**:

1. Click the + sign (**[!UICONTROL Connect records +]**) next to **[!UICONTROL Products]**.
   The _Select Products_ popup opens. You can search for a specific supported product.

1. Select the products that your campaign includes. Products are defined by your organization during [guidelines creation](/help/user-guide/guidelines/products.md).
   Optionally, choose **[!UICONTROL See all]** to open a view of all available products.

## Step 4: Complete campaign creation

Click **[!UICONTROL Create]** to save entered values and create the campaign.

The new campaign name is now available as a campaign label in [!DNL Content] and [!DNL Create]. You can add approved asset and experiences to your campaign through [!DNL Content], or assign an asset and experience to a campaign during content creation.

## Step 5: Add content to your campaign

GenStudio for Performance Marketing associates content with a campaign through the campaign label, which is saved in [!DNL Content] metadata. Content can belong to multiple campaigns.  A campaign label identifies the campaign and its attributes in [!DNL Content]. Associating a campaign label with an asset or experience links that content to the specific campaign. You can assign assets and experiences to multiple campaigns.

**To add content from [!DNL Content]**

1. From the [!DNL Content] _Experiences_ or _Assets_ gallery, choose the approved experience or asset you want to add.

1. From the _Details_ view, select the name of the campaign from the _Campaign_ dropdown menu.

**To add content during content creation**

During content creation, you can publish the newly created asset or experience to [!DNL Content].

1. From the _Confirm details for your approved content_ popup, select a campaign from the _Campaigns_ drop-down menu.

1. Click **[!UICONTROL Publish]**.

This campaign is now available in the _Campaigns_ view.
