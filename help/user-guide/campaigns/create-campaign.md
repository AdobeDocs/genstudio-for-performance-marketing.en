---
title: Adobe GenStudio for Performance Marketing Campaigns
description: Learn how to create and manage digital marketing campaigns that leverage generative-AI assets and experiences.
feature: Campaign Planning, Campaign Brief
badgeBeta: label="Beta" tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."
---
# Create a campaign

A GenStudio for Performance Marketing campaign defines key digital campaign traits and evolves as stages are deployed and assessed. GenStudio for Performance Marketing supports the dynamic process of launching a campaign, tracking the performance of individual campaign components, and refocusing ad experiences based on performance metrics.

The key elements of your campaign are stored in a campaign object, which creates a shared context for all assets and experiences labeled with the same unique campaign name. This label identifies the campaign throughout GenStudio for Performance Marketing.

GenStudio system managers and Genstudio editors can create campaigns.

## Define campaign details

Campaign details define the foundational characteristics of your marketing campaign. These details are similar to the defining characteristics included in a campaign brief.

Campaign _Details_ fields are defined in this table:

| Detail     | Description |
|------------|-------------|
| Campaign name   | Unique name used to identify the campaign. This name is available as a campaign label throughout the product. |
| Description     | Summary of campaign for internal stakeholders.   |
| Objective       | Primary goals of the campaign, such as increasing brand awareness, generating leads, or driving sales. |
| Key messaging   | Defines the central message to be communicated in all campaign assets.<br>Focuses content creators on the campaign's strategic message and tone.                                                                                              |
| Start           | The quarter, season, or year during which the ad experience becomes active.                       |
| End             | The quarter, season, or year during which the ad experience ends.                                 |
| Status          | Upcoming—Campaign starts in the future<br>Active—Campaign is in progress<br>Complete—Campaign ended |
| Last modified   | (Read-only) Timestamp that identifies the last time campaign details or content were edited.                  |

**To enter campaign details**:

1. From [!DNL Campaigns], click **[!UICONTROL Add campaign]**. The _Create a campaign_ view opens.

   Details encompass both optional and mandatory fields that define your campaign. These details are saved in [!DNL Campaigns] as metadata attributes of the campaign.

1. Double-click the _New campaign_ header and enter an informative, unique name. 
   
   This name becomes a _campaign label_ in GenStudio for Performance Marketing, allowing you to associate assets or experiences with the campaign during upload and creation.

1. Enter values in _Details_ fields that describe your campaign. Consult the _Campaign details_ table for definitions of these campaign features.

## Assign channels and regions

Channel and region settings determine where the campaign is deployed and its distribution channels.

GenStudio for Performance Marketing uses predefined templates called _records_ to represent key campaign components—such as channels, regions, personas, and products. When creating a campaign, you associate it with the relevant records for each of these components.

* **Channel settings**—Defines the public distribution channels for your campaign, including paid media accounts, email marketing services, and display ad networks. Data about the performance of campaigns, assets, and experiences in these channels is fed into [[!DNL Insights]](/help/user-guide/insights/overview.md) for channel-specific analysis.

* **Region settings**—Specifies the geographic areas where you deploy your campaign. By connecting to regional data sources, GenStudio for Performance Marketing can tailor content and strategy to local audience preferences. This enables more accurate targeting and performance analysis based on regional metrics.

**To select distribution channels for your campaign**:

1. Click the + sign (**[!UICONTROL Connect records +]**) next to **[!UICONTROL Channels]**.
   
   The _Select Channels_ popup opens.

1. Select the channels on which the campaign is deployed. Valid values include `Email`, `Paid media`, `Web`, and `Display ads`.
   
   Optionally, choose **[!UICONTROL See all]** to open a view of all supported channels.

**To assign regions to your campaign**:

1. Click the + sign (**[!UICONTROL Connect records +]**) next to **[!UICONTROL Regions]**.
   
   The _Select Regions_ popup opens. You can search for a specific supported region.

1. Select the regions one or more target regions for your campaign. Valid regions include `AMER`, `LATAM`, `EMEA`, `APAC`, and `Japan`.
   
   Optionally, choose **[!UICONTROL See all]** to open a view of all supported regions.

## Assign personas and products

[Personas](/help/user-guide/guidelines/personas.md) and [products](/help/user-guide/guidelines/products.md) are saved as records. A persona record defines the characteristics of a specific customer segment—your target audience for generated content. It may include demographic details and a history of customer interactions.

Product records define key product specifications and attributes in context of your brand guidelines. Attributes can include features, associated imagery, and product positioning within your brand.

The options in the _Personas_ and _Products_ drop-down menus are defined at the organizational level. When creating a campaign, you select from these predefined records to ensure consistent product representation and support accurate targeting, messaging, and performance tracking.

**To assign personas to your campaign**:

1. Click the + sign (**[!UICONTROL Connect records +]**) next to **[!UICONTROL Personas]**.
   
   The _Select Personas_ popup opens. You can search for a specific supported personas.

1. Select the personas that your campaign is targeting. Valid personas are defined by your organization during [guidelines creation](/help/user-guide/guidelines/personas.md).

   Optionally, choose **[!UICONTROL See all]** to open a view of all available personas.

**To assign products to your campaign**:

1. Click the + sign (**[!UICONTROL Connect records +]**) next to **[!UICONTROL Products]**.
   
   The _Select Products_ popup opens. You can search for a specific supported product.

1. Select one or more products. Products are defined by your organization during [guidelines creation](/help/user-guide/guidelines/products.md).
   
   Optionally, choose **[!UICONTROL See all]** to open a view of all available products.

## Complete campaign creation

Click **[!UICONTROL Create]** to save entered values and create the campaign.

The new campaign name is now available as a campaign label in [!DNL Content] and [!DNL Create]. You can add approved assets and experiences to your campaign through [!DNL Content], or assign an asset and experience to a campaign during content creation.

## Add content to your campaign

GenStudio for Performance Marketing links content to campaigns using campaign labels stored in [!DNL Content] metadata. A single piece of content can be associated with multiple campaigns.

Campaign labels identify the campaign and its attributes. Assigning a label to an asset or experience connects it to the corresponding campaign.

**To add assets and experiences from [!DNL Content]**:

1. From the [!DNL Content] _Experiences_ or _Assets_ gallery, choose the approved experience or asset.

1. From the _Details_ view, select the name of the campaign from the _Campaigns_ dropdown menu.

**To add assets and experiences during content creation**:

During content creation, you can publish the newly created asset or experience to [!DNL Content].

1. From the _Confirm details for your approved content_ popup, select a campaign from the _Campaigns_ drop-down menu.

1. Click **[!UICONTROL Publish]**.

This campaign is now available in the _Campaigns_ dashboard.
