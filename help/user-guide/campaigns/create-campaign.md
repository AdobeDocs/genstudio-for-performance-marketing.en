---
title: Adobe GenStudio for Performance Marketing Campaigns
description: Learn how to create and manage digital marketing campaigns that leverage generative-AI assets and experiences.
feature: Campaign Planning, Campaign Brief
badgeBeta: label="Beta" tooltip="This feature is currently in Beta, so some functionality may be limited or subject to change."
exl-id: b7c4194f-fa61-4739-acd6-7acbdd98e9b2
TQID: https://experienceleague.adobe.com/fcmU2HDzq75iNR7LlKqMcANCa67FpA0fFelMhkQtOJk
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
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
subfeature_v2:
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: b286a442-6f0d-405a-adea-abb4a98e2d7b
    internal-label: Campaign brief
  - id: bf1f49e6-dcda-4b68-a4d5-aeecf05031a6
    internal-label: Campaign planning
  - id: dd48f9df-f2e2-49fe-a918-332a8e240ffe
    internal-label: Channels
  - id: e3878dde-4b87-4290-9e81-ed7ee6eb83fe
    internal-label: Experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: beb7a3c1-66ab-4786-b879-7621375b3c40
    internal-label: Email marketing
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
---
# Create a campaign

A GenStudio for Performance Marketing campaign defines key digital campaign traits and evolves as stages are deployed and assessed. GenStudio for Performance Marketing supports the dynamic process of launching a campaign, tracking the performance of individual campaign components, and refocusing ad experiences based on performance metrics.

The key elements of your campaign are stored in a campaign object, which creates a shared context for all assets and experiences labeled with the same unique campaign name. This label identifies the campaign throughout GenStudio for Performance Marketing.

GenStudio system managers and GenStudio editors can create campaigns.

## Define campaign details

{{$include /help/_includes/campaign-details.md}}

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
