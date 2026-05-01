---
title: Asset Details
description: Adobe GenStudio for Performance Marketing stores approved content with rich metadata for searchability and performance tracking.
feature: Generative AI, Content Attributes, Content Management
exl-id: 2be5cfee-f315-4ad6-8cf0-a8d3929b9ba3
TQID: https://experienceleague.adobe.com/Hm7qcrP6VcXf6IqZ2pYybduNyjjV8kdWj571gcRpglI
product_v2:
  - id: c4f2e613-b6a1-4be6-b2fc-6021190d498d
    internal-label: GenStudio for Performance Marketing
feature_v2:
  - id: bffd9bc2-7f41-4bf6-9f08-f14cbd37afd7
    internal-label: Campaigns
  - id: c7c3a4ab-6b96-4f2f-8931-4d2b360c3d12
    internal-label: Generative AI
  - id: c95c94c1-727b-457a-9184-a4dda4c95ab2
    internal-label: Insights
  - id: cd5564d5-2a4e-4a5a-8064-57a804f6fd3a
    internal-label: Create
  - id: f321b88b-6bb7-49cc-a16a-ae2b665ebd32
    internal-label: Content attributes
  - id: f71bd2fc-e9ca-4cb6-8088-82e250211e32
    internal-label: Guidelines
subfeature_v2:
  - id: a8b28c00-da6e-4d27-8667-80f790ad8972
    internal-label: Email experiences
  - id: a98e0185-3180-4e8c-8f31-f72af4cc21a2
    internal-label: Assets
  - id: b03d2162-d906-40a0-9cbd-001391e22d4a
    internal-label: Content performance
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
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: eb30f47f-d87a-400f-8f78-63ce7979ff56
    internal-label: Machine learning
---
# Asset details

Adobe GenStudio for Performance Marketing stores approved content with rich metadata for discoverability and performance tracking.

Each asset (including experiences and templates) has associated _details_ (metadata) that help to identify, track, use, and learn from content performance.

**To view asset details**:

1. In _[!DNL Content]_, select an asset, experience, or template. Clicking on an asset opens a focused view of the asset.

1. In the asset view, review the _[!UICONTROL Details]_ section on the right.

1. If the _[!UICONTROL Details]_ section is not visible, click the **[!UICONTROL Information]** (i) icon.

Asset details include metadata applied during the create or upload process. Asset metadata types include [system metadata](#system-metadata) and [user-defined metadata](#user-defined-metadata).

The following image asset contains system metadata describing the file type, size, and other characteristics, one user-defined keyword, and several AI-detected attributes and colors.

![details of an asset with multiple tags](/help/assets/content-asset-details.png)

>[!NOTE]
>
>Assets from AEM repositories display different metadata. See [Configure asset visibility](connect-aem-repo.md#step-4-configure-asset-visibility) to learn how to configure [!DNL AEM Assets Content Hub] asset details.

## System metadata

Some asset metadata is automatically collected when an asset is uploaded, such as file type, size, dimensions, source, and more. Except for the file name, you cannot edit default system metadata.

### Generated tags

When you store an approved asset in [!DNL Content], GenStudio for Performance Marketing uses Adobe's AI and machine learning capabilities to study the asset and apply tags based on the asset features. For example, a picture of a cat may result in attribute tags like `pet photography` or `cat`, and color tags that identify dominant colors in the picture. You cannot edit tags that are detected and automatically applied.

See [!DNL Insights] [Attribute categories](/help/user-guide/insights/attributes.md#categories) for detailed lists of image, video, and text features.

### Generated content metadata

The information used to generate a new asset or experience becomes metadata, such as the prompt that was used. You cannot edit the prompt once the content is approved, but you can use it as a starting place for generating something new.

## User-defined metadata

User-defined metadata adds marketing context to the asset's content, allowing marketers to understand how to use and engage with the asset.

When you [upload an asset](/help/user-guide/content/manage-assets.md#add-assets), you can define a set of optional asset details that exist in GenStudio for Performance Marketing as metadata. Including more details can improve asset identification in searches and filtering.

**To edit the user-defined metadata**:

1. In _[!DNL Content]_, select an asset, experience, or template. Clicking on an asset opens a focused view of the asset.

1. In the asset view, review the _[!UICONTROL Details]_ section on the right.

1. Click **[!UICONTROL Edit details]** (pencil) to edit asset, experience, or template metadata.

   The more details that you provide, the more you experience the robust capabilities of GenStudio for Performance Marketing. Select one or more details from the list, or enter a new one where applicable, such as with keywords. Each detail you add appears below the list. Click **`x`** to remove a detail.

### Metadata details

The following table details the metadata (asset details) that you can define when creating an asset.

| Field          | Description |
| -------------- | ----------- |
| Title          | Name of the asset; the default title may be the original filename |
| [!DNL Campaigns]| [[!DNL Campaigns]](/help/user-guide/campaigns/overview.md) include promotional content with consistent messaging for the purpose of achieving a business goal<br>Clicking on a campaign link takes you to the campaign's overview page |
| [!DNL Brands]  | [[!DNL Brands]](/help/user-guide/guidelines/brands.md) added to GenStudio for Performance Marketing and published for use |
| [!DNL Products]| [[!DNL Products]](/help/user-guide/guidelines/products.md) added to GenStudio for Performance Marketing for use |
| [!DNL Personas]| [[!DNL Personas]](/help/user-guide/guidelines/personas.md) added to GenStudio for Performance Marketing for use |
| Channels       | Platforms for distributing certain content types, such as email and Banner and Display ad |
| [!UICONTROL Timeframe] | Time frame for which the asset is used, such as quarter, season, year, etc. Example: `Winter 2023` |
| Region         | Regions for which the asset is used. Examples: `North America`, `APAC`, `Italy` |
| Language       | Languages for which the asset is used. Example: `Spanish` |
| Keywords       | User-defined keywords are used for further identification of asset characteristics and purpose |

>[!TIP]
>
>Click on **[!UICONTROL Edit details]** (pencil) to edit asset metadata. For example, you can change the asset name or add or remove keywords.

## Generative context

The [!UICONTROL Generative Context] section shows what information was used to generate the experience, such as the `Prompt` used during the [!DNL Create] process. This insight may help you to build even more successful variants.

Information may include:

- `Brand`, `Product`, and `Persona` parameters selected during the [!DNL Create] process
- `Subject line` and `Preheader` for email experiences
- `Headline` and `Body` for Meta ads

## History

Expand the _[!UICONTROL History]_ section in an experience to view a timeline of approvals and activity. For example, an approved experience reveals the approval date, time, and approver:

```
Approved

December 10, 2024 at 6:00 PM by Username
```
