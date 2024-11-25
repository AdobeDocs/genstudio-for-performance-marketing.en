---
title: Asset details
description: Adobe GenStudio for Performance Marketing stores approved content with rich metadata for searchability and performance tracking.
feature: Attributes, Assets
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
---
# Asset details

Adobe GenStudio for Performance Marketing stores approved content with rich metadata for discoverability and performance tracking.

Each asset (including experiences and templates) has associated _details_ (metadata) that help to identify, track, use, and learn from content performance.

**To view asset details**:

1. In _[!DNL Content]_, select an asset, experience, or template. Clicking on an asset opens a focused view of the asset.

1. In the asset view, review the _[!UICONTROL Details]_ section on the right.

   >[!TIP]
   >
   >If the _[!UICONTROL Details]_ section is not visible, click the **[!UICONTROL Information]** (i) icon.

Asset details include metadata applied during the creation or upload process. Asset metadata types include [system metadata](#system-metadata) and [user-defined metadata](#user-defined-metadata).

The following asset contains system metadata describing the file type, size, and other characteristics, one user-defined keyword, and several AI-detected attributes and colors.

![details of an asset with multiple tags](/help/assets/content-asset-details.png)

>[!NOTE]
>
>Assets from AEM repositories display different metadata. See [Configure asset visibility](connect-aem-repo.md#step-4-configure-asset-visibility) to learn how to configure [!DNL AEM Assets Content Hub] asset details.

## System metadata

Some asset metadata is automatically collected when an asset is uploaded. You cannot edit default system metadata.

Default metadata that is stored and captured for an asset include the file's name, dimensions, source, and more.

### Generated tags

When you store an approved asset in [!DNL Content], GenStudio for Performance Marketing uses Adobe's AI and machine learning capabilities to study the asset and apply tags based on the asset features. For example, a picture of a cat may result in attribute tags like `pet photography` or `cat`, and color tags that identify dominant colors in the picture. You cannot edit tags that are detected and automatically applied.

See [!DNL Insights] [Attribute categories](/help/user-guide/insights/attribute-category.md) for detailed lists of image, video, and text features.

### Generated content metadata

The information used to generate a new asset or experience becomes metadata, such as the prompt that was used. You cannot edit the prompt once the content is approved, but you can use it as a starting place for generating something new.

## User-defined metadata

User-defined metadata adds marketing context to the asset's content, allowing marketers to understand how to use and engage with the asset.

When you [upload an asset](/help/user-guide/content/manage-assets.md#add-assets), you can define a set of optional asset details that exist in GenStudio for Performance Marketing as metadata. Including more details can improve asset identification in searches and filtering.

### Metadata details

The following table details the metadata (asset details) you can define when creating an asset.

| Field         | Description |
| ------------- | ----------- |
| Campaigns (project name) | Default metadata captured and stored with the asset |
| [!DNL Brands]    | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) added to GenStudio for Performance Marketing and published for use |
| [!DNL Products]      | [[!DNL Products]](/help/user-guide/guidelines/products.md) added to GenStudio for Performance Marketing for use |
| [!DNL Personas]      | [[!DNL Personas]](/help/user-guide/guidelines/personas.md) added to GenStudio for Performance Marketing for use |
| Channels      | Content types in GenStudio for Performance Marketing the asset is used for, such as email and Meta ads |
| Timeframe     | Timeframe for which the asset is used, such as quarter, season, year, etc. Example: `Winter 2023` |
| Region        | Regions for which the asset is used. Examples: `North America`, `APAC`, `Italy` |
| Language      | Languages for which the asset is used. Example: `Spanish` |
| Keywords      | User-defined keywords used for further identification of asset characteristics and purpose |

<!-- ## History

Expand the _[!UICONTROL History]_ section to view a timeline of approvals and activity.

list other activity, show screenshot?
-->
